# 🖋️ Mystery Writer Skill Configuration (CONFIG.md)

欢迎使用 **Mystery Writer Skill** 配置文件。本文件用于定义悬疑小说写作助手的核心逻辑、文风权重、角色设定以及自动化处理管线。

---

## 🛠️ 核心参数设定 (Core Settings)

以下参数决定了 AI 在生成悬疑内容时的基础行为偏好和逻辑严密性。

| 参数名称 (Parameter) | 默认值 (Value) | 类型 (Type) | 描述 (Description) |
| :--- | :--- | :--- | :--- |
| `logic_strictness` | `0.95` | Float | **逻辑严密性**：控制诡计与线索的无缝衔接，数值越高越无破绽。 |
| `pacing_control` | `Dynamic` | String | **节奏控制**：`Slow-Burn`（慢热）、`Fast-Paced`（快节奏）或 `Dynamic`（动态）。 |
| `red_herring_ratio` | `0.30` | Float | **红鲱鱼（误导线索）比例**：每组线索中虚假误导信息的占比。 |
| `climax_intensity` | `High` | String | **高潮张力**：决定收尾部分的戏剧冲突与反转力度。 |
| `auto_save_milestone`| `true` | Boolean| **自动保存**：在完成大纲、伏笔埋设等关键节点时自动备份。 |

---

## 🎭 文风与氛围权重 (Style & Atmosphere Weights)

通过调整以下权重，可以让故事偏向不同的悬疑流派（如：硬汉派、社会派、本格推理等）。

*   **🕵️‍♂️ 推理严密性 (Deduction)** `[██████████] 90%`
    *   专注于物证、不在场证明和逻辑链条的闭环。
*   **👁️ 心理惊悚 (Psychological Thriller)** `[████████░░] 80%`
    *   侧重于角色的内心独白、不可靠叙事者以及压抑氛围的营造。
*   **🌆 黑色电影风 (Noir / Gritty)** `[██████░░░░] 60%`
    *   冷酷的冷硬派侦探视角，多雨的城市背景，社会暗面的描绘。
*   **🩸 惊悚度 (Gore / Gore-Tex)** `[████░░░░░░] 40%`
    *   适度的犯罪现场描写，服务于悬念，不流于廉价恐怖。

---

## 📈 写作管线流 (Writing Pipeline)

技能启动后，将严格按照以下四阶段生命周期执行：

```mermaid
graph TD
    A[Phase 1: 核心诡计与世界观] --> B[Phase 2: 伏笔与线索网部署]
    B --> C[Phase 3: 动态大纲与视点交替]
    C --> D[Phase 4: 文本生成与逻辑回溯校验]

1. 核心诡计与世界观 (Core Trick & Lore)

    确立“不可能犯罪”类型（如：密室、孤岛、叙述性诡计）。

    生成死者、嫌疑人关系网络及核心动机（Motivations）。

2. 伏笔与线索网部署 (Clues & Red Herrings)

    显性线索 (Overt Clues)：警方直接发现的物证。

    隐性线索 (Covert Clues)：隐藏在对话、环境描写中的关键矛盾。

    误导信息 (Red Herrings)：合理的嫌疑人伪证或巧合。

3. 动态大纲与视点交替 (Dynamic Outline & POV)

    支持 多视角（POV） 轮动（如：神探视角、凶手视角、受害者视角）。

    控制信息差（Information Asymmetry），确保读者与侦探同步或滞后。

4. 文本生成与逻辑回溯校验 (Generation & Verification)

    每生成 2000 字进行一次“逻辑回溯”，确保后文没有推翻前文设置的定论。

🚫 规避红线 (Safety & Tropes to Avoid)

    ⚠️ 重要提示：
    为了保证故事的高级感与合规性，系统会自动过滤或重写包含以下内容的代码块/文本：

        机械降神 (Deus ex Machina)：禁止在结局突兀引入毫无铺垫的超自然力量或新人物来破案。

        降智打击 (Character Dumb Down)：侦探或反派的智商必须在线，禁止为了推进剧情强行让角色犯常识性错误。

        过度血腥 (Gratuitous Violence)：犯罪描写应服务于谜题本身，避免纯粹的感官刺激。

📂 输出格式配置 (Output Templates)

在生成章节、大纲或人物卡时，系统将遵循以下统一的 Markdown 格式输出：
人物卡模板示例
Markdown

### 👤 角色编码：[Name_ID]
*   **社会身份**：职业 / 年龄 / 与被害人关系
*   **表面动机**：公开的利益或情感冲突
*   **深层秘密**：核心诡计所隐藏的阴暗面
*   **携带线索**：[线索A (真) / 线索B (伪)]

⚙️ 高级扩展 (Advanced Extensions)
JSON

{
  "plugins": {
    "timeline_verifier": "enabled",
    "motive_analyzer": "strict",
    "cliché_detector": "active"
  },
  "ai_temperature": 0.72
}

如需修改以上高级底座参数，请联系系统管理员或调整环境变量 MYSTERY_ENV_MODE。