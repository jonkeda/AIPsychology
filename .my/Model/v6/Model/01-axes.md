# Axes

The model uses two modulating axes and one per-domain ceiling property. All three change the *intensity* of each state; none of them move a person between states.

They operate at different levels:

| Property | Scope | What it captures |
| --- | --- | --- |
| **Identity Stakes** | Per-domain | How central the domain's skill is to self-concept |
| **Delegation Ceiling** | Per-domain | Maximum AI involvement the person can accept in that domain |
| **Task Delegation Level (D1–D4)** | Per-interaction | How much cognitive authority is delegated for one specific task |

## Axis 1 — Identity Stakes

A property of the person *relative to a domain*. The same person can have low stakes in one domain (using AI for travel planning) and high stakes in another (using AI for the craft they trained in for twenty years).

| Identity Stakes | Description | Effect on the model |
| --- | --- | --- |
| **Low** | Skill or role is not a core part of self-concept | Resistance and shock states (S2D, S3E, S3B) are weak or skipped |
| **High** | Skill or role is closely tied to identity (craft, expertise, profession) | Resistance and shock states are amplified and often unavoidable |

Conceptually related to **role-identity centrality** (the degree to which a role is central to the self-concept). Borrowed as vocabulary; high centrality is a plausible reason for threat appraisal under capability challenge, not a tested cause of any specific state.

Identity Stakes is **per-domain**, not per-person. The model's behavior in any given situation depends on which domain is in play.

**Measurement note:** Identity Stakes must be assessed independently of the outcome being explained. Assessing stakes after observing which fork a person took (S2T vs S2D) is circular — the fork is the outcome the stakes are supposed to predict. For stakes to function as a predictor, they must be measured before the observation: for example, years invested in the domain, proportion of income from it, or a short self-report interview administered before any AI interaction is observed. The validation protocol should operationalize Identity Stakes this way. The model flags this explicitly because post-hoc redeclaration of stakes is the main way the S1 fork prediction can be made unfalsifiable.

## Axis 2 — Task Delegation Level

A property of a single interaction. Defines how much cognitive authority is delegated for that task.

| Level | Example | Qualitative weight |
| --- | --- | --- |
| **D1. Information** | "Summarise this article" | Low — no identity engagement |
| **D2. Task execution** | "Write this email for me" | Moderate — skill relevance |
| **D3. Creative delegation** | "Draft this design / strategy / argument" | High — core identity engaged |
| **D4. Autonomous partnership** | "Make decisions with me" | Very high — agency at stake |

Qualitative experience of any state scales with both axes. V4 expressed this as the formula `intensity = baseline × Stakes × Delegation`. V5 removed the formula because the multipliers have no defined units. V6 keeps that decision: the qualitative anchor table under [S3E Ego Shock](states/S3E-ego-shock.md) is the operative claim.

The two axes are **independent**. A high-stakes person can operate at D1 (low intensity for that interaction) and at D4 (very high intensity for that interaction) on the same day.

## Delegation Ceiling

A property of the person **in a specific domain**, not of the interaction. The maximum Task Delegation Level a person can accept for AI involvement in that domain, given their current state and history. Like Identity Stakes, the Delegation Ceiling is per-domain — the same person can have a D1 ceiling in their core craft and a D4 ceiling in a low-stakes area.

| Ceiling level | Description |
| --- | --- |
| **D1** | Will accept AI only for information retrieval. Any task execution feels threatening. |
| **D2** | Will accept task execution but not creative delegation. |
| **D3** | Will accept creative delegation but not autonomous partnership. |
| **D4 (unbounded)** | No hard ceiling on delegation for AI in core domain. |

The Delegation Ceiling is **independent of state**. A person in S5 Understanding can still have a D2 ceiling if their prior S3E Ego Shock was severe. A person in S3B Bargaining can have a D3 ceiling for low-stakes domains while maintaining D1 for their core craft.

The ceiling is not fixed. It changes through:

- Sustained skill-building (seeing one's own contribution survive alongside AI).
- Readiness work (therapy, coaching, peer support).
- Natural ceiling shifts following capability exposure.

Forcing delegation beyond a person's current ceiling is the mechanism behind *coerced S5 Understanding* — the person appears to integrate but has not changed their ceiling; the underlying resistance re-surfaces later.

**Conjecture —** the Delegation Ceiling is a descriptive concept. No measurement instrument currently exists for it. The construct is offered as vocabulary for a phenomenon practitioners report but is not empirically validated.
