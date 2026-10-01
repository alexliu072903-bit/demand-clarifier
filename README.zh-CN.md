# demand-clarifier

**[English](README.md) | 中文**

一个 skill，帮你在有人写文档之前，把产品想法想清楚。它会追问、挑战你的假设，并且每次对话都以一个具体的下一步结束。

支持 Claude Code、Codex，以及任何能加载 `SKILL.md` 的 Agent，也可以放进 Claude Project 使用。

## 它做什么

- 先判断产品是 ToB 还是 ToC，因为后面的检查项不一样。
- 判断你现在需要什么：探索方向、在方案间做决定、定义范围，还是研究某个主题。
- 运行下面的命令之一：

| 命令 | 做什么 |
| --- | --- |
| `/office-hours` | 逐个问六个问题，然后重述问题、挑战三个前提、给出从最小到最大的三条路径 |
| `/ceo-review` | 用十个部分审查想法，从痛点是否真实到最大风险，最后给出建议：缩减、保持、选择性扩展、扩展 |
| `/autoplan` | 两个都跑，输出一份综合决策摘要 |
| `@oracle "问题"` | 只分析：列出方案和取舍，不执行，等你说选哪个再继续 |

- 输出可以交给工程团队的设计文档摘要。

## 安装

把仓库克隆到你的 Agent 的 skills 目录。

Claude Code：

```bash
git clone https://github.com/alexliu072903-bit/demand-clarifier ~/.claude/skills/demand-clarifier
```

Codex：

```bash
git clone https://github.com/alexliu072903-bit/demand-clarifier ~/.codex/skills/demand-clarifier
```

然后描述你的想法，或者使用命令：

```text
/office-hours 我在想做一个面向团队的习惯打卡工具。
```

### 在 Claude Project 里使用

1. 新建一个 Project。
2. 把 `SKILL.md` 的内容粘贴到 Project 的指令里。
3. 把 `references/` 里的文件上传到 Project 知识库。

## 语言

指令本身是中文写的。Skill 会用你提问时使用的语言回答。

## 目录

```text
SKILL.md                    角色、原则、产品类型、意图分类、规则
references/office-hours.md  六个问题与设计文档摘要
references/ceo-review.md    十节审查与范围建议
references/oracle.md        只分析模式
references/autoplan.md      串联运行并合并结论
references/knowledge.md     框架、访谈问题库和模板
```

## 原则

- **先问，再动。** 问题没想清楚之前，不写任何文档。
- **挑战假设，不确认假设。** 每个判断都有立场和理由。
- **一个下一步。** 每次对话都以一件今天就能做的具体事情结束。

## 适合谁

- 想要一个思考搭档、而不是一个附和者的产品经理。
- 总因为需求不清楚而做错东西的开发者。
- 被要求写 PRD、规格说明或任务清单、应该先确认问题的 AI Agent。

## License

MIT
