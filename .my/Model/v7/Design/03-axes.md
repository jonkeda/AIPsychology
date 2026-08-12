# Axes

Four properties modulate the model. None of them move a person between positions; all of them change what occupying a position is like, and three of them constrain which edges are available.

| Property | Scope | What it captures |
| --- | --- | --- |
| **Identity Stakes** | Per-domain | How central the domain's skill is to self-concept |
| **Delegation Level (D1–D5)** | Per-interaction | How much cognitive authority is handed over for one task |
| **Delegation Ceiling** | Per-domain | The highest Delegation Level the person can currently accept in that domain |
| **Verification Burden** | Per-workflow | How much of the work has become checking output rather than producing it |

The first three are carried over from V6, with Identity Stakes gaining a third level and Delegation gaining a fifth step. Verification Burden is new.

## Axis 1 — Identity Stakes

How much of the person's professional self-concept is invested in the domain whose skill AI is replicating.

V6 used two levels. Practitioners reported that most real cases sat between them, and the binary forced a choice that discarded information. V7 uses three.

| Level | Description | Effect on the model |
| --- | --- | --- |
| **Low** | The skill is incidental. The person could stop doing it tomorrow without disturbance to how they see themselves. | Disruption family is weak or skipped entirely. `FC` First Contact → `OE` Open Evaluation → `CU` Calibrated Use is the typical route. |
| **Moderate** | The skill matters professionally but is not core to self-concept. Losing it would be uncomfortable, not destabilising. | `OE` Open Evaluation more likely than `GE` Guarded Evaluation. If `IS` Identity Shock occurs it is milder and shorter. |
| **High** | The skill is central to professional identity — the thing the person is known for, trained in, or paid for. | Disruption family is amplified and frequently unavoidable. `GE` Guarded Evaluation likely. |

Conceptually related to **role-identity centrality** — the degree to which a role occupies a central place in the self-concept. Borrowed as vocabulary. High centrality is a plausible reason for threat appraisal under capability challenge; it is not a tested cause of any position.

### Measurement independence is mandatory

Identity Stakes must be assessed **before** any position is observed, and from evidence independent of the position.

This is not a methodological nicety. It is the difference between a model that predicts and a model that cannot be wrong. If stakes are inferred from the fact that someone ended up in `GE` Guarded Evaluation, and `GE` Guarded Evaluation is then explained by high stakes, the model has explained nothing and cannot be refuted.

Acceptable independent indicators, all collected before any position discussion:

| Indicator | Why it is independent |
| --- | --- |
| Years invested in the domain | Historical fact, fixed before the observation |
| Proportion of income from the domain | Structural fact |
| Depth of formal training | Historical fact |
| Whether the person is publicly known for the skill | Externally verifiable |
| Whether the person names the skill unprompted when describing their work | Elicited before AI is mentioned |

The protocol in [30-practitioner-use.md](30-practitioner-use.md) enforces this ordering. A stakes assessment made after a position assessment should be recorded as unusable.

## Axis 2 — Delegation Level

A property of a **single interaction**: how much cognitive authority was handed over for that specific task. The same person moves across the full range within a day.

| Level | Example instruction | What the person retains | Qualitative weight |
| --- | --- | --- | --- |
| **D1. Information** | "Summarise this document." | All judgement and all production | Low — no identity engagement |
| **D2. Task execution** | "Write this email." | Judgement; production is delegated | Moderate — skill relevance |
| **D3. Creative delegation** | "Draft the argument / the design / the strategy." | Final judgement only | High — core identity engaged |
| **D4. Autonomous partnership** | "Work through this with me and decide as we go." | Shared judgement, step-by-step visibility | Very high — agency at stake |
| **D5. Objective delegation** | "Achieve this outcome. Report when done." | The objective and the acceptance decision | Highest — authorship at stake |

**New in V7 —** D5 did not exist in V6, which topped out at partnership. D5 describes delegation where the person specifies an outcome and does not observe the process. It is qualitatively different from D4 in a way that matters psychologically: at D4 the person is present for the work and can locate their contribution in it. At D5 they cannot. What they retain is the objective and the decision to accept the result.

D5 has three consequences the model has to account for:

- **Authorship becomes ambiguous even to the person.** At D3 a person can point at what they did. At D5 the honest answer is "I decided this should exist and I decided it was good enough."
- **Verification replaces production as the work.** See Axis 4.
- **Responsibility and control separate.** The person remains accountable for output they did not observe being produced. **Conjecture —** this separation is the principal new stressor introduced by agentic tooling, and it is not captured by any V6 construct.

The two axes remain **independent**. A high-stakes person operates at D1 and D5 on the same day, in different domains and sometimes in the same one.

V4 expressed the interaction as `intensity = baseline × Stakes × Delegation`. V5 removed the formula because the multipliers have no units. V7 keeps it removed. The qualitative anchor tables under each position are the operative claim.

## Axis 3 — Delegation Ceiling

The highest Delegation Level the person can accept **in a specific domain**, given their history. A per-domain property of the person, not of the interaction.

| Ceiling | Description |
| --- | --- |
| **D1** | Information retrieval only. Any task execution in this domain feels like a concession. |
| **D2** | Task execution accepted; creative delegation refused. |
| **D3** | Creative delegation accepted; will not hand over decisions. |
| **D4** | Partnership accepted; will not accept unobserved work. |
| **D5 (unbounded)** | No hard ceiling in this domain. |

The ceiling is **independent of position**. A person in `CU` Calibrated Use can hold a D2 ceiling because an earlier `IS` Identity Shock was severe. A person in `SB` Scope Boundary can hold a D5 ceiling in peripheral domains while holding D1 in their core craft — that combination is close to the definition of `SB` Scope Boundary.

Ceilings move through sustained skill-building where the person's own contribution visibly survives alongside the tool, through readiness work, and through capability exposure that resolves rather than confirms a fear. They do not move because someone was told to move them.

**Forcing delegation above the ceiling produces coerced Calibrated Use** — the person's behaviour looks integrated while nothing underneath has changed. The pattern surfaces later as `GE` Guarded Evaluation, `OU` Overuse: mandate, or `BO` Burnout. This is the single most common way organisations manufacture the outcomes they were trying to avoid.

**Conjecture —** the ceiling is a descriptive construct with no measurement instrument. It becomes observable only at refusal events, which are rare and easily suppressed in environments where refusal is costly.

## Axis 4 — Verification Burden

**New in V7.** How much of the person's working time has become checking machine output rather than producing work.

V6 had no need for this axis. When output arrived one turn at a time and matched roughly what a person could produce in the time saved, verification was a step inside the task. When a system produces in an hour more than a person can carefully read in a day, verification becomes the task, and eventually stops being possible.

| Level | Description | Typical consequence |
| --- | --- | --- |
| **Incidental** | Checking is a minor step within producing. | None. |
| **Substantial** | A meaningful share of the working day is review. | Fatigue; reduced satisfaction; authorship questions begin. |
| **Dominant** | Most of the work is review. Production is delegated. | Loss of felt authorship; the `OL` Oversight Load position becomes available. |
| **Exceeded** | More output arrives than can be checked at the standard the person holds. | Forced choice: lower the standard silently, or refuse the volume. |

The **Exceeded** level is the important one, because it forces a choice with no acceptable option:

- **Rubber-stamping.** The person approves what they have not adequately checked. Quality degrades invisibly, and — the psychologically significant part — the person knows it. This is a distinct and corrosive experience that V6 could not name.
- **Refusal.** The person declines the volume, which reads as a productivity problem in any environment that measures throughput.
- **Withdrawal.** The person disengages from the responsibility, either by leaving the role or by ceasing to care about the output. Routes to `BO` Burnout or `DX` Disengagement.

**Conjecture —** Verification Burden at Exceeded is a stronger predictor of `BO` Burnout than raw usage volume. **Testable —** and it is one of the more tractable studies in the set, because verification time is measurable from workflow data without instrumenting the person. See [20-testing.md](20-testing.md).

### Why this is an axis and not a position

Verification Burden describes a workflow, not a person's stance. Two people with identical burden can hold very different positions: one in `IP` Integrated Practice: mastery who has designed the review process and finds it satisfying, one in `OL` Oversight Load who is drowning in it. The burden sets the conditions; the position describes the response.

## How the axes interact

Only a few combinations are worth naming. These are the ones that recur.

| Combination | What it produces |
| --- | --- |
| High Stakes + D4/D5 | The most activating combination in the model. Core identity engaged with no visible contribution to point at. |
| High Stakes + ceiling forced upward | Coerced `CU` Calibrated Use; later `GE` Guarded Evaluation, `OU` Overuse: mandate, or `BO` Burnout. |
| Low Stakes + any delegation | Little to nothing. Most AI use is here and generates no psychological content at all. |
| Any Stakes + Verification Exceeded | Routes toward `OL` Oversight Load; then `BO` Burnout or a silent standards collapse. |
| Moderate Stakes + D5 | **Conjecture —** the most under-described case. Not enough at stake to trigger `IS` Identity Shock, but enough that unobserved delegation produces a persistent low-grade unease with no name. |

The last row is the honest gap. The model was built around high stakes, where the phenomena are loud. Most of the working population is at moderate stakes, where the phenomena are quiet and the model has less to say.
