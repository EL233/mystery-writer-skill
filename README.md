# 🖋️ Mystery Writer Skill（推理小说写作助手）

![Version](https://img.shields.io/badge/Version-1.2.0-blue.svg)
![Type](https://img.shields.io/badge/AI--Agent-Creative--Writing-orange.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Framework-Active-green.svg)

Mystery Writer Skill 是一个面向 AI Agent 的悬疑小说创作增强框架。

它通过结构化提示词、人物关系管理、线索矩阵、时间线审计以及叙事约束系统，帮助 AI 生成具有以下特质的悬疑、推理、心理惊悚类故事：

- 严密因果关系
- 多层线索布局
- 高信息差设计
- 反转闭环结构

本项目适用于：

- ChatGPT 自定义 GPT / Project
- Claude Project
- Gemini Gem
- 本地 Agent 框架
- 其他支持 Markdown Skill / Prompt Package 的 AI 平台

---

## ✨ Features

### 🧩 Timeline Verification 时间线校验

通过章节级时间线记录，辅助 AI 检查：

- 人物行动是否符合时间顺序
- 不在场证明是否成立
- 事件因果是否闭合
- 前文设定是否冲突

> **目标：** 每一个关键事件，都能在故事内部找到原因。

---

### 🕸️ Clue Network 线索网络系统

自动管理：

- 核心证据
- 假线索（Red Herring）
- 隐藏伏笔
- 信息误差
- 最终解释路径

支持配置：

```yaml
red_herring_ratio: 0.30
clue_density: high
foreshadowing_level: advanced
```

示例：

| 类型 | 内容 |
| :--- | :--- |
| 表面线索 | A 在案发时间进入房间 |
| 隐藏信息 | 监控时间存在延迟 |
| 最终解释 | 进入房间的人并非 A |

---

### 🎭 Dynamic POV 叙事视角控制

支持视角类型：

- 侦探视角
- 犯罪者视角
- 受害者视角
- 第三人称限制视角

自动控制：

- 角色知道的信息
- 读者知道的信息
- 真相隐藏程度

避免：

- 作者提前泄底
- 角色突然获得未知信息
- 视角作弊

---

### 🧠 Mystery Logic Engine 推理逻辑框架

**支持生成的不可能犯罪类型：**

- 密室
- 暴风雪山庄
- 时间诡计
- 身份诡计
- 叙述性诡计

**犯罪结构：**
犯罪动机
↓
犯罪机会
↓
执行方式
↓
误导设计
↓
真相揭示
---

## 🚀 Quick Start

### 1. 加载 Skill

将项目文件导入你的 AI 平台：
mystery-writer-skill/
├── SKILL.md
├── CONFIG.md
├── README.md
├── templates/
│   ├── character.md
│   ├── clue_matrix.md
│   ├── chapter_outline.md
├── plugins/
│   └── timeline_verifier.md
└── examples/
### 2. 初始化

发送：
初始化 Mystery Writer Skill。
读取 CONFIG.md。
进入悬疑小说创作模式。
请根据当前配置生成故事架构。
### 3. 创建故事

示例：
使用暴风雪山庄模式。
要求：

7名嫌疑人
1名真实凶手
双重诡计
最终解释必须闭环

先生成案件设计。
---

## 📈 Writing Pipeline

整个创作流程：
Idea
│
▼
Core Mystery 核心谜题设计
│
▼
Character Graph 人物关系网络
│
▼
Clue Matrix 线索矩阵部署
│
▼
Chapter Outline 章节规划
│
▼
Generation 正文生成
│
▼
Verification 逻辑审计

---

## 📂 Project Structure
mystery-writer-skill/
├── README.md
├── SKILL.md
├── CONFIG.md
├── templates/
│   ├── character.md
│   ├── case.md
│   ├── clue_matrix.md
│   ├── chapter_outline.md
├── plugins/
│   ├── timeline_verifier.md
│   └── logic_checker.md
└── examples/
├── short-demo/
└── long-demo/
---

## ⚙️ Configuration

通过 `CONFIG.md` 调整创作方向。

示例：

```yaml
logic_strictness: 0.95

mystery_style:
  deduction: 90
  psychological: 80
  thriller: 50

pacing:
  mode: balanced

violence:
  level: low
```

### 高逻辑推理模式

推荐配置：

```yaml
logic_strictness: 1.00

motive_analyzer:
  mode: strict

timeline_check:
  enabled: true
```

适合：

- 本格推理
- 复杂案件
- 多重反转

### 心理悬疑模式

推荐配置：

```yaml
psychology_weight: 90
character_conflict: high
unreliable_narrator: true
```

适合：

- 心理犯罪
- 人格反转
- 叙述欺骗

---

## 🛠️ Custom Extensions

可以新增：
plugins/
├── dream_logic.md
├── fair_play_checker.md
└── character_arc.md
用于扩展 AI 行为。

例如 `fair_play_checker` 用于检测：

- 真相是否提前提供足够提示
- 读者是否拥有公平推理机会
- 反转是否依赖隐藏规则

---

## 🤝 Contribution

欢迎提交：

- 新模板
- 新推理结构
- 新校验规则
- 案例库

建议保持：

- 可解释
- 可复用
- 平台无关

---

## 📄 License

MIT License

允许：

- 修改
- 二次开发
- 商业使用
- 发布衍生版本

请保留原始版权声明。