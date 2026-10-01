# demand-clarifier

**English | [中文](README.zh-CN.md)**

A skill that helps you think a product idea through before anyone writes a document. It asks hard questions, challenges your assumptions, and ends every session with one concrete next step.

It works with Claude Code, Codex, and any agent that loads a `SKILL.md`. You can also use it in a Claude Project.

## What it does

- Decides first whether the product is ToB or ToC, because the checks that follow differ.
- Classifies what you need: explore a direction, decide between options, define scope, or research a topic.
- Runs one of these commands:

| Command | What it does |
| --- | --- |
| `/office-hours` | Asks six questions one at a time, then restates the problem, challenges three assumptions, and offers three paths from smallest to largest |
| `/ceo-review` | Reviews the idea in ten sections, from whether the pain is real to the biggest risk, then recommends: shrink, keep, selectively expand, or expand |
| `/autoplan` | Runs both and gives one combined decision summary |
| `@oracle "question"` | Analyzes only. Lays out options and trade-offs, never executes, and waits until you say which way to go |

- Gives a design-document summary you can hand to engineering.

## Install

Clone the repository into your agent's skills directory.

For Claude Code:

```bash
git clone https://github.com/alexliu072903-bit/demand-clarifier ~/.claude/skills/demand-clarifier
```

For Codex:

```bash
git clone https://github.com/alexliu072903-bit/demand-clarifier ~/.codex/skills/demand-clarifier
```

Then describe your idea, or use a command:

```text
/office-hours I am thinking about building a habit tracker for teams.
```

### In a Claude Project

1. Start a new Project.
2. Paste the contents of `SKILL.md` into the Project instructions.
3. Upload the files in `references/` to Project knowledge.

## Language

The instructions are written in Chinese. The skill answers in the language you write in.

## What is inside

```text
SKILL.md                    role, principles, product type, intent classification, rules
references/office-hours.md  the six questions and the design-document summary
references/ceo-review.md    the ten-section review and the scope recommendation
references/oracle.md        analysis-only mode
references/autoplan.md      running both and combining them
references/knowledge.md     frameworks, interview question bank, and templates
```

## Principles

- **Ask first, build later.** No documentation is written until the problem is clear.
- **Challenge assumptions, do not confirm them.** Every judgment has a position and a reason.
- **One next action.** Every session ends with something specific you can do today.

## Who it is for

- Product managers who want a thinking partner, not a yes-machine.
- Developers who keep building the wrong thing because the requirement was unclear.
- AI agents asked to write a PRD, spec, or task list who should first confirm the problem.

## License

MIT
