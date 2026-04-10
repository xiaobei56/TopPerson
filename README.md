# 顶尖人 TopPerson

`TopPerson` 是一个开源的「人物方法论 skill 仓库」。
`TopPerson` is an open-source repository of person-based skills for AI.

它不做名人语录收集，也不做人设崇拜，而是把人物的生平、原始著作、可信研究，整理成可以被 AI 调用的结构化 skill。
It is not a quote collection or a fandom project. It turns biographies, primary works, and credible research into structured skills that AI can use.

它想回答的问题是：
The core question is:

`如果按这个人的做事方式处理现实问题，会怎么判断、怎么取舍、怎么行动？`
`If we handled a real problem in this person's style, how would we judge, decide, and act?`

## 为什么做这个仓库 / Why This Repository

很多人物内容在互联网上会被压缩成：
Online content about notable people is often compressed into:

- 鸡汤金句 / motivational snippets
- 断章取义的“成功秘诀” / decontextualized “secrets”
- 神秘化、戏剧化的人设标签 / exaggerated personal branding

`TopPerson` 反过来做四件事：
`TopPerson` does the opposite:

- 回到来源 / go back to sources
- 提炼方法 / extract reusable methods
- 建立边界 / define boundaries
- 变成可执行的 skill / turn them into actionable skills

## 核心原则 / Core Principles

- `来源优先 / Source-first`
  一手资料优先，二手研究辅助，流行金句降权。
  Prefer primary materials, use secondary research as support, and downgrade viral quote culture.
- `方法优先 / Method-first`
  不做人物简介，要做可复用的判断框架。
  Do not stop at biography. Extract reusable judgment frameworks.
- `现代转译 / Modern translation`
  历史人物的方法必须翻译到现代、合法、非伤害性的语境。
  Historical methods must be translated into modern, lawful, non-harmful contexts.
- `结构统一 / Consistent structure`
  让不同 skill 都能稳定被 AI 调用和复用。
  Keep skills structured so they can be invoked reliably by AI.

## 当前已收录 / Current Skills

| Skill | Person | What it does |
| --- | --- | --- |
| `zeng-guofan` | 曾国藩 / Zeng Guofan | 用曾国藩的修身、识人、处事、带队框架分析现实问题 / Analyze real-world problems through Zeng Guofan's discipline, leadership, and judgment framework |

技能目录 / Skill files:

- [`zeng-guofan/SKILL.md`](./.agents/skills/zeng-guofan/SKILL.md)
- [`zeng-guofan/references/overview.md`](./.agents/skills/zeng-guofan/references/overview.md)
- [`zeng-guofan/references/source-map.md`](./.agents/skills/zeng-guofan/references/source-map.md)
- [`zeng-guofan/references/principles.md`](./.agents/skills/zeng-guofan/references/principles.md)

## 快速开始 / Quick Start

### 1. 浏览技能 / Browse Skills

进入 [`.agents/skills`](./.agents/skills) 查看已收录人物。
Browse [`.agents/skills`](./.agents/skills) to see available person skills.

### 2. 调用技能 / Use a Skill

在支持 skill 的环境里，你可以直接这样调用：
In a skill-enabled environment, invoke a skill like this:

```text
Use $zeng-guofan to analyze this situation in 曾国藩式做事风格，并给出可执行建议。
```

### 3. 查看单个 skill 说明 / Read a Skill Guide

每个 skill 可以在自己的目录里放说明文件。
Each skill can keep its own guide inside its directory.

例如 / Example:

- [`zeng-guofan/references/overview.md`](./.agents/skills/zeng-guofan/references/overview.md)

### 4. 本地校验 / Validate Locally

提交前运行：
Run this before opening a PR:

```bash
python3 scripts/validate_skills.py
```

### 5. 从模板开始 / Start From the Template

新增人物 skill 时，直接参考：
When adding a new person skill, start from:

- [`templates/person-skill/SKILL.md`](./templates/person-skill/SKILL.md)
- [`templates/person-skill/references/overview.md`](./templates/person-skill/references/overview.md)
- [`templates/person-skill/references/source-map.md`](./templates/person-skill/references/source-map.md)
- [`templates/person-skill/references/principles.md`](./templates/person-skill/references/principles.md)
- [`templates/person-skill/agents/openai.yaml`](./templates/person-skill/agents/openai.yaml)

## 曾国藩 Skill / Zeng Guofan Skill

### 这个 skill 做什么 / What This Skill Does

这个 skill 把曾国藩的做事方式整理成一套现代可用框架，重点放在：
This skill translates Zeng Guofan's way of working into a modern decision framework, especially for:

- 修身与自我整顿 / self-discipline and self-correction
- 团队治理与收拾烂摊子 / team cleanup and organizational repair
- 识人、用人、分责 / judging people, staffing, and ownership
- 冲突处理与信任修复 / conflict handling and trust repair
- 长期工程的节奏控制 / pacing long-term work
- 家庭、金钱、秩序与日常纪律 / family order, thrift, and routine

它不是为了模仿晚清权谋，也不是为了生产“成功学版曾国藩”。
It is not meant to imitate late-Qing power politics or produce a shallow “success guru” version of Zeng Guofan.

### 参考内容 / Source Base

高优先级材料 / High-confidence materials:

- `《曾国藩家书》`
- `《曾国藩日记》`
- `奏折、批牍、书信、读书札记、诗文`
- `《曾国藩全集》`

辅助解释材料 / Supporting interpretive materials:

- 唐浩明相关整理与研究
- 张宏杰相关传记与研究
- 年谱、导读、学术研究论文

低置信辅助材料 / Low-confidence auxiliary materials:

- `《冰鉴》`
- `《挺经》`
- 网络流传的“曾国藩名言”与商业鸡汤式二次加工

这个仓库对来源的基本态度是：
This repository follows one source rule:

`一手资料优先，二手研究辅助，流行金句降权。`
`Primary materials first, secondary research second, viral quote culture downgraded.`

### 怎么使用 / How To Use It

可以直接调用：
Direct invocation:

```text
Use $zeng-guofan to analyze this situation in 曾国藩式做事风格，并给出可执行建议。
```

也可以自然语言触发：
Natural-language triggers also work:

- `按曾国藩的风格看，这个团队烂摊子该怎么收拾？`
- `如果是曾国藩，会怎么处理合作伙伴失信？`
- `用曾国藩的方法帮我定一个三十天自我整顿计划。`
- `我该不该现在辞职创业？请用曾国藩式做事法来判断。`

### 默认输出结构 / Default Output Shape

- `曾式总判 / Core judgment`
- `先办什么 / First moves`
- `暂不做什么 / Avoid`
- `今日 / 七日 / 三十日 / Today / 7 days / 30 days`
- `对人怎么说 / If you need to say it`
- `自省一问 / Reflection question`

## 欢迎贡献 / Contributing

欢迎大家提交更多人物 skill，例如历史人物、企业家、投资人、学者、管理者、或某个领域的顶尖实践者。
Contributions are welcome for historical figures, founders, investors, scholars, managers, and outstanding practitioners in specific domains.

但请不要把仓库做成：
Please do not turn this repository into:

- 语录大全 / a quote dump
- 神化人物的宣传材料 / hero worship
- 没有来源的“成功学” / unsourced self-help
- 鼓吹操控、压迫、洗脑、伪科学的方法库 / manipulative, harmful, or pseudoscientific guidance

开始贡献前，请先看：
Before contributing, read:

- [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- [`docs/review-checklist.md`](./docs/review-checklist.md)
- [`.github/PULL_REQUEST_TEMPLATE.md`](./.github/PULL_REQUEST_TEMPLATE.md)

## 仓库结构 / Repository Structure

```text
.agents/skills/
  <skill-name>/
    SKILL.md
    agents/openai.yaml
    references/
      overview.md
      source-map.md
      principles.md

docs/
  review-checklist.md

scripts/
  validate_skills.py

templates/
  person-skill/
    SKILL.md
    agents/openai.yaml
    references/
      overview.md
      source-map.md
      principles.md
```

## 自动校验 / Validation

仓库包含一个本地校验脚本和 GitHub Action。
The repository includes a local validation script and a GitHub Action.

- 本地运行 / local: `python3 scripts/validate_skills.py`
- PR 自动运行 / CI: `.github/workflows/validate-skills.yml`

它会检查：
It checks:

- skill 目录命名 / skill directory naming
- `SKILL.md` frontmatter
- 必需文件是否存在 / required files
- `openai.yaml` 关键字段 / key `openai.yaml` fields

## License

本仓库采用 [`MIT License`](./LICENSE)。
This repository is released under the [`MIT License`](./LICENSE).

这意味着：
This means:

- 代码、脚本、结构和仓库组织方式可以自由复用
- 贡献内容前请确认你有权提交
- 不要直接搬运受版权保护的长篇原文
- code, scripts, and repository structure can be reused freely
- only contribute content you have the right to submit
- do not copy long copyrighted source texts into the repository
