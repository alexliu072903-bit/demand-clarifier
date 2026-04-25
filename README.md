# demand-clarifier

**A structured prompt system for clarifying product requirements before writing a single line of documentation.**

Built for AI coding agents and product managers who want to think clearly before they build.

---

## What This Is

`demand-clarifier` is a two-file prompt system that turns vague product ideas into actionable, well-scoped decisions. It combines a YC partner's instinct for early-stage products with a senior PM's systematic thinking.

Two files, two purposes:

- **`Instructions.md`** — The operating system. Defines how the AI agent thinks, questions, and responds.
- **`Knowledge.md`** — The knowledge base. Frameworks and templates the agent draws on when going deeper.

---

## What It Does

- Identifies whether a product is **ToB or ToC** before anything else
- Classifies your intent: explore / decide / define / research
- Runs structured review sessions from two perspectives: YC partner and serial founder
- Challenges assumptions instead of confirming them
- Outputs a **Design Document Summary** ready for handoff to engineering

---

## Commands

| Command | What It Does |
|---------|-------------|
| `/office-hours` | YC mentor mode — redefines what you're actually building |
| `/ceo-review` | Founder mode — 10-node review, challenges scope and assumptions |
| `/autoplan` | Runs both in sequence, outputs a combined decision summary |
| `@oracle "question"` | Analysis only — gives options and tradeoffs, never executes |

---

## How to Use

### With Claude (recommended)

1. Start a new Project in Claude
2. Upload both `Instructions.md` and `Knowledge.md` to Project Knowledge
3. Start a conversation — the agent will follow the instruction system automatically

### With other AI agents

Paste the contents of `Instructions.md` as a system prompt. Reference `Knowledge.md` when deeper framework analysis is needed.

---

## Design Principles

**Ask first, build later.** No documentation is written until the problem is clear.

**Challenge assumptions, don't confirm them.** Every judgment has a position and a reason. No "both are valid" answers.

**One clear next action.** Every session ends with something specific you can do today.

**Complete output only.** Partial answers are broken answers.

---

## Who This Is For

- Product managers who want a thinking partner, not a yes-machine
- Developers who keep building the wrong thing because requirements weren't clear
- AI agents being asked to write PRDs, tech specs, or task lists

---

## License

MIT — use it, adapt it, build on it.

---

---

# demand-clarifier（中文版）

**一套结构化的提示词系统，在写任何一行文档之前，先把需求想清楚。**

为 AI 编程助手和产品经理设计——先想清楚，再动手建。

---

## 这是什么

`demand-clarifier` 是一个两文件提示词系统，帮你把模糊的产品想法转化为清晰、有边界的决策。它结合了 YC 合伙人对早期产品的直觉，以及资深产品经理的系统性思维。

两个文件，两个用途：

- **`Instructions.md`** — 操作系统。定义 AI agent 如何思考、如何提问、如何回应。
- **`Knowledge.md`** — 知识库。当需要深入某个框架时，agent 会自动调用这里的内容。

---

## 它能做什么

- 在一切开始之前，先判断产品是 **ToB 还是 ToC**
- 识别你的意图：探索方向 / 做决策 / 定义范围 / 做调研
- 从两个视角运行结构化审查：YC 合伙人 + 连续创业者
- 挑战假设，而不是确认假设
- 输出**设计文档摘要**，可直接交给工程团队

---

## 命令速查

| 命令 | 作用 |
|------|------|
| `/office-hours` | YC 导师模式——重新定义你真正在做什么 |
| `/ceo-review` | 创始人模式——10节审查，挑战范围和假设 |
| `/autoplan` | 自动串联两个模式，输出综合决策摘要 |
| `@oracle "问题"` | 只分析不执行——给出多方案权衡，不替你拍板 |

---

## 如何使用

### 配合 Claude（推荐）

1. 在 Claude 新建一个 Project
2. 把 `Instructions.md` 和 `Knowledge.md` 上传到 Project Knowledge
3. 开始对话——agent 会自动按照指令系统运作

### 配合其他 AI agent

把 `Instructions.md` 的内容作为 system prompt 粘贴进去。需要深入框架分析时，引用 `Knowledge.md`。

---

## 设计原则

**先问，再动。** 问题没想清楚之前，不写任何文档。

**挑战假设，而不是确认假设。** 每个判断都有立场和理由，不做"都对"式回答。

**明确的下一步行动。** 每次对话结束都有今天可以做的具体一件事。

**只输出完整内容。** 不完整的输出等于损坏的输出。

---

## 适合谁用

- 想要一个思考伙伴而不是应声虫的产品经理
- 因为需求不清楚而反复做错事情的开发者
- 被要求写 PRD、技术文档或任务清单的 AI agent

---

## 许可证

MIT — 随意使用、改造、二次开发。
