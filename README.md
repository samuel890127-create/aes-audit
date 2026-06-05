# AES Audit

AES Audit is a Codex Skill for screening early business ideas under one-person company constraints.

It is designed for people who are trying to find a first monetizable project and need a sober reviewer before building. It does not help make ideas sound better. It helps decide whether an idea deserves time, how to validate it fastest, and when to stop.

## What It Does

AES Audit reviews a business idea through:

- project normalization
- project shape classification
- red / yellow / green screening
- six universal questions
- optional expert lenses
- monetization priority scoring
- 7-30 day paid validation probability
- fastest validation action
- stop conditions

For one-person company, vibe coding, AI SaaS, micro-SaaS, and tool-first product ideas, it also applies a supplementary one-person execution lens: demand strength × one-person deliverability.

## Best For

- one-person company ideas
- AI tools and Skills
- micro-SaaS concepts
- content monetization ideas
- benchmark-derived opportunities
- local service experiments
- early product ideas before coding

## Not For

- writing a business plan
- making an idea sound investable
- encouraging every project
- replacing legal, tax, food safety, medical, financial, or compliance advice
- guaranteeing startup success

## Install

Copy the Skill into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R skills/business-project-screening ~/.codex/skills/
```

Restart Codex or open a new conversation if the Skill is not detected immediately.

## Usage

Use the Skill by name:

```text
Use $business-project-screening to judge whether this business idea is worth doing:
{your idea}
```

You can also use slash-style trigger text:

```text
/AESAudit
My project is: {your idea}
```

Chinese trigger examples:

```text
/项目审查
我的项目是：给餐饮门店做自动炒菜机器人
```

```text
/商业筛选
我的项目是：给初次创业小白提供项目筛选 Skill
```

For first-time users, see [AES Audit 新手使用文档](docs/beginner-usage-guide.md).

For the latest usability check, see [Skill 可用性测试报告](docs/skill-usability-test-2026-06-05.md).

## Output

The Skill returns:

- conclusion: continue / pause / stop
- one-sentence judgment
- monetization priority index
- 7-30 day paid validation probability
- red / yellow / green signals
- biggest false assumption
- fastest validation action
- success threshold
- stop condition

## Example

Input:

```text
/AESAudit
My project is: a mobile dessert cart in Beijing parks and markets, selling zongzi ice cream.
```

Expected review shape:

```text
Conclusion: pause original version, continue with a smaller validation.

Judgment:
The product has seasonal and impulse-purchase potential, but a mobile food cart is heavy for one-person validation. Test compliant pop-up sales and preorders before buying or building a cart.

Score:
- Monetization Priority Index: 55/100 for the original cart version
- 7-30 Day Paid Validation Probability: 35%-45%

Fastest validation:
Contact 3-5 market or park event organizers, confirm food stall entry requirements and costs, then test 30-50 preorder or sample sales.

Stop condition:
Stop if compliant entry is unclear, unit economics are weak, or fewer than 10 out of 50 target users show payment intent.
```

## Folder Structure

```text
aes-audit/
├── README.md
├── LICENSE
├── docs/
│   ├── beginner-usage-guide.md
│   └── skill-usability-test-2026-06-05.md
└── skills/
    └── business-project-screening/
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        └── references/
            ├── framework.md
            ├── solo-vibe-coding-project-screening.md
            └── templates.md
```

## License

MIT License.
