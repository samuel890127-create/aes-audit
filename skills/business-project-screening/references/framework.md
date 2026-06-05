# Business Project Screening Framework

## How The Traffic-Light Logic Works

Use red/yellow/green lights together, not as three separate scores.

1. Count red lights first. Red lights are hard risks.
   - 3 or more red lights: default to `stop`.
   - 1-2 red lights: default to `pause`, unless strong evidence offsets them.
   - 0 red lights: continue to yellow and green checks.
2. Use yellow lights to decide what must be shrunk.
   - Yellow lights do not mean the project is bad.
   - They identify the part that is too broad, too unclear, too heavy, or too untested.
3. Use green lights only to justify a small validation.
   - Green lights do not mean “build the full product.”
   - They mean the project deserves a 3-7 day test that can produce payment, rejection, deposit, appointment, or another high-intent signal.
4. Final conclusion still depends on the full picture:
   - `continue`: small paid validation is justified.
   - `pause`: shrink the project before testing.
   - `stop`: do not continue in the current shape.

## Count-To-Decision Mapping

Use this mapping as the default decision rule. Red lights have priority over yellow and green lights.

| Counts | Default conclusion | Meaning |
|---|---|---|
| Red >= 3 | `stop` | The current shape has too many hard risks. Do not continue without redefining the project. |
| Red 1-2 | `pause` | There are hard risks. Shrink or change the project before testing, unless strong evidence offsets them. |
| Red 0 + Yellow >= 5 | `pause` | No fatal hard risk, but the project is too broad, heavy, or unclear. Shrink aggressively. |
| Red 0 + Yellow 3-4 | `pause` | Testable only after narrowing user, scene, offer, price, or delivery. |
| Red 0 + Yellow 1-2 + Green >= 3 | `continue` | A small 3-7 day paid validation is justified. Do not build the full product yet. |
| Red 0 + Yellow 0 + Green >= 3 | `continue` | Strongest early-stage case, but still start with paid validation. |
| Green 0 | `pause` or `stop` | There is no positive validation basis. If red/yellow lights are also high, default to `stop`. |

When counts conflict, follow this priority:

```text
red count -> yellow count -> green count -> final conclusion
```

Always show the count of each light in the output, for example:

```text
Red lights（红灯）: 3
Yellow lights（黄灯）: 4
Green lights（绿灯）: 2
Count-to-decision（数量判定）: Red >= 3, so default conclusion is stop.
```

## Red Lights

If 3 or more red lights appear, default to `stop`. If 1-2 appear, default to `pause` unless strong facts offset them.

1. The user has no clear loss; it is merely "nice to have".
2. Existing alternatives are cheap, trusted, and good enough.
3. The payer is unclear, or monetization is only "ads, membership, B2B later".
4. A complete product must be built before demand can be tested.
5. The project needs heavy cold-start content, manual review, manual operation, or manual matching.
6. It needs high-density network effects, such as social matching, marketplaces, or local liquidity.
7. The founder must personally maintain information accuracy.
8. Acquisition depends mainly on viral content without payment or repeat behavior.
9. Users only like, save, or share, but do not pay, book, deposit, or submit high-intent signals.
10. Success depends on several uncertain events happening together.
11. A one-person founder cannot validate it within 7 days.
12. If usage grows 10x, work grows linearly instead of being absorbed by product, templates, automation, or partners.

## Yellow Lights

Yellow lights mean shrink the project until it becomes testable.

1. Demand exists, but the target group is too broad.
2. Users may use it, but payment reason is unclear.
3. Content may spread, but conversion path is unclear.
4. Product can be built, but acquisition is unclear.
5. Users may pay, but delivery is too heavy.
6. Competitors exist, but the founder cannot explain the advantage.
7. B2B buyers may exist, but no decision maker or budget scene is identified.
8. C users may like it, but use frequency is too low.
9. Long-term potential exists, but no 7-day validation exists.
10. The founder likes the direction, but external signals are weak.

Shrink by narrowing user, scene, deliverable, price, validation period, and offer.

## Green Lights

Green lights justify a 3-7 day validation, not a full build.

1. Users already use a clumsy workaround.
2. The problem creates money, time, relationship, emotional, or opportunity loss.
3. The project can be stated as: who, in what scene, lacks what, and pays for what.
4. A paid action can be designed within 7 days.
5. The first 10-30 users can be directly reached.
6. Delivery can become a template, checklist, workflow, partial automation, or repeatable service.
7. The result can trigger repurchase, referral, sharing, signup, visit, or transaction.
8. There is a clear disconfirming test.
9. The work creates data, methods, content, customer relationship, or reusable process assets.
10. Even failure improves the screening model or market understanding.

## Six Universal Questions

### Demand

Is the problem real, specific, recurring, and already being handled by the user? Strong demand usually has an existing workaround.

### Payment

Separate usage, recommendation, and payment. Payment needs a concrete reason: make money, save money, save time, reduce risk, secure a better experience, or improve identity/relationship outcomes.

### Alternative

The competitor may be a tool, spreadsheet, WeChat group, phone call, friend's advice, agency, or doing nothing. A new project must change the user's next real behavior, not merely organize information better.

### Reach

Do not use market size as early evidence. Ask whether the founder can reach 10-30 exact users and get a test, payment, appointment, or rejection.

### Delivery

A project can be valid but unsuitable for one person if every customer requires heavy conversation, custom work, support, maintenance, or field operation.

### Accumulation

Look for assets: method, data, content, customer relationships, industry understanding, tools, templates, or reusable delivery systems.

## Scoring

`Monetization Priority Index` totals 100:

| Dimension | Weight |
|---|---:|
| Paid problem strength | 20 |
| Payment path clarity | 15 |
| One-person execution efficiency | 20 |
| Acquisition testability | 15 |
| Productization potential | 10 |
| Differentiation and asset accumulation | 10 |
| Risk control | 10 |

Interpretation:

- 80-100: prioritize; usually requires real payment or strong reservation signals.
- 65-79: continue into a small experiment.
- 50-64: pause; shrink user, scene, or paid offer first.
- 0-49: stop unless new strong facts appear.

`7-30 Day Paid Validation Probability` estimates the chance of getting payment, deposit, paid reservation, or explicit commercial cooperation under current one-person constraints.

- 60-70%: strong access, sample, benchmark, or existing user signal; still capped before validation.
- 40-59%: direction clear but payment unproven.
- 20-39%: demand possible but acquisition, payment, or delivery uncertain.
- 0-19%: mostly imagined, or one-person validation is inefficient.

## Payment Signal Strength

Strong to weak:

1. Paid.
2. Deposit paid.
3. Price accepted and trial scheduled.
4. User submits information, invites others, or joins a serious test.
5. User adds contact for more discussion.
6. User likes, saves, comments "want".
7. User says "interesting".

Only 1-3 count as paid validation. 4 is strong intent. 5-7 are content feedback.

## Low-Efficiency Fantasy

A low-efficiency fantasy is a project that looks complete, scalable, or viral in imagination but consumes large amounts of time before proving payment.

Common forms:

- Treating market size as personal revenue.
- Treating user interest as payment.
- Treating viral content as business validity.
- Treating AI feasibility as demand.
- Treating competitor existence as proof that the founder can enter.
- Treating more features as more value.
- Treating "ads, membership, B2B later" as an early business model.
- Ignoring maintenance, support, updates, acquisition, and delivery cost.

## Shape-Specific Warnings

- Hardware: capital, supply chain, installation, maintenance, safety, and procurement cycles are often incompatible with early one-person validation.
- Two-sided marketplace: density and liquidity are the main risk, not feature completeness.
- Social/community: existing groups and habits are usually strong alternatives.
- Local information product: who maintains freshness is the core question.
- Agent product: sell workflow ROI, not agent novelty.
- Skill product: sell immediate judgment or output, not AI capability.
