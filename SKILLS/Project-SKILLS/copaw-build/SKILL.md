---
name: copaw-build
description: 构建龙虾，龙虾打包，CoPaw (VJSP-Claw) Python 项目 PyInstaller 构建技能。涵盖虚拟环境激活、PyInstaller 打包、构建产物复制到 VJSP 客户端等完整构建流程。
---

# copaw-build

## 概述

CoPaw 是一个基于 Python 的 AI 助手项目，使用 PyInstaller 打包为 Windows 独立可执行文件 `VJSP-Claw.exe`。构建产物最终会被复制到 VJSP 客户端项目的 [`apps/web/copaw-dist`](apps/web/copaw-dist) 目录，供 Electron 应用集成使用。

## 构建前置条件

### 1. 项目结构

- [`copaw/`](copaw/) — CoPaw Python 项目根目录
- [`copaw/.venv/`](copaw/.venv/) — Python 虚拟环境（必须已创建并安装所有依赖）
- [`copaw/copaw.spec`](copaw/copaw.spec) — PyInstaller 打包配置文件
- [`copaw/src/run_copaw.py`](copaw/src/run_copaw.py) — 应用入口文件
- [`copaw/console/`](copaw/console/) — 前端控制台（需先构建，产物在 `console/dist/`）
- [`scripts/copy-copaw-build.ps1`](scripts/copy-copaw-build.ps1) — 构建产物复制脚本

### 2. 依赖准备

- Python 3.10+（由 [`.python-version`](copaw/.python-version) 指定）
- PyInstaller（已安装在虚拟环境中）
- 所有项目依赖已通过 `pip install -e .` 安装
- 前端控制台已构建：在 [`copaw/console/`](copaw/console/) 目录下执行 `npm run build`
- VJSPEasySDK-Python已经安装：在`VJSPEasySDK-Python`目录下执行`pip install -e .`（也需要虚拟环境）

## 构建步骤

### 步骤 1：激活虚拟环境

在 [`copaw/`](copaw/) 目录下激活 Python 虚拟环境：

```powershell
# Windows PowerShell
cd copaw
.\.venv\Scripts\Activate.ps1
```

```cmd
# Windows CMD
cd copaw
.venv\Scripts\activate.bat
```

激活后，终端提示符前会显示 `(.venv)` 标识。

### 步骤 2：执行 PyInstaller 打包

在虚拟环境激活状态下，于 [`copaw/`](copaw/) 目录执行：

```powershell
pyinstaller.exe copaw.spec --clean --noconfirm
```

参数说明：
- `copaw.spec` — 使用项目根目录的打包配置文件
- `--clean` — 清理之前的构建缓存
- `--noconfirm` — 跳过确认提示

打包产物输出目录：[`copaw/dist/vjspclaw/`](copaw/dist/vjspclaw/)

#### 构建产物结构

```
copaw/dist/vjspclaw/
├── VJSP-Claw.exe          # 主可执行文件
├── copaw/                 # 资源文件
│   ├── console/           # 前端控制台静态资源
│   ├── agents/            # Agent 配置和技能文件
│   ├── tokenizer/         # 分词器数据
│   └── security/          # 安全规则文件
├── reme/                  # reme 配置
├── vjspeasyim/            # VJSP EasyIM SDK
└── ...                    # 其他 Python 运行时依赖
```

### 步骤 3：复制构建产物到 VJSP 客户端

在项目根目录执行 PowerShell 脚本：

```powershell
.\scripts\copy-copaw-build.ps1
```

该脚本执行以下操作：
1. 验证 [`copaw/dist/vjspclaw/VJSP-Claw.exe`](copaw/dist/vjspclaw/VJSP-Claw.exe) 是否存在
2. 清理目标目录 [`apps/web/copaw-dist/`](apps/web/copaw-dist/)
3. 将构建产物完整复制到目标目录
4. 验证复制结果并显示文件大小

## 完整构建命令（一键执行）

```powershell
# 从项目根目录执行
cd copaw
.\.venv\Scripts\Activate.ps1
pyinstaller.exe copaw.spec --clean --noconfirm
cd ..
.\scripts\copy-copaw-build.ps1
```

## 常见问题

### 1. 虚拟环境未找到

确保已创建虚拟环境并安装依赖：

```powershell
cd copaw
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -e .
pip install pyinstaller
```

### 2. 前端控制台未构建

PyInstaller 打包需要 [`copaw/console/dist/`](copaw/console/dist/) 目录存在：

```powershell
cd copaw/console
yarn install
yarn build
```

### 3. 构建产物复制失败

检查：
- 确保已成功执行 PyInstaller 打包
- 确保 [`copaw/dist/vjspclaw/VJSP-Claw.exe`](copaw/dist/vjspclaw/VJSP-Claw.exe) 文件存在
- 以管理员身份运行 PowerShell（如有权限问题）

### 4. PyInstaller 打包报错

常见原因：
- 缺少 hidden imports：在 [`copaw/copaw.spec`](copaw/copaw.spec) 的 `hiddenimports` 列表中添加缺失的模块
- 缺少数据文件：在 `datas` 列表中添加对应的数据目录映射
- 依赖版本冲突：检查 [`copaw/pyproject.toml`](copaw/pyproject.toml) 中的依赖版本

## 参考文件

- [`copaw/copaw.spec`](copaw/copaw.spec) — PyInstaller 打包配置（Analysis、EXE、COLLECT 定义）
- [`scripts/copy-copaw-build.ps1`](scripts/copy-copaw-build.ps1) — 构建产物复制脚本
- [`copaw/pyproject.toml`](copaw/pyproject.toml) — 项目依赖和元数据
- [`copaw/.python-version`](copaw/.python-version) — Python 版本要求