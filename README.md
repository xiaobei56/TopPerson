[English](./README.md) | [简体中文](./README.zh-CN.md)

# TopPerson

`TopPerson` is an open-source repository of person-based AI skills.

It helps AI answer a practical question:

`How would a top person judge, decide, and act in this situation?`

## Contents

- [What It Does](#what-it-does)
- [Main Use Cases](#main-use-cases)
- [Current Skills](#current-skills)
- [How To Use](#how-to-use)
- [How To Propose A New Skill](#how-to-propose-a-new-skill)
- [Contribution Rules](#contribution-rules)
- [Validation](#validation)
- [License](#license)

## What It Does

TopPerson turns biographies, primary works, letters, speeches, interviews, and credible research into reusable skills.

This repository is for:

- practical judgment
- action planning
- modern translation of historical or modern methods

This repository is not for:

- quote collections
- fandom
- empty motivation
- harmful or manipulative guidance

## Main Use Cases

You can use TopPerson skills to think through:

- `Life`: self-discipline, habits, emotional stability, long-term direction
- `Study`: learning methods, focus, explanation, practice, curiosity
- `Work`: execution, management, communication, product judgment, decision-making
- `Life guidance`: major choices, setbacks, transitions, values, how to act next

## Current Skills

Current repository status: `33` skill directories in [`.agents/skills`](./.agents/skills).

### Reference Skill

- [`zeng-guofan`](./.agents/skills/zeng-guofan/SKILL.md)

### Other Available Skills

- [`andy-grove`](./.agents/skills/andy-grove/SKILL.md)
- [`benjamin-franklin`](./.agents/skills/benjamin-franklin/SKILL.md)
- [`cao-cao`](./.agents/skills/cao-cao/SKILL.md)
- [`cao-dewang`](./.agents/skills/cao-dewang/SKILL.md)
- [`charlie-munger`](./.agents/skills/charlie-munger/SKILL.md)
- [`duan-yongping`](./.agents/skills/duan-yongping/SKILL.md)
- [`elon-musk`](./.agents/skills/elon-musk/SKILL.md)
- [`haruki-murakami`](./.agents/skills/haruki-murakami/SKILL.md)
- [`hayao-miyazaki`](./.agents/skills/hayao-miyazaki/SKILL.md)
- [`jack-ma`](./.agents/skills/jack-ma/SKILL.md)
- [`jeff-bezos`](./.agents/skills/jeff-bezos/SKILL.md)
- [`jensen-huang`](./.agents/skills/jensen-huang/SKILL.md)
- [`kazuo-inamori`](./.agents/skills/kazuo-inamori/SKILL.md)
- [`kobe-bryant`](./.agents/skills/kobe-bryant/SKILL.md)
- [`konosuke-matsushita`](./.agents/skills/konosuke-matsushita/SKILL.md)
- [`lee-kuan-yew`](./.agents/skills/lee-kuan-yew/SKILL.md)
- [`lei-jun`](./.agents/skills/lei-jun/SKILL.md)
- [`luo-xiang`](./.agents/skills/luo-xiang/SKILL.md)
- [`marcus-aurelius`](./.agents/skills/marcus-aurelius/SKILL.md)
- [`napoleon`](./.agents/skills/napoleon/SKILL.md)
- [`peter-drucker`](./.agents/skills/peter-drucker/SKILL.md)
- [`rafael-nadal`](./.agents/skills/rafael-nadal/SKILL.md)
- [`ray-dalio`](./.agents/skills/ray-dalio/SKILL.md)
- [`ren-zhengfei`](./.agents/skills/ren-zhengfei/SKILL.md)
- [`richard-feynman`](./.agents/skills/richard-feynman/SKILL.md)
- [`steve-jobs`](./.agents/skills/steve-jobs/SKILL.md)
- [`su-shi`](./.agents/skills/su-shi/SKILL.md)
- [`wang-xing`](./.agents/skills/wang-xing/SKILL.md)
- [`wang-yangming`](./.agents/skills/wang-yangming/SKILL.md)
- [`warren-buffett`](./.agents/skills/warren-buffett/SKILL.md)
- [`zhang-yiming`](./.agents/skills/zhang-yiming/SKILL.md)
- [`zhuge-liang`](./.agents/skills/zhuge-liang/SKILL.md)

See also:

- English backlog: [`docs/person-backlog.md`](./docs/person-backlog.md)
- Chinese backlog: [`docs/person-backlog.zh-CN.md`](./docs/person-backlog.zh-CN.md)

## How To Use

### 1. Browse skills

Open [`.agents/skills`](./.agents/skills) and choose a person.

### 2. Invoke a skill

Example:

```text
Use $zeng-guofan to analyze this situation and give me actionable advice.
```

### 3. Ask by scenario

Example prompts:

```text
Use $wang-yangming to help me stop overthinking and start acting.
Use $richard-feynman to help me learn this topic clearly.
Use $lei-jun to help me judge this product direction.
Use $duan-yongping to help me decide whether this opportunity is worth doing.
```

## How To Propose A New Skill

If you want to add a new person skill, use this simple path:

1. Pick a person with real source material.
2. Explain why ordinary people can use the method.
3. State the main use case.
4. List primary and secondary sources.
5. Open an issue or PR.

Start here:

- [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- [`CONTRIBUTING.zh-CN.md`](./CONTRIBUTING.zh-CN.md)
- [`docs/review-checklist.md`](./docs/review-checklist.md)
- [`docs/review-checklist.zh-CN.md`](./docs/review-checklist.zh-CN.md)

Recommended template files:

- [`templates/person-skill/SKILL.md`](./templates/person-skill/SKILL.md)
- [`templates/person-skill/references/source-map.md`](./templates/person-skill/references/source-map.md)
- [`templates/person-skill/references/principles.md`](./templates/person-skill/references/principles.md)
- [`templates/person-skill/agents/openai.yaml`](./templates/person-skill/agents/openai.yaml)

## Contribution Rules

Good contributions should be:

- source-based
- method-first
- modern and safe
- usable by AI

Please avoid:

- quote dumps
- myth-making
- fake sources
- unlawful, deceptive, or harmful advice

## Validation

Run this before opening a PR:

```bash
python3 scripts/validate_skills.py
```

## License

This repository is released under the [`MIT License`](./LICENSE).
