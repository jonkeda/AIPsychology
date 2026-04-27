# The AI Psychological Adaptation Cycle — Version 6

V6 is a descriptive-first rewrite of V5. The substantive shape of the model — states, axes, transitions — is preserved. What changes is framing, scope, and a small number of structural additions.

This file is the entry point. It is meant to be readable on its own in roughly five minutes. The supporting files hold the detail.

This model is a **speculative conceptual framework under construction**. The states and transitions are written as concrete descriptions to make the vocabulary usable and testable, not because they have been empirically validated. Validation is the next step; this document is the hypothesis. Everything marked **Conjecture —** is explicitly untested. Everything marked **Testable —** points at a study that could confirm or refute the claim. Everything without a marker is a well-grounded but unvalidated hypothesis.

## Scope

This model describes psychological adaptation to AI for **knowledge workers and creatives** who encounter AI *after* building a meaningful professional identity in their domain.

It applies when:

- The person's first substantive exposure to AI happens in adulthood.
- Identity is at stake because skill, expertise, or craft is being replicated by AI.
- The person has a viable economic position (the role can still exist in an AI-collaborative form, even if that form is uncertain). For people whose economic position is not viable, see [populations.md](populations.md) and [states/S3X-structural-displacement.md](states/S3X-structural-displacement.md).

It does **not** describe:

- AI-native users (first meaningful exposure before professional identity formed).
- Non-knowledge-work domains (manual work, physical care, service roles where AI is an economic threat but not an identity-replication threat).
- Emotional or relational AI use (companion apps, support tools, AI therapy).
- AI as assistive technology (users who rely on AI as an access tool, not as a productivity tool competing with an existing skill).
- Users facing permanent economic displacement through AI (see [populations.md](populations.md)).

These populations are not unimportant. They are out of scope because the model's vocabulary (identity-protection cognition, self-efficacy collapse, metacognitive calibration) is built around the identity-replication threat. Applying that vocabulary to people who face economic replacement without identity replication, or who have no professional identity yet invested in the domain, risks misdiagnosis.

## What kind of model this is

This model is **descriptive**. It provides:

- Names for recognisable psychological patterns.
- A graph of transitions between those patterns.
- Modulating factors that change how intensely a pattern is experienced.

It does **not** provide:

- Causal mechanisms. The Mechanism anchors indicate conceptual connections, not tested causes.
- Empirical predictions. Transition probabilities are not specified.
- Diagnostic instruments. No validated test places someone in a state.
- Treatment protocols.

A model can be useful without being empirically tested. This one offers vocabulary for conversations that previously had no shared language, a map for practitioners who are trying to orient themselves, and a set of hypotheses for future research. Until testing occurs, treat every state description as a well-grounded hypothesis, not an established fact.

The model describes observed paths, not recommended paths. It should not be used to push people through transitions faster, or to set a target state as a goal for someone. Its value is in helping practitioners understand where someone is, not in helping them engineer where that person goes next. The right outcome for any individual depends on their situation, domain, values, and economic position — not on reaching any particular state.

## What this model adds over prior frameworks

The state-graph structure (recognisable patterns with transition rules) appears in prior frameworks, notably the Technology Acceptance Model (Davis, 1989 — adoption is driven by perceived usefulness and perceived ease of use) and Diffusion of Innovations (Rogers — adoption depends on perceived compatibility with existing practice). What this model adds is **two modulating axes** that change the *intensity* of each state rather than which state a person is in:

1. **Identity Stakes** — how central the skill AI is replicating is to the person's professional self-concept. High stakes amplify every state; low stakes compress or skip the difficult ones.
2. **Task Delegation Level (D1–D4)** — how much cognitive authority the person hands to AI in a single interaction. D4 autonomous partnership in a high-stakes domain is the most psychologically activating combination.

These two axes are independent, **per-domain**, and **per-interaction**. They do not put people on a track; they change the texture of wherever they are.

A third property — **Delegation Ceiling** — describes the maximum delegation level a person can accept in their core domain given their history, separate from their current state. See [01-axes.md](01-axes.md).

For the relationship to TAM, Rogers, the Transtheoretical Model, the Gartner Hype Cycle, and prior versions of this model, see [00-relationship-to-prior.md](00-relationship-to-prior.md).

## How to read the claims in this model

Three levels of epistemic confidence appear throughout:

- **(no marker)** — an established or widely observed pattern with reasonable grounding in related literature.
- **Conjecture —** a claim the model makes because it is a useful frame, not because it is observed. Each conjecture is marked inline at the point it appears.
- **Testable —** a claim that could be falsified with a defined study. Marked inline; full notes in [limits-of-operationalization.md](limits-of-operationalization.md).

Everything the V5 limits-of-operationalization section listed as conjecture is still conjecture in V6. The reader does not need to reach the end of the document to know the model's epistemic status.

## Mechanism anchors are conceptual, not diagnostic

Each state in this model is connected to one or more concepts from psychology and adjacent fields. These connections are **vocabulary**, not **mechanism**. Knowing that S3E Ego Shock is conceptually related to self-efficacy collapse (Bandura) tells the reader what kind of phenomenon S3E belongs to. It does not let anyone diagnose S3E in a person, and it does not commit the model to the claim that self-efficacy collapse is the cause of S3E.

The model uses mechanism anchors to:

- Anchor each state in existing thinking, so the reader knows the construct is not invented from scratch.
- Provide a starting point for further reading.
- Make the conceptual content of each state legible to a reader with academic background.

The model does **not** use mechanism anchors to:

- Predict what a person will do.
- Identify which state a person is in.
- Claim a causal mechanism without empirical support.

## What this model is

Read it as three things stacked together:

1. **A vocabulary.** Names for recognisable patterns — Ego Shock, Bargaining, Maturity, Burnout. Once the names exist, two readers can say "she is in S2D Defensive Resistance about her writing but S5 Understanding about her email" and agree on what is meant.
2. **A graph of transitions.** Arrows that describe which states tend to follow which. These are tendencies, not laws.
3. **Two modulating axes.** Identity Stakes and Task Delegation Level change the intensity of whatever state the person is in.

What the model is **not**:

- Not a stage theory. People do not march from S1 to S7 in order. They loop, regress, and occupy multiple states at once across different domains.
- Not a diagnosis. No test places someone in a state.
- Not a value judgment. S7B Burnout and S3B Bargaining are not failures.
- Not a prescription. The model describes paths; it does not recommend them.

## States are per-domain

The model describes states of *a person in a specific domain*, not states of a whole person. Most people occupy several states at once across different domains. A senior craftsperson can be S2D Defensive Resistance about AI in their craft, S2T Trust Evaluation about AI for adjacent professional tasks, and S5 Understanding about AI for travel planning — all on the same day.

When using this model, the first question is *which domain are we talking about?*, not *which state are they in?*

## Regression and cycling

Regression is a property of every transition, not a destination. Any state in S5 Understanding through S7 can be pushed back to earlier states by changes in the AI environment. The triggers vary:

- **Capability changes.** A new model release that breaks the person's mental model. A capability jump in a domain the person had bounded. A high-profile AI failure that re-validates earlier fears.
- **Access and cost changes.** A price increase that makes the tools the person relied on unaffordable. Loss of access (the org pulls a tool, the API is deprecated, the seat is reassigned). A new tool the person cannot afford to evaluate.
- **Tooling shifts.** Better tooling that makes a previously closed domain feel newly relevant. Worse tooling that breaks a previously stable workflow.
- **Workplace changes.** New mandates, new managers, new peer groups, new performance metrics that change which AI uses are visible or rewarded.
- **Personal experience.** Being outperformed by a peer using AI. A failure that was caused by AI use the person had been confident in.

People cycle through the model more than once because the AI environment keeps changing, not because the person is unstable. Cycling is the model's expected behavior, not a deviation.

**Conjecture —** the claim that "most people cycle through the model more than once" remains qualitative. V6 makes no numerical claim about cycle frequency.

## Reading guide — files in this version

- [00-relationship-to-prior.md](00-relationship-to-prior.md) — TAM, Rogers, TTM, Gartner, V4/V5 lineage.
- [01-axes.md](01-axes.md) — Identity Stakes, Task Delegation Level, Delegation Ceiling.
- [02-state-graph.md](02-state-graph.md) — full state graph, occupancy rules.
- [states/](states/) — one file per state.
- [triggers.md](triggers.md) — external trigger layer, ⚡ rules.
- [social-context.md](social-context.md) — ambient field.
- [dropout.md](dropout.md) — two-axis dropout.
- [populations.md](populations.md) — out-of-scope populations and edge cases.
- [healthiness.md](healthiness.md) — interpretive layer mapping states to a sustainability frame.
- [usage.md](usage.md) — what the model is for and what it cannot be used for.
- [observation-guide.md](observation-guide.md) — concrete behavioral markers a practitioner can look for.
- [limits-of-operationalization.md](limits-of-operationalization.md) — what is testable, what is longitudinal-only, what is conjecture.
