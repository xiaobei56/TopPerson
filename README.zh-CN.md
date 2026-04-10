[English](./README.md) | [简体中文](./README.zh-CN.md)

# 顶尖人 TopPerson

`TopPerson` 是一个开源的人物方法论 AI skill 仓库。

它要解决的问题很简单：

`遇到现实问题时，如果按某个顶尖人物的方式来判断、取舍和行动，会怎么做？`

## 目录

- [它能做什么](#它能做什么)
- [主要使用场景](#主要使用场景)
- [当前 Skill](#当前-skill)
- [怎么使用](#怎么使用)
- [怎么提议新增 Skill](#怎么提议新增-skill)
- [贡献要求](#贡献要求)
- [校验方式](#校验方式)
- [License](#license)

## 它能做什么

TopPerson 会把人物的著作、书信、演讲、访谈、传记和可信研究，整理成可被 AI 调用的 skill。

这个仓库主要做三件事：

- 提炼人物的方法论
- 翻译成现代可执行建议
- 让 AI 能稳定调用

这个仓库不做：

- 语录合集
- 名人崇拜
- 空洞鸡汤
- 操控、伤害、伪科学内容

## 主要使用场景

你可以用 TopPerson 的 skill 来处理：

- `生活`：自律、习惯、情绪、长期节奏
- `学习`：理解、记忆、解释、练习、建立学习方法
- `工作`：执行、沟通、带队、管理、产品判断、决策
- `人生指导`：重大选择、低谷调整、方向判断、价值取舍

## 当前 Skill

当前仓库状态： [`.agents/skills`](./.agents/skills) 下已有 `33` 个 skill 目录。

### 参考示例

- [`曾国藩 / zeng-guofan`](./.agents/skills/zeng-guofan/SKILL.md)

### 其他已创建 Skill

- [`安迪·格鲁夫 / andy-grove`](./.agents/skills/andy-grove/SKILL.md)
- [`本杰明·富兰克林 / benjamin-franklin`](./.agents/skills/benjamin-franklin/SKILL.md)
- [`曹操 / cao-cao`](./.agents/skills/cao-cao/SKILL.md)
- [`曹德旺 / cao-dewang`](./.agents/skills/cao-dewang/SKILL.md)
- [`查理·芒格 / charlie-munger`](./.agents/skills/charlie-munger/SKILL.md)
- [`段永平 / duan-yongping`](./.agents/skills/duan-yongping/SKILL.md)
- [`马斯克 / elon-musk`](./.agents/skills/elon-musk/SKILL.md)
- [`村上春树 / haruki-murakami`](./.agents/skills/haruki-murakami/SKILL.md)
- [`宫崎骏 / hayao-miyazaki`](./.agents/skills/hayao-miyazaki/SKILL.md)
- [`马云 / jack-ma`](./.agents/skills/jack-ma/SKILL.md)
- [`贝索斯 / jeff-bezos`](./.agents/skills/jeff-bezos/SKILL.md)
- [`黄仁勋 / jensen-huang`](./.agents/skills/jensen-huang/SKILL.md)
- [`稻盛和夫 / kazuo-inamori`](./.agents/skills/kazuo-inamori/SKILL.md)
- [`科比 / kobe-bryant`](./.agents/skills/kobe-bryant/SKILL.md)
- [`松下幸之助 / konosuke-matsushita`](./.agents/skills/konosuke-matsushita/SKILL.md)
- [`李光耀 / lee-kuan-yew`](./.agents/skills/lee-kuan-yew/SKILL.md)
- [`雷军 / lei-jun`](./.agents/skills/lei-jun/SKILL.md)
- [`罗翔 / luo-xiang`](./.agents/skills/luo-xiang/SKILL.md)
- [`马可·奥勒留 / marcus-aurelius`](./.agents/skills/marcus-aurelius/SKILL.md)
- [`拿破仑 / napoleon`](./.agents/skills/napoleon/SKILL.md)
- [`彼得·德鲁克 / peter-drucker`](./.agents/skills/peter-drucker/SKILL.md)
- [`纳达尔 / rafael-nadal`](./.agents/skills/rafael-nadal/SKILL.md)
- [`Ray Dalio / ray-dalio`](./.agents/skills/ray-dalio/SKILL.md)
- [`任正非 / ren-zhengfei`](./.agents/skills/ren-zhengfei/SKILL.md)
- [`理查德·费曼 / richard-feynman`](./.agents/skills/richard-feynman/SKILL.md)
- [`乔布斯 / steve-jobs`](./.agents/skills/steve-jobs/SKILL.md)
- [`苏轼 / su-shi`](./.agents/skills/su-shi/SKILL.md)
- [`王兴 / wang-xing`](./.agents/skills/wang-xing/SKILL.md)
- [`王阳明 / wang-yangming`](./.agents/skills/wang-yangming/SKILL.md)
- [`巴菲特 / warren-buffett`](./.agents/skills/warren-buffett/SKILL.md)
- [`张一鸣 / zhang-yiming`](./.agents/skills/zhang-yiming/SKILL.md)
- [`诸葛亮 / zhuge-liang`](./.agents/skills/zhuge-liang/SKILL.md)

更多规划可看：

- 英文 backlog：[`docs/person-backlog.md`](./docs/person-backlog.md)
- 中文 backlog：[`docs/person-backlog.zh-CN.md`](./docs/person-backlog.zh-CN.md)

## 怎么使用

### 1. 先选人物

进入 [`.agents/skills`](./.agents/skills) 选择一个人物。

### 2. 直接调用

例如：

```text
Use $zeng-guofan to analyze this situation and give me actionable advice.
```

### 3. 按问题场景去问

例如：

```text
Use $wang-yangming to help me stop overthinking and start acting.
Use $richard-feynman to help me learn this topic clearly.
Use $lei-jun to help me judge this product direction.
Use $duan-yongping to help me decide whether this opportunity is worth doing.
```

## 怎么提议新增 Skill

如果你想新增一个人物 skill，建议按这个最短路径来：

1. 先选一个资料足够扎实的人物。
2. 说明普通人为什么能用这个人的方法。
3. 写清这个 skill 主要解决什么问题。
4. 列出一手资料和二手资料。
5. 提 issue 或直接发 PR。

相关入口：

- [`CONTRIBUTING.zh-CN.md`](./CONTRIBUTING.zh-CN.md)
- [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- [`docs/review-checklist.zh-CN.md`](./docs/review-checklist.zh-CN.md)
- [`docs/review-checklist.md`](./docs/review-checklist.md)

推荐从这些模板开始：

- [`templates/person-skill/SKILL.md`](./templates/person-skill/SKILL.md)
- [`templates/person-skill/references/source-map.md`](./templates/person-skill/references/source-map.md)
- [`templates/person-skill/references/principles.md`](./templates/person-skill/references/principles.md)
- [`templates/person-skill/agents/openai.yaml`](./templates/person-skill/agents/openai.yaml)

## 贡献要求

好的贡献应该满足：

- 有来源
- 有方法论
- 能现代转译
- 能被 AI 稳定调用

请避免：

- 语录堆砌
- 神化人物
- 伪史料和伪引文
- 非法、欺骗、操控、伤害性建议

## 校验方式

发 PR 前运行：

```bash
python3 scripts/validate_skills.py
```

## License

本仓库采用 [`MIT License`](./LICENSE)。
