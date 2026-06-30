# 🖋️ Mystery Writer Skill (推理小说写作助手)

![Version](https://img.shields.io/badge/Version-1.2.0-blue.svg)
![Type](https://img.shields.io/badge/AI--Agent-Creative--Writing-orange.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Framework-Active-green.svg)

`Mystery Writer Skill` 是一款专注于**悬疑、推理、心理惊悚小说**创作的 AI 辅助教练与高拟真文本生成引擎。通过精密的逻辑回溯算法和严苛的情节管控管线，该技能能够帮助创作者或系统自动构建高智商、强反转、无逻辑破绽的悬疑故事架构。

---

## 🎯 核心功能特性

*   **🧩 零漏洞逻辑校验 (`timeline_verifier`)**：内置时间线与因果律动态审计，每生成 2000 字自动回溯前文，严防“吃设定”或“逻辑吃书”等常识性 Bug。
*   **🕸️ 智能线索网部署**：根据动态设定的 `red_herring_ratio`（红鲱鱼比例），自动在故事中交织编排“显性物证”、“隐性伏笔”与“合理误导信息”。
*   **🎭 叙事视点交替 (Dynamic POV)**：支持侦探、凶手、受害者等多视角自由轮动，并精准锁定“信息差（Information Asymmetry）”，让解谜过程充满张力。
*   **🛡️ 智能红线拦截**：原生拦截“机械降神”、“强行降智”、“无意义血腥”等低级叙事套路，确保故事的高级感与文学性。

---

## 🚀 快速启动指引

### 1. 环境准备
确保您的 AI 容器或 Agent 框架已载入本技能包，并正确读取了 `CONFIG.md` 配置文件。

### 2. 环境变量配置
在系统根目录中设置环境模式（或在对话中显式指定）：
```bash
# 设置为严格的本格推理模式
export MYSTERY_ENV_MODE="strict_deduction"
3. 初始化指令 (Prompt)

向加载了该技能的 AI 发送以下激活指令：

    “初始化 Mystery Writer Skill。请读取 CONFIG.md 配置，准备以 [本格推理 90% / 心理惊悚 80%] 的文风权重，开始构建全新的暴风雪山庄模式大纲。”

📈 自动化写作管线 (Pipeline)

本技能的运行严格遵循以下四阶段闭环生命周期：

    Phase 1: 核心诡计与世界观 (Core Trick & Lore)

        定义不可能犯罪类型（密室、叙述性诡计、不在场证明盲点）。

        构建死者与嫌疑人的 Graph 关系图谱。

    Phase 2: 伏笔与线索网部署 (Clues & Red Herrings)

        根据配置比例（默认 30% 误导）自动埋设真假线索。

    Phase 3: 动态大纲与视点交替 (Dynamic Outline & POV)

        输出分幕大纲，锁定读者、侦探与反派的三方信息差。

    Phase 4: 文本生成与逻辑回溯校验 (Generation & Verification)

        生成具体章节小说文本，并持续触发底层校验器进行闭环审计。

📂 目录与文件结构

    README.md - 本说明文件（引导与核心概述）。

    CONFIG.md - 核心参数配置文件（控制逻辑严密性、文风权重、输出模板及高级 JSON 插件）。

    /templates - 存放人物卡、线索追踪矩阵、章节细纲等 Markdown 标准化模板。

    /plugins - 包含 timeline_verifier（时间线校验）等底层伪代码逻辑。

⚙️ 进阶微调 (Advanced Tuning)

如需深度定制 AI 的写作偏好，请直接修改 CONFIG.md 中的参数：

    追求极度烧脑、无懈可击：将 logic_strictness 调至 1.00，并开启 motive_analyzer: strict。

    追求快节奏、重口味犯罪悬疑：调高 Gore 权重至 60%，并将 pacing_control 设为 Fast-Paced。

📄 开源协议 (License)

本项目基于 MIT License 协议开源。这意味着您可以自由地商业化使用、修改和分发此技能配置，唯独需要在衍生作品中附带原作者的版权声明。

让每一次反转，都在意料之外；让每一个线索，都在情理之中。