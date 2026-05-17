**[English](README.md) | [中文](README.zh.md)**

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

MIT
