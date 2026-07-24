# li-skills

个人 AI 编程助手 Skills 存储库，收录了一系列用于提升开发效率与设计质量的技能模块。每个 Skill 以 [`SKILL.md`](SKILLS/common/brainstorming/SKILL.md) 为核心定义文件，包含使用场景、工作流程、最佳实践及参考资源。

## 目录

- [li-skills](#li-skills)
  - [目录](#目录)
  - [目录结构](#目录结构)
  - [Skills 概览](#skills-概览)
    - [通用技能（common）](#通用技能common)
      - [Brainstorming — 头脑风暴与设计规划](#brainstorming--头脑风暴与设计规划)
    - [设计技能（design）](#设计技能design)
      - [Adobe XD — 设计与原型](#adobe-xd--设计与原型)
      - [Algorithmic Art — p5.js 生成式算法艺术](#algorithmic-art--p5js-生成式算法艺术)
      - [Animation Vocabulary — 动画术语反向查询](#animation-vocabulary--动画术语反向查询)
      - [Apple Design — Apple 设计理念（Web 实现）](#apple-design--apple-设计理念web-实现)
      - [Brand Guidelines — 品牌视觉规范](#brand-guidelines--品牌视觉规范)
      - [Canvas Design — 画布级静态视觉设计](#canvas-design--画布级静态视觉设计)
      - [Emil Design Engineering — Emil Kowalski 设计工程哲学](#emil-design-engineering--emil-kowalski-设计工程哲学)
      - [Find Animation Opportunities — 发现动画机会](#find-animation-opportunities--发现动画机会)
      - [Improve Animations — 动画改进审计与计划](#improve-animations--动画改进审计与计划)
      - [Pick UI Library — UI 库选择指南](#pick-ui-library--ui-库选择指南)
      - [Review Animations — 动画代码审查](#review-animations--动画代码审查)
    - [文档技能（document）](#文档技能document)
      - [Architecture Document Generator — 架构文档生成器](#architecture-document-generator--架构文档生成器)
    - [前端开发技能（web-frontEnd）](#前端开发技能web-frontend)
      - [Tailwind CSS — 实用优先 CSS 框架](#tailwind-css--实用优先-css-框架)
      - [UI/UX Pro Max — UI/UX 设计智能引擎](#uiux-pro-max--uiux-设计智能引擎)
      - [Vue Best Practices — Vue 3 最佳实践（Composition API）](#vue-best-practices--vue-3-最佳实践composition-api)
      - [Vue JSX Best Practices — Vue JSX 最佳实践](#vue-jsx-best-practices--vue-jsx-最佳实践)
      - [Vue Options API Best Practices — Vue Options API 最佳实践](#vue-options-api-best-practices--vue-options-api-最佳实践)
      - [Vue Pinia Best Practices — Pinia 状态管理最佳实践](#vue-pinia-best-practices--pinia-状态管理最佳实践)
    - [工程技能（engineering）](#工程技能engineering)
      - [Ask Matt — 技能路由器](#ask-matt--技能路由器)
      - [Code Review — 双轴代码审查](#code-review--双轴代码审查)
      - [Codebase Design — 深模块设计词汇](#codebase-design--深模块设计词汇)
      - [Diagnosing Bugs — 硬 Bug 诊断循环](#diagnosing-bugs--硬-bug-诊断循环)
      - [Domain Modeling — 领域模型构建与锐化](#domain-modeling--领域模型构建与锐化)
      - [Grill with Docs — 带文档的拷问式访谈](#grill-with-docs--带文档的拷问式访谈)
      - [Implement — 基于规格的实现](#implement--基于规格的实现)
      - [Improve Codebase Architecture — 代码库架构改进](#improve-codebase-architecture--代码库架构改进)
      - [Prototype — 一次性原型构建](#prototype--一次性原型构建)
      - [Research — 背景代理研究](#research--背景代理研究)
      - [Resolving Merge Conflicts — 合并冲突解决](#resolving-merge-conflicts--合并冲突解决)
      - [Setup Matt Pocock Skills — 工程技能配置](#setup-matt-pocock-skills--工程技能配置)
      - [TDD — 测试驱动开发](#tdd--测试驱动开发)
      - [To Spec — 对话转规格](#to-spec--对话转规格)
      - [To Tickets — 拆分为追踪弹工单](#to-tickets--拆分为追踪弹工单)
      - [Triage — 工单分类状态机](#triage--工单分类状态机)
      - [Wayfinder — 大型工作规划地图](#wayfinder--大型工作规划地图)
    - [生产力技能（productivity）](#生产力技能productivity)
      - [Grill Me — 无代码库的拷问式访谈](#grill-me--无代码库的拷问式访谈)
      - [Grilling — 拷问式访谈原语](#grilling--拷问式访谈原语)
      - [Handoff — 对话交接文档](#handoff--对话交接文档)
      - [Teach — 多会话教学](#teach--多会话教学)
      - [Writing Great Skills — 技能编写参考](#writing-great-skills--技能编写参考)
    - [杂项技能（misc）](#杂项技能misc)
      - [Git Guardrails — Git 安全钩子](#git-guardrails--git-安全钩子)
      - [Migrate to Shoehorn — 迁移到 Shoehorn](#migrate-to-shoehorn--迁移到-shoehorn)
      - [Scaffold Exercises — 练习目录脚手架](#scaffold-exercises--练习目录脚手架)
      - [Setup Pre-commit — 预提交钩子设置](#setup-pre-commit--预提交钩子设置)
    - [个人技能（personal）](#个人技能personal)
      - [Edit Article — 文章编辑与改进](#edit-article--文章编辑与改进)
      - [Obsidian Vault — Obsidian 笔记管理](#obsidian-vault--obsidian-笔记管理)
    - [写作技能（writing）](#写作技能writing)
      - [Writing Beats — 节拍式写作](#writing-beats--节拍式写作)
      - [Writing Fragments — 碎片式写作](#writing-fragments--碎片式写作)
      - [Writing Shape — 文章塑形](#writing-shape--文章塑形)
    - [项目级技能（Project-SKILLS）](#项目级技能project-skills)
      - [CoPaw Build — CoPaw 项目构建](#copaw-build--copaw-项目构建)
  - [许可证](#许可证)

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
├── engineering/                     # 工程技能
│   ├── ask-matt/                    # 技能路由器
│   ├── code-review/                 # 双轴代码审查（Standards + Spec）
│   ├── codebase-design/             # 深模块设计词汇
│   ├── diagnosing-bugs/             # 硬 Bug 诊断循环
│   ├── domain-modeling/             # 领域模型构建与锐化
│   ├── grill-with-docs/             # 带文档的拷问式访谈
│   ├── implement/                   # 基于规格的实现
│   ├── improve-codebase-architecture/  # 代码库架构改进
│   ├── prototype/                   # 一次性原型构建
│   ├── research/                    # 背景代理研究
│   ├── resolving-merge-conflicts/   # 合并冲突解决
│   ├── setup-matt-pocock-skills/    # 工程技能配置
│   ├── tdd/                         # 测试驱动开发
│   ├── to-spec/                     # 对话转规格
│   ├── to-tickets/                  # 拆分为追踪弹工单
│   ├── triage/                      # 工单分类状态机
│   └── wayfinder/                   # 大型工作规划地图
├── misc/                            # 杂项技能
│   ├── git-guardrails-claude-code/  # Git 安全钩子
│   ├── migrate-to-shoehorn/         # 迁移到 Shoehorn
│   ├── scaffold-exercises/          # 练习目录脚手架
│   └── setup-pre-commit/            # 预提交钩子设置
├── personal/                        # 个人技能
│   ├── edit-article/                # 文章编辑与改进
│   └── obsidian-vault/              # Obsidian 笔记管理
├── productivity/                    # 生产力技能
│   ├── grill-me/                    # 无代码库的拷问式访谈
│   ├── grilling/                    # 拷问式访谈原语
│   ├── handoff/                     # 对话交接文档
│   ├── teach/                       # 多会话教学
│   └── writing-great-skills/        # 技能编写参考
├── web-frontEnd/                    # 前端开发技能
│   ├── tailwindcss/                 # Tailwind CSS v4 实用指南
│   ├── ui-ux-pro-max/               # UI/UX 设计智能引擎
│   ├── vue-best-practices/          # Vue 3 最佳实践（Composition API）
│   ├── vue-jsx-best-practices/      # Vue JSX 最佳实践
│   ├── vue-options-api-best-practices/   # Vue Options API 最佳实践
│   ├── vue-pinia-best-practices/    # Pinia 状态管理最佳实践
│   └── vue-router-best-practices/   # Vue Router 最佳实践
├── writing/                         # 写作技能
│   ├── writing-beats/               # 节拍式写作
│   ├── writing-fragments/           # 碎片式写作
│   └── writing-shape/               # 文章塑形
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

### 工程技能（engineering）

> 来源：Matt Pocock 的工程技能集。使用前需运行 [`/setup-matt-pocock-skills`](SKILLS/engineering/setup-matt-pocock-skills/SKILL.md) 配置 Issue 追踪器、分类标签和领域文档布局。

#### Ask Matt — 技能路由器

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/ask-matt/`](SKILLS/engineering/ask-matt/SKILL.md) |
| 用途 | 技能路由器，帮助选择当前场景适合的技能或流程 |
| 核心流程 | 主流程（idea → ship）：`/grill-with-docs` → `/to-spec` → `/to-tickets` → `/implement`（内部驱动 `/tdd`，结束时 `/code-review`） |
| 入口 | Bug 堆积 → `/triage`；东西坏了 → `/diagnosing-bugs`；大型模糊任务 → `/wayfinder` |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Code Review — 双轴代码审查

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/code-review/`](SKILLS/engineering/code-review/SKILL.md) |
| 用途 | 对比固定点（commit/branch/tag）以来的变更，沿两个轴审查：Standards（编码规范 + Fowler 代码异味基线）和 Spec（是否忠实实现原始 issue/PRD） |
| 核心流程 | 确定固定点 → 识别规格来源 → 识别标准来源 → 并行子代理审查 → 聚合报告 |
| 输出 | Standards 和 Spec 两个独立报告，不合并或重排序发现 |
| 调用方式 | 模型调用 |

#### Codebase Design — 深模块设计词汇

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/codebase-design/`](SKILLS/engineering/codebase-design/SKILL.md) |
| 用途 | 设计深模块的共享词汇表：小接口、清晰接缝、通过接口可测试 |
| 核心概念 | Module、Interface、Implementation、Depth、Seam、Adapter、Leverage、Locality |
| 原则 | 深度是接口属性而非实现属性；删除测试；接口即测试面；一个适配器=假设接缝，两个=真实接缝 |
| 参考文件 | [`DEEPENING.md`](SKILLS/engineering/codebase-design/DEEPENING.md)、[`DESIGN-IT-TWICE.md`](SKILLS/engineering/codebase-design/DESIGN-IT-TWICE.md) |
| 调用方式 | 模型调用 |

#### Diagnosing Bugs — 硬 Bug 诊断循环

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/diagnosing-bugs/`](SKILLS/engineering/diagnosing-bugs/SKILL.md) |
| 用途 | 硬 Bug 和性能回归的纪律性诊断循环 |
| 六阶段 | 构建反馈循环 → 复现+最小化 → 假设（3-5 个排序假设） → 仪表化 → 修复+回归测试 → 清理+事后分析 |
| 核心原则 | 反馈循环是核心——没有红色命令不进入假设阶段；一次只改一个变量；调试日志加唯一前缀标签 |
| 调用方式 | 模型调用 |

#### Domain Modeling — 领域模型构建与锐化

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/domain-modeling/`](SKILLS/engineering/domain-modeling/SKILL.md) |
| 用途 | 主动构建和锐化项目的领域模型——挑战术语、用场景压力测试、内联更新 `CONTEXT.md` 和 ADR |
| 核心活动 | 对照术语表挑战、锐化模糊语言、讨论具体场景、与代码交叉引用、内联更新 `CONTEXT.md`、谨慎提供 ADR |
| 参考文件 | [`CONTEXT-FORMAT.md`](SKILLS/engineering/domain-modeling/CONTEXT-FORMAT.md)、[`ADR-FORMAT.md`](SKILLS/engineering/domain-modeling/ADR-FORMAT.md) |
| 调用方式 | 模型调用 |

#### Grill with Docs — 带文档的拷问式访谈

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/grill-with-docs/`](SKILLS/engineering/grill-with-docs/SKILL.md) |
| 用途 | 运行 `/grilling` 会话，同时使用 `/domain-modeling` 技能，在拷问过程中创建 ADR 和术语表 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Implement — 基于规格的实现

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/implement/`](SKILLS/engineering/implement/SKILL.md) |
| 用途 | 基于规格或工单实现工作，内部驱动 `/tdd`，完成后运行 `/code-review` |
| 核心流程 | 使用 `/tdd` 在预定的接缝处 → 定期类型检查 → 单文件测试 → 最终全量测试 → `/code-review` → 提交 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Improve Codebase Architecture — 代码库架构改进

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/improve-codebase-architecture/`](SKILLS/engineering/improve-codebase-architecture/SKILL.md) |
| 用途 | 扫描代码库寻找深化机会，以可视化 HTML 报告呈现，然后拷问选定的一个 |
| 核心流程 | 探索代码库（寻找浅模块、耦合、测试困难处） → 生成 HTML 报告（Tailwind + Mermaid） → 拷问循环设计深化模块 |
| 输出 | 自包含 HTML 报告（写入系统临时目录），每个候选含 Files/Problem/Solution/Benefits/Before-After 图/推荐强度 |
| 参考文件 | [`HTML-REPORT.md`](SKILLS/engineering/improve-codebase-architecture/HTML-REPORT.md) |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Prototype — 一次性原型构建

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/prototype/`](SKILLS/engineering/prototype/SKILL.md) |
| 用途 | 构建一次性原型回答设计问题：逻辑/状态模型的终端应用，或多个可切换 UI 变体 |
| 分支 | 逻辑分支（[`LOGIC.md`](SKILLS/engineering/prototype/LOGIC.md)）→ 交互式终端应用；UI 分支（[`UI.md`](SKILLS/engineering/prototype/UI.md)）→ 可切换 UI 变体 |
| 规则 | 从第一天起就是一次性的、一条命令运行、默认无持久化、跳过打磨、暴露状态、完成后删除或吸收 |
| 调用方式 | 模型调用 |

#### Research — 背景代理研究

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/research/`](SKILLS/engineering/research/SKILL.md) |
| 用途 | 启动背景代理针对高信任原始来源调查问题，将发现写入 Markdown 文件 |
| 核心流程 | 针对原始来源（官方文档、源码、规范、第一方 API）调查 → 撰写带引用的 Markdown 文件 → 保存到仓库约定位置 |
| 调用方式 | 模型调用 |

#### Resolving Merge Conflicts — 合并冲突解决

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/resolving-merge-conflicts/`](SKILLS/engineering/resolving-merge-conflicts/SKILL.md) |
| 用途 | 解决进行中的 git merge/rebase 冲突 |
| 流程 | 查看当前状态 → 查找每个冲突的原始来源 → 逐 hunk 解决（保留双方意图） → 运行自动化检查 → 完成合并/rebase |
| 调用方式 | 模型调用 |

#### Setup Matt Pocock Skills — 工程技能配置

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/setup-matt-pocock-skills/`](SKILLS/engineering/setup-matt-pocock-skills/SKILL.md) |
| 用途 | 为工程技能配置每仓库的基础设施：Issue 追踪器、分类标签词汇、领域文档布局 |
| 配置项 | Issue 追踪器（GitHub/GitLab/本地 Markdown/其他）、分类标签（5 个规范角色）、领域文档（单上下文/多上下文） |
| 参考文件 | [`issue-tracker-github.md`](SKILLS/engineering/setup-matt-pocock-skills/issue-tracker-github.md)、[`issue-tracker-gitlab.md`](SKILLS/engineering/setup-matt-pocock-skills/issue-tracker-gitlab.md)、[`issue-tracker-local.md`](SKILLS/engineering/setup-matt-pocock-skills/issue-tracker-local.md)、[`triage-labels.md`](SKILLS/engineering/setup-matt-pocock-skills/triage-labels.md)、[`domain.md`](SKILLS/engineering/setup-matt-pocock-skills/domain.md) |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### TDD — 测试驱动开发

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/tdd/`](SKILLS/engineering/tdd/SKILL.md) |
| 用途 | 红 → 绿循环的测试驱动开发，一次一个垂直切片 |
| 核心原则 | 测试验证公共接口行为而非实现细节；只在预定接缝测试；一次一个切片 |
| 反模式 | 实现耦合测试、同义反复测试、水平切片 |
| 参考文件 | [`tests.md`](SKILLS/engineering/tdd/tests.md)、[`mocking.md`](SKILLS/engineering/tdd/mocking.md) |
| 调用方式 | 模型调用 |

#### To Spec — 对话转规格

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/to-spec/`](SKILLS/engineering/to-spec/SKILL.md) |
| 用途 | 将当前对话上下文合成为规格（PRD）并发布到 Issue 追踪器，不访谈用户 |
| 输出模板 | Problem Statement、Solution、User Stories、Implementation Decisions、Testing Decisions、Out of Scope、Further Notes |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### To Tickets — 拆分为追踪弹工单

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/to-tickets/`](SKILLS/engineering/to-tickets/SKILL.md) |
| 用途 | 将计划/规格/对话拆分为追踪弹工单集，每个工单声明其阻塞边 |
| 核心流程 | 收集上下文 → 探索代码库 → 起草垂直切片 → 向用户确认 → 发布到追踪器 |
| 规则 | 每个切片切穿所有层（schema/API/UI/tests）；宽重构例外使用 expand-contract 序列 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Triage — 工单分类状态机

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/triage/`](SKILLS/engineering/triage/SKILL.md) |
| 用途 | 将 Issue 和外部 PR 通过分类角色状态机移动——分类、验证、必要时拷问、撰写代理就绪简报 |
| 角色 | 分类：`bug`/`enhancement`；状态：`needs-triage`/`needs-info`/`ready-for-agent`/`ready-for-human`/`wontfix` |
| 参考文件 | [`AGENT-BRIEF.md`](SKILLS/engineering/triage/AGENT-BRIEF.md)、[`OUT-OF-SCOPE.md`](SKILLS/engineering/triage/OUT-OF-SCOPE.md) |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Wayfinder — 大型工作规划地图

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/engineering/wayfinder/`](SKILLS/engineering/wayfinder/SKILL.md) |
| 用途 | 为超出单个代理会话容量的大型工作规划——在 Issue 追踪器上绘制共享调查工单地图，逐一解决直到路径清晰 |
| 核心概念 | 地图（索引 Issue）、工单（子 Issue）、战争之雾（尚未可指定的决策）、范围外、前沿 |
| 工单类型 | Research（AFK）、Prototype（HITL）、Grilling（HITL）、Task（HITL/AFK） |
| 原则 | 规划而非执行；每次会话最多解决一个工单；按名称引用而非编号 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

### 生产力技能（productivity）

> 通用工作流工具，不限于代码。

#### Grill Me — 无代码库的拷问式访谈

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/productivity/grill-me/`](SKILLS/productivity/grill-me/SKILL.md) |
| 用途 | 无代码库场景下的拷问式访谈，无状态——不保存任何本地文件 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Grilling — 拷问式访谈原语

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/productivity/grilling/`](SKILLS/productivity/grilling/SKILL.md) |
| 用途 | 对计划的每个方面进行无情访谈，逐个解决决策树分支，每个问题附带推荐答案 |
| 核心规则 | 一次只问一个问题；事实查代码库而非问用户；决策归用户；确认共享理解后才执行 |
| 调用方式 | 模型调用 |

#### Handoff — 对话交接文档

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/productivity/handoff/`](SKILLS/productivity/handoff/SKILL.md) |
| 用途 | 将当前对话压缩为交接文档，供新代理继续工作 |
| 规则 | 保存到系统临时目录；包含建议技能部分；不重复已有工件；脱敏敏感信息 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Teach — 多会话教学

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/productivity/teach/`](SKILLS/productivity/teach/SKILL.md) |
| 用途 | 在多个会话中教授用户新技能或概念，使用当前目录作为有状态教学工作区 |
| 工作区 | `MISSION.md`（学习动机）、`reference/*.html`（参考材料）、`RESOURCES.md`（资源列表）、`learning-records/*.md`（学习记录）、`lessons/*.html`（课程）、`assets/*`（可复用组件）、`NOTES.md`（笔记） |
| 理念 | 知识（高质量资源）+ 技能（交互式课程）+ 智慧（社区互动）；流利度 vs 存储强度；最近发展区 |
| 参考文件 | [`MISSION-FORMAT.md`](SKILLS/productivity/teach/MISSION-FORMAT.md)、[`RESOURCES-FORMAT.md`](SKILLS/productivity/teach/RESOURCES-FORMAT.md)、[`LEARNING-RECORD-FORMAT.md`](SKILLS/productivity/teach/LEARNING-RECORD-FORMAT.md)、[`GLOSSARY-FORMAT.md`](SKILLS/productivity/teach/GLOSSARY-FORMAT.md) |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Writing Great Skills — 技能编写参考

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/productivity/writing-great-skills/`](SKILLS/productivity/writing-great-skills/SKILL.md) |
| 用途 | 编写和编辑技能的参考——使技能可预测的词汇和原则 |
| 核心概念 | 可预测性（核心美德）、调用方式（模型 vs 用户）、信息层级（步骤 → 技能内参考 → 外部参考）、渐进式披露、粒度、修剪、引导词 |
| 失败模式 | 过早完成、重复、沉积、蔓延、空操作、否定 |
| 参考文件 | [`GLOSSARY.md`](SKILLS/productivity/writing-great-skills/GLOSSARY.md) |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

### 杂项技能（misc）

> 保留但不常使用的工具，未在插件中推广。

#### Git Guardrails — Git 安全钩子

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/misc/git-guardrails-claude-code/`](SKILLS/misc/git-guardrails-claude-code/SKILL.md) |
| 用途 | 设置 Claude Code 钩子，在执行前阻止危险 git 命令（push、reset --hard、clean、branch -D 等） |
| 阻止列表 | `git push`（含 --force）、`git reset --hard`、`git clean -f`/`-fd`、`git branch -D`、`git checkout .`/`git restore .` |
| 脚本 | [`scripts/block-dangerous-git.sh`](SKILLS/misc/git-guardrails-claude-code/scripts/block-dangerous-git.sh) |
| 调用方式 | 模型调用 |

#### Migrate to Shoehorn — 迁移到 Shoehorn

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/misc/migrate-to-shoehorn/`](SKILLS/misc/migrate-to-shoehorn/SKILL.md) |
| 用途 | 将测试文件从 `as` 类型断言迁移到 @total-typescript/shoehorn |
| 迁移模式 | `as Type` → `fromPartial()`；`as unknown as Type` → `fromAny()` |
| 注意 | 仅限测试代码，不用于生产代码 |
| 调用方式 | 模型调用 |

#### Scaffold Exercises — 练习目录脚手架

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/misc/scaffold-exercises/`](SKILLS/misc/scaffold-exercises/SKILL.md) |
| 用途 | 创建练习目录结构，包含章节、问题、解决方案和解释器，通过 lint 检查 |
| 命名规范 | 章节：`XX-section-name/`；练习：`XX.YY-exercise-name/`；变体：`problem/`/`solution/`/`explainer/` |
| 调用方式 | 模型调用 |

#### Setup Pre-commit — 预提交钩子设置

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/misc/setup-pre-commit/`](SKILLS/misc/setup-pre-commit/SKILL.md) |
| 用途 | 在当前仓库设置 Husky 预提交钩子，配合 lint-staged（Prettier）、类型检查和测试 |
| 安装 | husky + lint-staged + prettier（devDependencies） |
| 流程 | 检测包管理器 → 安装依赖 → 初始化 Husky → 创建 `.husky/pre-commit` → 创建 `.lintstagedrc` → 创建 `.prettierrc`（如缺失） → 验证 → 提交 |
| 调用方式 | 模型调用 |

### 个人技能（personal）

> 与个人设置相关的技能，未在插件中推广。

#### Edit Article — 文章编辑与改进

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/personal/edit-article/`](SKILLS/personal/edit-article/SKILL.md) |
| 用途 | 通过重组章节、提升清晰度、紧凑文字来编辑和改进文章 |
| 流程 | 按标题分节 → 确认章节顺序（信息为有向无环图） → 逐节重写（每段最多 240 字符） |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Obsidian Vault — Obsidian 笔记管理

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/personal/obsidian-vault/`](SKILLS/personal/obsidian-vault/SKILL.md) |
| 用途 | 在 Obsidian Vault 中搜索、创建和管理笔记，使用 wikilinks 和索引笔记 |
| 命名规范 | Title Case；索引笔记聚合相关主题；无文件夹组织——使用链接和索引笔记 |
| 工作流 | 按文件名/内容搜索 → 创建笔记（Title Case + wikilinks） → 查找反向链接 → 查找索引笔记 |
| 调用方式 | 模型调用 |

### 写作技能（writing）

> 开发中的写作技能，源自 in-progress 目录。

#### Writing Beats — 节拍式写作

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/writing/writing-beats/`](SKILLS/writing/writing-beats/SKILL.md) |
| 用途 | 将原始材料组装为节拍旅程，选择你自己的冒险风格，逐节拍写作 |
| 核心概念 | 节拍（旅程中的一个动作）、基础（概念在使用前必须被建立）、先决条件 vs 引入 |
| 流程 | 确立先决条件 → 2-3 个候选起始节拍 → 用户选择 → 仅写该节拍 → 重新读取 → 提供 2-3 个候选下一节拍 → 循环直到自然结束 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Writing Fragments — 碎片式写作

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/writing/writing-fragments/`](SKILLS/writing/writing-fragments/SKILL.md) |
| 用途 | 纯探索阶段——挖掘原始碎片，暂不施加结构 |
| 核心概念 | 碎片（任何可能存活到最终文章的文本片段）、引导词（承载全局的紧凑隐喻） |
| 文件格式 | H1 工作标题 + 碎片间用 `---` 分隔，无内部标题，无标签，无顺序 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

#### Writing Shape — 文章塑形

| 属性 | 值 |
|------|-----|
| 路径 | [`SKILLS/writing/writing-shape/`](SKILLS/writing/writing-shape/SKILL.md) |
| 用途 | 将原始材料逐段塑形为文章，在每个格式选择处进行论证 |
| 流程 | 读取材料 → 确立先决条件 → 2-3 个候选开头 → 逐段增长（从材料中拉取） → 论证格式选择（散文 vs 列表、内联 vs 标注、表格 vs 重复结构） → 循环直到完成 |
| 调用方式 | 用户调用（`disable-model-invocation: true`） |

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
