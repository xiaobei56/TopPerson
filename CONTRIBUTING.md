# 贡献指南 / Contributing

欢迎为 `顶尖人 TopPerson` 提交新的 skill 或改进现有 skill。
Welcome to contribute new skills or improve existing ones in `TopPerson`.

这个仓库接收的不是普通文章，而是可被 AI 调用的结构化人物方法论 skill。
This repository accepts structured, AI-usable person-methodology skills rather than ordinary articles.

我们最看重：
We care most about:

- 来源质量 / source quality
- 方法抽象能力 / method extraction
- 结构一致性 / structural consistency
- 现代适配能力 / modern translation and safety

## 适合提交什么 / What Fits This Repository

适合：
Good submissions:

- 某个历史人物的做事方法 skill
- 某个现代人物的决策风格 skill
- 对现有 skill 的来源补强、结构优化、错误纠正
- 更清晰的参考资料整理

不适合：
Not a fit:

- 单纯的人物简介 / plain biography
- 没有方法论抽象的传记摘要 / biography summary without method extraction
- 没有来源支撑的名言合集 / unsourced quote collection
- 含明显伪科学、相术、操控术、PUA、违法建议的内容 / pseudoscience, manipulation, or unlawful guidance

## 最低结构 / Minimum Skill Structure

每个 skill 建议放在：
Each skill should usually live under:

```text
.agents/skills/<skill-name>/
```

最低必需文件：
Minimum required files:

```text
.agents/skills/<skill-name>/SKILL.md
.agents/skills/<skill-name>/agents/openai.yaml
.agents/skills/<skill-name>/references/source-map.md
.agents/skills/<skill-name>/references/principles.md
```

推荐补充：
Recommended additional file:

```text
.agents/skills/<skill-name>/references/overview.md
```

文件用途 / File roles:

- `SKILL.md`
  主 skill 文件，说明 skill 做什么、何时触发、怎么输出。
  Main skill file describing purpose, triggers, and output style.
- `references/overview.md`
  给人阅读的说明页，适合放双语简介、来源概览、使用方式。
  Human-facing guide for bilingual description, source summary, and usage.
- `references/source-map.md`
  写清来源层级，一手资料、二手资料、低置信资料如何排序。
  Source hierarchy: primary, secondary, and low-confidence materials.
- `references/principles.md`
  把人物方法论翻译成现代可执行原则。
  Distilled principles translated into modern actionable guidance.
- `agents/openai.yaml`
  用于 UI 与调用元数据。
  UI-facing and invocation metadata.

## 命名规范 / Naming Rules

- skill 文件夹名使用小写加连字符，例如 `zeng-guofan`
- `SKILL.md` frontmatter 中的 `name` 必须与文件夹名一致
- 名称应尽量简短、稳定、可预测

In English:

- Use lowercase hyphenated folder names such as `zeng-guofan`
- The `name` field in `SKILL.md` frontmatter must match the folder name
- Names should be short, stable, and predictable

## 内容规范 / Content Rules

### 1. 一手资料优先 / Prefer Primary Sources

优先使用：
Prefer:

- 著作 / books by the person
- 书信 / letters
- 日记 / diaries
- 讲话 / speeches
- 论文 / papers
- 访谈 / interviews
- 原始公开材料 / verified public materials

如果一手资料不足，可以使用高质量二手研究，但必须在 `source-map.md` 里讲清楚。
If primary sources are limited, high-quality secondary research is acceptable, but explain that clearly in `source-map.md`.

### 2. 区分来源置信度 / Separate Source Confidence

至少分成三层：
At minimum, use three layers:

- 高置信来源 / high-confidence sources
- 辅助解释来源 / interpretive supporting sources
- 低置信或存疑来源 / low-confidence or disputed sources

### 3. 不做“名言拼盘” / Do Not Build Quote Dumps

我们要的是：
We want:

- 可复用的判断框架 / reusable judgment frameworks
- 可执行的动作建议 / actionable guidance
- 明确的适用边界 / clear boundaries

不是：
Not:

- 励志句子堆砌 / motivational quote piles
- 伪古文口号 / fake archaic slogans
- 把人物神化成万能导师 / turning a person into a mythic guru

### 4. 必须做现代适配 / Must Translate To Modern Contexts

历史人物 skill 不能直接照搬时代环境。
Historical skills cannot import their original era literally.

必须转译成现代、合法、伦理上可接受的表达。
They must be translated into modern, lawful, ethically acceptable guidance.

例如：
Examples:

- 不鼓励暴力 / do not encourage violence
- 不鼓励操控和羞辱 / do not encourage manipulation or humiliation
- 不鼓励歧视或压迫 / do not encourage discrimination or oppression
- 不鼓励把相术、出身、权谋当作核心方法 / do not center physiognomy, class bias, or power games

### 5. 给出明确输出结构 / Provide A Clear Output Shape

建议每个 skill 提供默认输出结构，例如：
Each skill should suggest a stable default output structure, such as:

- 总判断 / core judgment
- 先做什么 / first moves
- 不要做什么 / avoid
- 短中期动作 / short- and mid-term plan
- 沟通建议 / communication advice
- 反思问题 / reflection question

## 推荐流程 / Recommended Workflow

1. 整理人物的真实来源 / gather real sources
2. 在 `source-map.md` 里建立来源层级 / build source hierarchy
3. 在 `principles.md` 里提炼核心方法 / distill principles
4. 在 `SKILL.md` 里写触发条件、使用方法、输出格式、边界 / write triggers, usage, output, boundaries
5. 在 `references/overview.md` 里写双语说明 / add a bilingual overview
6. 本地运行校验脚本 / run local validation
7. 提交 PR / open a PR

## 提交前自查 / Pre-Submission Checklist

- `python3 scripts/validate_skills.py` 可以通过 / passes successfully
- `SKILL.md` frontmatter 完整 / complete frontmatter
- 必需文件都在 / required files exist
- `references/source-map.md` 写清来源层级 / source hierarchy is explicit
- `references/principles.md` 不是纯摘抄 / principles are distilled, not copied
- 没有明显伪史料、伪引文、伪科学内容 / no obvious fake sources or pseudoscience
- 没有鼓励非法、欺骗、操控、伤害性的建议 / no unlawful, deceptive, manipulative, or harmful guidance

## PR 应该写什么 / What A PR Should Include

PR 描述至少说明：
A PR description should at least include:

- 这个 skill 对应谁 / who the skill is about
- 主要参考了哪些来源 / main sources used
- 适合解决什么问题 / what kinds of problems it helps solve
- 争议点或低置信内容如何处理 / how disputed or low-confidence material was handled

请使用仓库自带 PR 模板。
Please use the repository PR template.

## 审查标准 / Review Standard

维护者主要按以下维度审查：
Maintainers review along these dimensions:

1. 来源质量 / source quality
2. 结构完整度 / structural completeness
3. 方法抽象质量 / quality of method extraction
4. 现代适配与安全边界 / modern translation and safety boundaries
5. 可读性与可调用性 / readability and AI usability

更细清单见：
For a more detailed checklist, see:

- [`docs/review-checklist.md`](./docs/review-checklist.md)

## 小建议 / Suggestions

- 宁可少写，但要写准 / write less, but write accurately
- 宁可少引用金句，也要把方法讲清 / fewer quotes, clearer method
- 宁可承认“不确定”，也不要装作确定 / say when confidence is limited
- 让 skill 像可靠的思考框架，而不是花哨人格扮演器 / make the skill a reliable thinking framework, not a flashy roleplay persona
