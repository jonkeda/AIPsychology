# Adoption Programme

An organisation wants people to use AI, expects productivity from it, and does not want to burn anyone out or waste money doing it. This document sets out how to approach that using the model, including the part where the model refuses the request as posed.

## The request and the problem with it

The request is usually some form of: *identify where people are, and move them to a better position.*

The model cannot support this, for reasons that are not merely procedural:

- **It is descriptive.** It names no target position. `IP` Integrated Practice: mastery is not the goal; it is one stable arrangement among several.
- **It is unvalidated.** Moving people according to an untested framework means acting confidently on something that may be wrong.
- **Positions are not levers.** A position is an outcome of a person's situation, history, and judgement. It is not a setting that can be changed directly, and attempting it produces compliance rather than change.

The last point is the practical one, and it is what makes the reframe below worth accepting rather than merely tolerating. **Programmes that target positions produce coerced calibration** — behaviour that looks like adoption while nothing underneath has changed. It measures as success and resurfaces later as disengagement, quality problems, or exit. Organisations that push hardest on position-shaped goals get the unravelling rollout most reliably.

## The reframe

**Target conditions, not positions.**

Conditions are the things an organisation actually controls. Positions are what emerge from them.

| Condition | Controlled by | Effect |
| --- | --- | --- |
| **Which tasks are delegated at which level** | Work allocation | Sets exposure to the high-stakes, high-delegation combination that is most activating |
| **Verification burden** | Workflow design | The strongest available predictor of the outcome nobody wants |
| **Incentive structure** | Management | Determines whether use is driven by judgement, throughput pressure, or visibility |
| **Whether delegation is mandated above what people accept** | Rollout design | The single largest cause of coerced calibration |
| **Whether skill-building is available** | Investment | The only legitimate route by which ceilings move |
| **Whether refusal is safe** | Culture | Determines whether any signal from the workforce is trustworthy |

Every one of these is measurable or observable without assessing anyone psychologically. A programme built on them needs no individual classification, which removes the legal exposure, the ethical problem, and the measurement contamination in one move.

**The reframe is not a compromise.** Conditions are where the leverage actually is. An organisation that fixes verification burden and incentive design will get more change than one that runs workshops aimed at moving individuals, and it will get change that lasts.

---

# The productivity question

## Being honest about what is known

The programme's premise is that AI use raises productivity. In software development this is less settled than the surrounding discourse suggests, and a programme built on an unexamined premise will measure the wrong thing.

What is reasonably clear: AI is strongly effective for well-specified, low-context, verifiable work. Boilerplate, tests against a clear specification, translation between formats, unfamiliar-syntax lookup, first drafts of routine code.

What is much less clear: whether it improves throughput on large, poorly-specified, high-context change in mature systems — which is where most engineering effort in an established organisation actually goes.

**The specific trap.** Time-to-first-draft improves dramatically and is easy to see. Time-to-merged-and-stable improves much less, and time spent on review, debugging unfamiliar generated code, and repairing subtle defects increases. A programme that measures the first and not the second will report a success that the organisation does not experience. This is not a hypothetical failure mode; it is the default outcome of measuring the easy thing.

## What to measure

Flow-level outcomes, never individual output.

| Measure | Why |
| --- | --- |
| **Change lead time** — commit to production | Captures the whole path, including review. Cannot be gamed by generating more code |
| **Change failure rate** | Catches quality degradation that volume metrics hide |
| **Time to restore** | Catches whether people can still debug what they shipped |
| **Review-to-production time ratio** | Direct instrumentation of verification burden. Rising ratio is the early warning |
| **Rework rate** — proportion of merged change revised soon after | The clearest signal that speed is being bought with defects |
| **Self-reported cognitive load, aggregated and anonymous** | The only sustainability signal that is not a lagging indicator |

**Measures to refuse, explicitly and in writing:**

- Lines of code, accepted suggestions, or generated volume. These measure activity and invert under quality pressure.
- Per-developer AI usage rates. Measuring this creates `OU` Overuse: mandate directly and destroys the signal it was meant to collect.
- Any per-individual productivity comparison. Every known attempt at this in software engineering has failed, and adding AI does not change that.

**The refusal matters as much as the selection.** If individual usage is tracked, people will use AI to make the number go up, and every subsequent measurement of adoption, satisfaction, or effectiveness becomes uninterpretable. This is worth stating to leadership in cost terms: tracking individual usage destroys the organisation's ability to know whether its investment is working.

---

# Sustainability

The failure mode is not that people refuse. It is that they comply, absorb the cost quietly, and leave.

## Verification burden is the control variable

The most useful single thing a programme can do is treat review capacity as a finite resource that is planned rather than assumed.

| Practice | Effect |
| --- | --- |
| **Instrument the review-to-production ratio** and treat a sustained rise as a workflow defect | Turns an invisible load into a tracked one |
| **Set an explicit review budget** — a stated share of the week beyond which review is not scheduled | Makes the constraint real rather than aspirational |
| **Rotate review-heavy work** | Prevents the load concentrating on the most senior and most conscientious people, which is its default distribution |
| **Design for sampled rather than exhaustive review** where the risk profile permits | The only structural answer once volume exceeds capacity |
| **Invest in automated verification before raising generation volume** | Tests, types, static analysis, and property checks shift verification from human attention to machine capacity. This is the highest-leverage sustainability investment available |

The last row is the important one. Raising generation capacity without raising verification capacity guarantees the burden lands on people. Most organisations do the first and not the second, then treat the resulting exhaustion as an attitude problem.

## Do not mandate a delegation level

Mandating exposure is defensible: *everyone should have used these tools on real work.* Mandating a delegation level is not: *all code review will be AI-assisted, all specifications will be AI-drafted.*

The difference is the ceiling. A person's acceptable delegation level in their core domain reflects their judgement about the work. Overriding it produces compliance without judgement — precisely the state in which mistakes stop being caught.

**A practical formulation:** mandate the floor, allow the ceiling to move on its own. Require that people try; do not require how far they go.

## Protect the high-stakes domains

The same rollout produces calm calibration in a low-stakes domain and acute disruption in a high-stakes one. Uniform rollouts to non-uniform stakes are the most common design error, and they are avoidable at no cost by sequencing.

**Start where stakes are low.** Not because it is easier, but because it builds a genuine evidence base about the tool's reliability that people can carry into the domains they care about. Someone who has watched the tool succeed and fail in a peripheral area has a real basis for judgement in a central one.

## Make refusal safe

If declining to use AI for a particular task carries a cost, three things follow immediately: nobody declines, the organisation learns nothing about where the tool is unsuitable, and every survey it runs returns enthusiasm.

A concrete version: an explicit, stated, senior-endorsed position that declining to use AI for a specific piece of work is a legitimate professional judgement requiring no justification. This is cheap and rarely done, and it is the precondition for any honest signal from the workforce.

## Watch for the specific patterns

| Pattern | Signal | Response |
| --- | --- | --- |
| Review load concentrating on a few people | Review-to-production ratio varies sharply across the team | Redistribute. This is a workflow problem |
| Quality drift with stable throughput | Rework and change failure rate rising | Verification capacity is exceeded. Reduce volume or automate checking |
| Usage high, complaints absent, engagement falling | Survey scores flat, attrition rising | Compliance without judgement. Check what was mandated |
| Senior people quietly disengaging | Reduced review participation, reduced technical opinion | Often the earliest signal of exceeded verification burden |
| One enthusiastic advocate, hardening team | Adoption stalling despite advocacy | Reduce the advocacy's prominence before addressing anyone's position |

---

# Cost efficiency

Token spend is a real constraint and it maps onto the model more cleanly than expected.

## Delegation level is the cost lever

The delegation axis and the cost axis are close to the same axis. D1 information retrieval is cheap. D5 objective delegation — an agent working autonomously over a long horizon — is expensive by orders of magnitude, and its cost is unbounded at the point of request.

**The core discipline: choose the delegation level deliberately, and default to the lowest that will do the job.** Most work is delegated at a higher level than it needs, because higher levels require less thought to initiate. This is simultaneously the largest available cost saving and a psychologically better default, since it keeps the person's judgement in the loop where it is needed.

This alignment is worth pointing out to leadership explicitly: the cost-efficient practice and the sustainable practice are the same practice.

## Practical measures

| Measure | Effect |
| --- | --- |
| **Match model capability to task** — cheap models for routine work | The largest single saving. Most requests do not need the most capable model |
| **Set the delegation level explicitly per task type** | Prevents defaulting to autonomous execution for work that needs a lookup |
| **Cap autonomous agent runs** by step count and spend | Bounds the worst case, which is otherwise unbounded |
| **Cache and reuse shared context** | Repeated codebase and standards context is a large share of spend |
| **Specify before delegating** | An underspecified request produces multiple expensive attempts. Specification cost is paid once |
| **Prefer deterministic tooling where it exists** | Formatters, linters, codemods, and generators are free and correct. Using a language model for work a deterministic tool does is pure waste |
| **Measure cost per merged change**, not cost per request | Aligns the cost measure with the outcome measure |

The last row prevents a specific failure: optimising for cheap requests by making many of them. Cost per merged change captures the whole path, in the same way lead time does for productivity.

## The false economy to avoid

Restricting access to capable models to save money, while continuing to expect the productivity gains that require them, produces frustration and worse outcomes at little saving. The saving available from **calibration** — using the right level and the right model per task — is much larger than the saving from **restriction**, and it does not carry the same cost in goodwill.

---

# Programme design

## Sequence

| Stage | Work | Why here |
| --- | --- | --- |
| **1. Instrument first** | Flow metrics and review-to-production ratio, before any adoption push | Without a baseline, no later claim about productivity is checkable |
| **2. Fix the incentives** | Remove individual usage tracking. State that refusal is safe. Confirm nothing enters performance processes | Every subsequent signal is uninterpretable until this is done |
| **3. Build verification capacity** | Automated checking, before generation volume rises | Prevents the burden landing on people |
| **4. Voluntary exposure, low stakes first** | Real work, low-stakes domains, no delegation-level requirement | Builds genuine judgement rather than compliance |
| **5. Support skill-building** | Time and space for people to find where the tool helps in their own domain | The only legitimate mechanism by which ceilings move |
| **6. Watch the sustainability signals** | Review ratio, rework, cognitive load, senior disengagement | Catches the failure before it becomes attrition |
| **7. Re-measure flow outcomes** | Against the stage-1 baseline | The only honest answer to whether it worked |

**Stage 1 is the one that gets skipped**, and skipping it means the programme can never demonstrate its own value. An organisation that cannot say what its lead time was before the programme cannot claim the programme improved it.

## What the programme reports

**Reports:** flow outcomes against baseline, review burden trend, cost per merged change, aggregated sustainability signals, and where the tooling turned out not to help.

**Does not report:** how many people are in each position, who is adopting and who is not, individual usage, or any per-person psychological characterisation.

The last item in the first list matters. A programme that only reports where AI helped is not credible and will not be believed by the engineers it depends on. **Reporting where it did not help is what makes the rest of the report trustworthy** — and the information is genuinely valuable, because it stops the organisation spending on cases that do not work.

## Where the model actually enters

Given all the above, the model's role is narrower than the original request assumed, and more useful than it sounds:

- **As vocabulary** for conversations about what is happening, which is most of its value.
- **As a design check** on the programme: has delegation been mandated above people's ceilings, is verification burden planned, do incentives reward volume over judgement, is refusal safe.
- **As a diagnostic for the environment**, not the individuals — the patterns table above.
- **As an early warning**, through verification burden, which requires no psychological assessment at all.

It does not enter as an assessment instrument, a targeting mechanism, or a progress measure. An organisation that wants those things should be told plainly that the model does not provide them, and that anything claiming to provide them about named employees should be treated as a liability.

## The honest summary for leadership

> The framework cannot tell the organisation where its people are, and should not be used to move them anywhere. What it can do is identify the conditions that determine how well an adoption programme goes — delegation level, verification burden, incentive design, and whether refusal is safe. Those are things the organisation controls, they can be measured without assessing anyone, and they are where the leverage is. A programme that fixes them will outperform one that targets individuals, and it will not create the legal and cultural exposure that individual assessment does.
