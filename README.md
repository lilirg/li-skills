# li-skills

个人 AI 编程助手 Skills 存储库，收录了一系列用于提升开发效率与设计质量的技能模块。每个 Skill 以 [`SKILL.md`](SKILLS/common/brainstorming/SKILL.md) 为核心定义文件，包含使用场景、工作流程、最佳实践及参考资源。

## 目录结构

```
SKILLS/
├── common/                          # 通用技能
│   └── brainstorming/               # 头脑风暴与设计规划
├── design/                          # 设计类技能
│   ├── adobe-xd/                    # Adobe XD 设计与原型
│   ├── algorithmic-art/             # p5.js 生成式算法艺术
│   ├── animation-vocabulary/        # 动画术语反向查询
│   ├── apple-design/                # Apple 设计理念（Web 实现）
│   ├── brand-guidelines/            # 品牌视觉规范
│   ├── canvas-design/               # 画布级静态视觉设计
│   ├── emil-design-eng/             # Emil Kowalski 设计工程哲学
│   ├── find-animation-opportunities/# 发现动画机会
│   ├── improve-animations/          # 动画改进审计与计划
│   ├── pick-ui-library/             # UI 库选择指南
│   └── review-animations/           # 动画代码审查
├── document/                        # 文档类技能
│   └── architecture-document-generator/  # 架构文档生成器（C4 模型）
├── web-frontEnd/                    # 前端开发技能
│   ├── tailwindcss/                 # Tailwind CSS v4 实用指南
│   ├── ui-ux-pro-max/               # UI/UX 设计智能引擎
│   ├── vue-best-practices/          # Vue 3 最佳实践（Composition API）
│   ├── vue-jsx-best-practices/      # Vue JSX 最佳实践
│   ├── vue-options-api-best-practices/   # Vue Options API 最佳实践
│   ├── vue-pinia-best-practices/    # Pinia 状态管理最佳实践
│   └── vue-router-best-practices/   # Vue Router 最佳实践
└── Project-SKILLS/                  # 项目级技能
    └── copaw-build/                 # CoPaw (VJSP-Claw) Python 项目构建
```

## Skills 概览

### 通用技能（common）

#### Brainstorming — 头脑风暴与设计规划

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/common/brainstorming/`](SKILLS/common/brainstorming/SKILL.md) |
| 用途 | 在任何创造性工作开始前，通过协作对话将想法转化为完整的设计方案与规格文档 |
| 核心流程 | 探索项目上下文 → 提出澄清问题 → 提出 2-3 种方案 → 呈现设计 → 撰写设计文档 → 规格审查循环 → 转入实现计划 |
| 亮点 | 内置可视化伴侣（浏览器端 Mockup 展示）、规格审查子代理、严格的设计审批门控 |

### 设计技能（design）

#### Adobe XD — 设计与原型

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/adobe-xd/`](SKILLS/design/adobe-xd/SKILL.md) |
| 用途 | 在 Adobe XD 中创建 UI/UX 设计、交互原型、可复用组件，以及开发者交付 |
| 核心功能 | 画板创建、组件状态、重复网格、原型交互（Tap/Drag/Voice + Transition/Auto-Animate）、开发者共享链接 |
| 注意 | Adobe 已弃用 XD，新项目建议评估 Figma |

#### Algorithmic Art — p5.js 生成式算法艺术

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/algorithmic-art/`](SKILLS/design/algorithmic-art/SKILL.md) |
| 用途 | 使用 p5.js 创建画廊级生成式艺术，输出自包含 HTML 交互式作品 |
| 核心流程 | 创建算法哲学宣言 → 推导概念种子 → 基于 [`templates/viewer.html`](SKILLS/design/algorithmic-art/templates/viewer.html) 模板实现 p5.js 算法 |
| 特性 | 种子随机性（Art Blocks 模式）、参数化控制、种子导航、实时交互、单文件自包含输出 |

#### Animation Vocabulary — 动画术语反向查询

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/animation-vocabulary/`](SKILLS/design/animation-vocabulary/SKILL.md) |
| 用途 | 将模糊的动画效果描述反向查询为精确的术语名称（如"弹出时弹跳的东西"→ Pop in） |
| 覆盖范围 | 入场/出场、序列与时间、移动与变换、状态过渡、滚动、反馈与交互、缓动、弹簧动画、循环与氛围、润色与效果、性能、原则 |
| 特性 | 只读查询，不涉及实现；支持近义术语辨析 |

#### Apple Design — Apple 设计理念（Web 实现）

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/apple-design/`](SKILLS/design/apple-design/SKILL.md) |
| 用途 | 将 Apple 的界面设计理念（WWDC 2018 等）转化为 Web 平台实现指南 |
| 核心原则 | 响应延迟消除、直接操控（1:1 跟踪）、可中断性、行为优先于动画（弹簧）、速度交接、动量投影、空间一致性、手势方向提示、橡皮筋效果、帧级流畅、材质与深度、多模态反馈、无障碍、排版 |
| 技术映射 | CSS、Pointer Events、`requestAnimationFrame`、Motion/Framer Motion 等弹簧库 |

#### Brand Guidelines — 品牌视觉规范

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/brand-guidelines/`](SKILLS/design/brand-guidelines/SKILL.md) |
| 用途 | 将品牌色彩与排版应用于演示文稿、文档、视觉作品等产出物 |
| 品牌色 | Dark `#141413`、Light `#faf9f5`、Orange `#d97757`、Blue `#6a9bcc`、Green `#788c5d` |
| 字体 | 标题 Poppins（回退 Arial）、正文 Lora（回退 Georgia） |

#### Canvas Design — 画布级静态视觉设计

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/canvas-design/`](SKILLS/design/canvas-design/SKILL.md) |
| 用途 | 创建博物馆/杂志级静态视觉作品，输出 .pdf 或 .png |
| 核心流程 | 创建视觉哲学宣言 → 推导微妙概念引用 → 在画布上以构图、色彩、排版表达 |
| 特性 | 内置 30+ 种 Canvas 字体（位于 [`canvas-fonts/`](SKILLS/design/canvas-design/canvas-fonts/) 目录）、极简文字、设计驱动构图、多页扩展支持 |

#### Emil Design Engineering — Emil Kowalski 设计工程哲学

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/emil-design-eng/`](SKILLS/design/emil-design-eng/SKILL.md) |
| 用途 | 编码 Emil Kowalski 关于 UI 润色、组件设计、动画决策和隐形细节的完整哲学 |
| 核心框架 | 动画决策框架（是否动画 → 目的 → 缓动 → 速度）、弹簧动画、组件构建原则、CSS Transform 精通、`clip-path` 动画、手势与拖拽交互、性能规则、无障碍、Sonner 组件原则 |
| 亮点 | 内置审查格式（Before/After 表格）、完整的缓动曲线和时长预算表、`@starting-style` 入口动画 |

#### Find Animation Opportunities — 发现动画机会

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/find-animation-opportunities/`](SKILLS/design/find-animation-opportunities/SKILL.md) |
| 用途 | 扫描代码库或 UI 中应该添加动画但尚未添加的位置，同时严格过滤不应动画的场景 |
| 核心原则 | 克制优先——基于频率、目的、速度、功能四道门控过滤 |
| 输出 | 按杠杆排序的机会表格 + 被拒绝的候选列表 + 总体评估 |
| 特性 | 只读分析，不修改代码；最多 5-7 条建议 |

#### Improve Animations — 动画改进审计与计划

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/improve-animations/`](SKILLS/design/improve-animations/SKILL.md) |
| 用途 | 作为高级动效顾问审计代码库的动画代码，生成优先级排序的审计结果和自包含实现计划 |
| 审计维度 | 目的与频率、缓动与时长、物理性与原点、可中断性、性能、无障碍、一致性与令牌、遗漏机会 |
| 输出 | 审计发现表格 + 自包含实现计划（写入 `plans/` 目录） |
| 参考文件 | [`AUDIT.md`](SKILLS/design/improve-animations/AUDIT.md)（审计规则）、[`PLAN-TEMPLATE.md`](SKILLS/design/improve-animations/PLAN-TEMPLATE.md)（计划模板） |

#### Pick UI Library — UI 库选择指南

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/pick-ui-library/`](SKILLS/design/pick-ui-library/SKILL.md) |
| 用途 | 为前端任务从精选列表中推荐合适的 UI 库 |
| 覆盖范围 | UI 组件与基元（base-ui、cmdk、Sonner、input-otp）、动效与视觉（Motion、NumberFlow、Cobe、Satori）、图表（Liveline、recharts）、交互与性能（dnd kit、Virtuoso）、状态与样式（zustand、clsx、cva、next-themes） |
| 特性 | 基于品味的精选推荐，非穷举列表；自动检查 `package.json` 已有依赖 |

#### Review Animations — 动画代码审查

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/design/review-animations/`](SKILLS/design/review-animations/SKILL.md) |
| 用途 | 以高标准审查动画和动效代码，默认倾向标记问题，批准需经严格验证 |
| 十大标准 | 合理动效、频率适配、响应式缓动、300ms 内、原点与物理正确、可中断性、仅 GPU 属性、无障碍、非对称进出、一致性 |
| 输出 | 发现表格（Before/After/Why）+ 按影响分组的评估 + 明确决策（Block/Approve） |
| 参考文件 | [`STANDARDS.md`](SKILLS/design/review-animations/STANDARDS.md)（完整规则目录） |

### 文档技能（document）

#### Architecture Document Generator — 架构文档生成器

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/document/architecture-document-generator/`](SKILLS/document/architecture-document-generator/SKILL.md) |
| 版本 | v1.0.0 |
| 用途 | 分析项目代码库和业务上下文，自动提取系统架构信息，生成符合 C4 模型标准的项目架构文档（`ARCHITECTURE.md`） |
| 核心流程 | 信息收集与解析（代码库扫描） → 架构抽象与建模（System Context / Container / Component） → 可视化图表生成（Mermaid） → 文档组装与 ADR 提取 → 校验与输出 |
| 输出 | 包含 C4 上下文图、容器图、组件图、时序图及 1-3 条架构决策记录（ADR）的标准化 Markdown 文档 |
| 异常处理 | 代码库不可访问时降级为纯文本骨架模式；Mermaid 语法错误自动修复重试 |

### 前端开发技能（web-frontEnd）

#### Tailwind CSS — 实用优先 CSS 框架

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/tailwindcss/`](SKILLS/web-frontEnd/tailwindcss/SKILL.md) |
| 版本 | v4.1.18（2026-01-28 生成） |
| 用途 | 使用 Tailwind CSS 进行 Web 应用样式开发、响应式设计、设计系统定制 |
| 覆盖范围 | 安装配置、实用类、主题变量、响应式设计、变体、布局（Flexbox/Grid/定位/尺寸/间距）、变换、排版、视觉效果、过渡动画、暗色模式、v3→v4 迁移 |
| 参考文档 | 40+ 篇参考文档位于 [`references/`](SKILLS/web-frontEnd/tailwindcss/references/) 目录 |

#### UI/UX Pro Max — UI/UX 设计智能引擎

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/ui-ux-pro-max/`](SKILLS/web-frontEnd/ui-ux-pro-max/SKILL.md) |
| 用途 | 全栈 UI/UX 设计指导，覆盖 50+ 风格、97 套配色、57 组字体搭配、99 条 UX 准则、25 种图表类型 |
| 支持技术栈 | React, Next.js, Vue, Svelte, SwiftUI, React Native, Flutter, Tailwind, shadcn/ui, Jetpack Compose |
| 核心功能 | 通过 Python CLI 工具搜索设计系统推荐（`--design-system`）、按域查询（style/color/typography/chart/ux/landing）、技术栈最佳实践、设计系统持久化（Master + 页面覆盖模式） |
| 交付前检查 | 内置视觉质量、交互、明暗模式、布局、无障碍五维检查清单 |

#### Vue Best Practices — Vue 3 最佳实践（Composition API）

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/vue-best-practices/`](SKILLS/web-frontEnd/vue-best-practices/SKILL.md) |
| 版本 | v18.0.0 |
| 用途 | Vue.js 开发全流程最佳实践，默认采用 Composition API + `<script setup lang="ts">` |
| 核心原则 | 状态可预测、数据流显式化、组件小而聚焦、避免不必要重渲染、可读性优先 |
| 覆盖范围 | 响应式、SFC 结构、组件数据流、Composables、Slots、透传属性、KeepAlive、Teleport、Suspense、动画、指令、异步组件、渲染函数、插件、状态管理、性能优化 |
| 参考文档 | 20+ 篇参考文档位于 [`references/`](SKILLS/web-frontEnd/vue-best-practices/references/) 目录，10+ 条规则位于 [`rules/`](SKILLS/web-frontEnd/vue-best-practices/rules/) 目录 |

#### Vue JSX Best Practices — Vue JSX 最佳实践

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/vue-jsx-best-practices/`](SKILLS/web-frontEnd/vue-jsx-best-practices/SKILL.md) |
| 版本 | v2.0.0 |
| 用途 | Vue 中 JSX 语法的最佳实践，涵盖 `class` vs `className`、JSX 插件配置等 |
| 参考 | [`render-function-jsx-vue-vs-react`](SKILLS/web-frontEnd/vue-jsx-best-practices/reference/render-function-jsx-vue-vs-react.md) |

#### Vue Options API Best Practices — Vue Options API 最佳实践

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/vue-options-api-best-practices/`](SKILLS/web-frontEnd/vue-options-api-best-practices/SKILL.md) |
| 版本 | v2.0.0 |
| 用途 | Vue 3 Options API 风格的最佳实践，TypeScript 集成与常见陷阱 |
| 覆盖范围 | TypeScript 类型推断、`this` 上下文类型安全、Props 类型、Provide/Inject 类型、Computed 返回类型、方法绑定、生命周期钩子 |

#### Vue Pinia Best Practices — Pinia 状态管理最佳实践

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/web-frontEnd/vue-pinia-best-practices/`](SKILLS/web-frontEnd/vue-pinia-best-practices/SKILL.md) |
| 版本 | v1.0.0 |
| 用途 | Pinia 状态管理的最佳实践、常见陷阱与模式 |
| 覆盖范围 | Store 设置（`getActivePinia` 错误、Setup Store 状态）、响应式（解构破坏响应性、方法绑定）、状态模式（URL 过滤器、大型应用状态管理） |

### 项目级技能（Project-SKILLS）

#### CoPaw Build — CoPaw 项目构建

| 属性 | 值 |
|------|-----|
| 路径 | [`Project-SKILLS/copaw-build/`](Project-SKILLS/copaw-build/SKILL.md) |
| 用途 | CoPaw (VJSP-Claw) Python 项目的 PyInstaller 构建技能，涵盖虚拟环境激活、打包、构建产物复制到 VJSP 客户端等完整流程 |
| 构建步骤 | 激活虚拟环境 → 执行 `pyinstaller copaw.spec --clean --noconfirm` → 运行 [`copy-copaw-build.ps1`](Project-SKILLS/copaw-build/SKILL.md) 复制产物到 `apps/web/copaw-dist/` |
| 产物 | `VJSP-Claw.exe` 独立可执行文件，集成前端控制台、Agent 配置、分词器、安全规则等资源 |
| 依赖 | Python 3.10+、PyInstaller、前端控制台已构建（`console/dist/`）、VJSPEasySDK-Python 已安装 |

## 许可证

各 Skill 的许可证信息见各自目录下的 `LICENSE.txt` 文件（如适用）。
