# 审查清单 / Review Checklist

这份清单用于维护者审查 skill 提交，也适合提交者自查。
This checklist is for maintainers reviewing submissions and for contributors self-checking before a PR.

## A. 来源审查 / Source Review

- 是否明确区分了一手资料、二手研究、低置信来源
- 核心原则是否主要来自高置信来源
- 是否存在“网上都这么说”但没有来源的句子
- 是否把争议较大的文本降权处理
- 是否避免把小说化、鸡汤化、营销化内容当成核心依据

English:

- Are primary, secondary, and low-confidence sources clearly separated?
- Are core principles grounded mainly in high-confidence sources?
- Are there unsourced “everyone says this” statements?
- Are disputed texts treated with reduced confidence?
- Does the submission avoid turning fiction, self-help, or marketing copy into core evidence?

## B. 方法审查 / Method Review

- 这个 skill 提炼的是“方法”，不是“人物介绍”
- 是否能回答现实问题，而不只是复述人物经历
- 是否形成了稳定的判断框架
- 是否提供了动作建议，而不只是抽象态度
- 是否说明了适用场景和不适用场景

English:

- Does the skill extract a method rather than merely present a biography?
- Can it answer real-world problems instead of just retelling life events?
- Does it present a stable judgment framework?
- Does it give actions instead of only attitudes?
- Does it explain where the method fits and where it does not?

## C. 现代适配审查 / Modern Translation Review

- 是否把历史情境翻译成现代合法场景
- 是否避免鼓励暴力、操控、歧视、羞辱、压迫
- 是否明确拒绝伪科学和伤害性做法
- 是否避免把人物缺陷包装成“高明手段”

English:

- Is the historical context translated into modern lawful settings?
- Does the skill avoid promoting violence, manipulation, discrimination, humiliation, or oppression?
- Does it clearly reject pseudoscience and harmful practices?
- Does it avoid packaging a person’s flaws as clever tactics?

## D. 结构审查 / Structure Review

- 目录结构是否符合仓库规范
- `SKILL.md` frontmatter 是否完整
- `agents/openai.yaml` 是否存在且字段齐全
- `references/source-map.md` 是否讲清来源层级
- `references/principles.md` 是否真的做了抽象整理
- `references/overview.md` 是否足够清晰，便于仓库访客理解
- 是否给出了输出格式和典型触发语句

English:

- Does the directory structure match repository conventions?
- Is `SKILL.md` frontmatter complete?
- Does `agents/openai.yaml` exist with the required fields?
- Does `references/source-map.md` explain source hierarchy clearly?
- Does `references/principles.md` perform real synthesis?
- Is `references/overview.md` clear enough for repository visitors?
- Does the skill provide an output format and example triggers?

## E. 可用性审查 / Usability Review

- 这个 skill 是否能直接拿来回答问题
- 输出框架是否明确稳定
- 语言是否清楚，不装腔作势
- 是否避免过度角色扮演和假古文
- 是否足够简洁，避免把技能写成百科全书

English:

- Can the skill be used immediately to answer real questions?
- Is the output structure stable and understandable?
- Is the language clear rather than performative?
- Does it avoid excessive roleplay or fake archaic prose?
- Is it concise enough not to become an encyclopedia?

## F. 一票否决项 / Hard Rejection Signals

出现以下情况，原则上直接要求修改或拒绝：
If any of the following appear, the submission should usually be rejected or sent back for revision:

- 明显伪史料或伪引文被当成核心依据
- 鼓励违法、伤害、欺骗、操控
- 大量相术、玄学、血统论、宿命论内容
- 提交的其实只是人物介绍，不是可调用 skill
- 结构不完整，无法稳定使用

English:

- Fake sources or fake quotations are treated as core evidence
- The skill encourages unlawful, harmful, deceptive, or manipulative conduct
- It relies heavily on physiognomy, mysticism, essentialism, or fatalism
- The submission is really just a profile, not an invokable skill
- The structure is incomplete and cannot be used reliably
