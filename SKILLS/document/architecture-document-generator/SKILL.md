---
name: architecture-document-generator
description: 分析项目代码库和业务上下文，自动提取系统架构信息，生成符合 C4 模型标准的项目架构文档（ARCHITECTURE.md），包含系统上下文、容器图、组件图及架构决策记录（ADR）。
version: 1.0.0
author: System
tags:
  - architecture
  - documentation
  - c4-model
  - adr
  - engineering
---

# Skill: 架构文档生成器 (Architecture Documentation Generator)

## 1. 核心定位
本 Skill 旨在将非结构化的项目信息（代码库、业务描述）转化为结构化、标准化的系统架构文档。它遵循“文档即代码 (Docs as Code)”理念，确保输出的文档具备可维护性、可读性和工程价值。

## 2. 输入参数 (Input Parameters)
Skill 接收以下参数以启动执行流程：

| 参数名 | 类型 | 必填 | 描述 |
| :--- | :--- | :---: | :--- |
| `project_name` | String | 是 | 项目的名称。 |
| `codebase_path` | String | 否 | 本地代码仓库路径或 Git 仓库 URL。用于静态代码分析。 |
| `business_context` | String | 否 | 项目的业务背景、核心目标或需求文档链接。 |
| `target_audience` | String | 否 | 文档的目标读者（如：新入职开发、架构评审委员会），默认为“内部研发团队”。 |
| `output_path` | String | 否 | 生成的文档保存路径，默认为项目根目录下的 `ARCHITECTURE.md`。 |

## 3. 依赖工具 (Required Tools)
本 Skill 在执行过程中需要调用以下外部工具/能力：

1. **`Codebase_Scanner` (代码库扫描器)**: 
   - 功能：遍历 `codebase_path`，识别目录结构、核心依赖文件（如 `pom.xml`, `package.json`, `go.mod`）、Docker/K8s 配置文件，提取技术栈和模块划分。
2. **`Mermaid_Renderer` (图表生成器)**: 
   - 功能：接收结构化的架构描述，生成并校验标准的 Mermaid 语法代码（Context, Container, Component, Sequence diagrams）。
3. **`File_Writer` (文件写入器)**: 
   - 功能：将最终生成的 Markdown 内容持久化写入到指定的 `output_path`。

## 4. 执行工作流 (Execution Workflow)
Skill 被触发后，将严格按照以下步骤（Steps）执行：

### Step 1: 信息收集与解析 (Information Gathering)
- **动作**: 检查输入参数。
- **工具调用**: 若提供 `codebase_path`，调用 `Codebase_Scanner`。
- **处理逻辑**: 
  - 提取技术栈（语言、框架、**具体版本号**）。
  - 识别核心模块（通过顶层目录或构建工具模块划分）。
  - 识别基础设施配置（通过 `docker-compose.yml` 或 CI/CD 脚本提取数据库、中间件信息）。
  - 结合 `business_context` 补充业务语义。

### Step 2: 架构抽象与建模 (Architecture Modeling)
- **动作**: 基于 Step 1 收集的数据，进行架构抽象（LLM 推理）。
- **处理逻辑**:
  - **Level 1 (System Context)**: 定义系统边界，识别外部用户（Actor）和依赖的第三方系统。
  - **Level 2 (Container)**: 将系统拆分为独立的容器（如 Web UI, API Gateway, Backend Service, Database），定义交互协议（REST, gRPC, MQ）。
  - **Level 3 (Component)**: 针对核心 Container，进一步拆分为内部组件（Controller, Service, Repository）。

### Step 3: 可视化图表生成 (Diagram Generation)
- **动作**: 将 Step 2 的抽象模型转化为可视化图表。
- **工具调用**: 调用 `Mermaid_Renderer`。
- **处理逻辑**: 
  - 生成 `C4_Context` 图。
  - 生成 `C4_Container` 图。
  - 生成 1-2 个核心业务的 `Sequence` (时序) 图。
  - 校验 Mermaid 语法，确保无渲染错误。

### Step 4: 文档组装与 ADR 提取 (Document Assembly)
- **动作**: 按照标准模板组装 Markdown 内容。
- **处理逻辑**:
  - 填充概述、技术栈、部署说明等基础章节。
  - 将 Step 3 生成的 Mermaid 代码块嵌入对应章节。
  - **推理生成 ADR**: 基于代码中使用的特殊技术或反直觉的设计，自动推导并生成 1-3 个架构决策记录（ADR），格式严格遵循：`背景` -> `选项` -> `决策` -> `后果`。

### Step 5: 校验与输出 (Validation & Output)
- **动作**: 质量检查并持久化文件。
- **工具调用**: 调用 `File_Writer`。
- **处理逻辑**:
  - 检查文档是否包含所有必填章节。
  - 检查 Mermaid 代码块是否正确闭合。
  - 将内容写入 `output_path`。
  - 返回执行结果摘要。

## 5. 输出规范 (Output Specification)
Skill 执行完毕后，需向调用者（用户或上游 Agent）返回以下结构化 JSON 结果：

```json
{
  "status": "success",
  "message": "架构文档生成完毕",
  "data": {
    "file_path": "/path/to/ARCHITECTURE.md",
    "tech_stack_detected": ["Java 17", "Spring Boot 3.2", "MySQL 8.0", "Redis"],
    "modules_identified": ["user-service", "order-service", "gateway"],
    "diagrams_generated": 4,
    "adr_count": 2
  }
}
```

## 6. 异常处理 (Exception Handling)
- **代码库为空或无法访问**: 降级为纯文本生成模式，仅基于 `business_context` 生成骨架文档，并在文档顶部标注 `[警告: 缺少代码库访问权限，需人工补充代码级细节]`。
- **Mermaid 语法错误**: 捕获渲染异常，触发 LLM 自我修复（Self-Correction）重试一次；若仍失败，则输出纯文本描述替代该图表。
- **文件写入权限不足**: 若 `File_Writer` 写入失败，将完整的 Markdown 内容作为文本结果直接返回给前端/调用方展示。