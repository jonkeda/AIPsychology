# The AI Psychological Adaptation Cycle — Version 5

A model of how people psychologically adapt to AI. V5 keeps V4's state-machine structure and inherits its two-axis modulation (Identity Stakes × Task Delegation Level). The substantive changes in V5 are:

- **Each state is anchored to an underlying cognitive-science mechanism** so the model is no longer purely descriptive.
- **The two-state fork after Initial Encounter is renamed** to remove V4's misleading "S1.5" ordinal.
- **The binary emotional-vs-practical dropout split is replaced** with two severity axes plus an operational test.
- **A "Limits of operationalization" section** marks which claims in the model are testable today, which require longitudinal data, and which are currently conjecture.
- **Several V4 claims are downgraded from "falsifiable" to "heuristic"** where the model lacks a workable measurement protocol.

V5 deliberately adds no new states, no new axes, and no numerical transition probabilities. Each construct still in the model has been kept because it earns its place on at least one of: explanatory power, operational use, or in-principle falsifiability.

---

## Reading this model

**States, not stages.** State labels (S0, S1, S2T, S2D, …) are **identifiers**, not ordinals. Movement through the model is a directed graph; regression is a normal transition.

**Two layers of intensity** modulate every state:

- **Identity Stakes** (low / high) — how much the person's self-concept depends on skills AI can replicate. A property of the *person relative to a domain*.
- **Task Delegation Level** (D1–D4) — how much cognitive authority is delegated for a single interaction. A property of the *interaction*.

Both are defined below before any state uses them. They modulate the *qualitative experience* of each state. V5 does not claim a numerical formula for intensity.

**Triggers and ambient field.** External events shape transition probabilities; the surrounding social field shapes transition rates. Both are described in their own sections.

**Mechanism anchors.** Each state is named with a description, then anchored to an underlying psychological mechanism from the existing literature. The anchor is not decoration — it tells the reader *why* the state behaves the way it does, and where to look for the failure modes.

---

## Axis 1 — Identity Stakes

A property of the person relative to a capability domain. A single person can have low stakes in one domain (using AI for travel planning) and high stakes in another (using AI for the craft they trained in for twenty years).

| Identity Stakes | Description                                                              | Effect on the model                                             |
| --------------- | ------------------------------------------------------------------------ | --------------------------------------------------------------- |
| **Low**   | Skill or role is not a core part of self-concept                         | Resistance and shock states (S2D, S3, S3B) are weak or skipped  |
| **High**  | Skill or role is closely tied to identity (craft, expertise, profession) | Resistance and shock states are amplified and often unavoidable |

Mechanism: **role-identity centrality** (the degree to which a role is central to the self-concept). High centrality predicts threat appraisal under capability challenge.

---

## Axis 2 — Task Delegation Level

A property of a single interaction. Defines how much cognitive authority is delegated for that task.

| Level                                | Example                                   | Qualitative weight            |
| ------------------------------------ | ----------------------------------------- | ----------------------------- |
| **D1. Information**            | "Summarize this article"                  | Low — no identity engagement |
| **D2. Task execution**         | "Write this email for me"                 | Moderate — skill relevance   |
| **D3. Creative delegation**    | "Draft this design / strategy / argument" | High — core identity engaged |
| **D4. Autonomous partnership** | "Make decisions with me"                  | Very high — agency at stake  |

Qualitative experience of any state scales with both axes. V4 expressed this as the formula `intensity = baseline × Stakes × Delegation`. V5 removes the formula because the multipliers have no defined units and the result is not measurable. The qualitative anchor table under S3 below is the operative claim.

The two axes are **independent**: a high-stakes person can operate at D1 (low intensity for that interaction) and at D4 (very high intensity for that interaction) on the same day.

---

## State map

```
                                 ┌──────────────┐
                                 │  S0 Baseline │
                                 └──────┬───────┘
                                        │ exposure
                                 ┌──────▼───────────────┐
                                 │ S1 Initial Encounter │
                                 └──────┬───────────────┘
                                        │
                          ┌─────────────┴────────────┐
                          │                          │
                  (low stakes)                (high stakes)
                          │                          │
                ┌─────────▼──────────┐     ┌─────────▼──────────────┐
                │ S2T Trust          │     │ S2D Defensive          │
                │      Evaluation    │     │      Resistance        │
                └─────────┬──────────┘     └─────────┬──────────────┘
                          │                          │
                          │                          ▼
                          │                  ┌────────────────┐
                          │                  │ S3 Ego Shock   │
                          │                  └───┬────────┬───┘
                          │                      │        │
                          │                      ▼        │
                          │              ┌──────────────┐ │
                          │              │ S3B Bargain  │ │
                          │              └──────┬───────┘ │
                          │                     │         │
                          └────────►────────────┴─────────┘
                                                │
                                        ┌───────▼────────┐
                                        │ S5 Understanding│
                                        └───┬────────────┘
                                            │
                        ┌───────────────────┼───────────────────┐
                        ▼                   ▼                   ▼
                  ┌──────────┐       ┌──────────┐       ┌──────────────┐
                  │ S6A–6D   │       │ S7A      │       │ S7B/7C/7F    │
                  │ Overuse  │       │ Maturity │       │ End states   │
                  └─────┬────┘       └────┬─────┘       └──────┬───────┘
                        │                 │                    │
                        └─────────────────┴────────────────────┘
                                          │
                                          ▼ (optional)
                                     ┌──────────┐
                                     │ S7D      │
                                     │ Burnout  │
                                     └──────────┘
```

Back-edges (regression) are legal from every state and are not drawn. Dropout is reachable from every state and is not drawn.

V5 renames V4's `S1.5 Trust Evaluation` and `S2 Defensive Resistance` to `S2T` and `S2D` respectively. Both are responses to S1; neither is sequentially "before" the other. Identity Stakes determines which fork the person takes.

---

## States

### S0 — Baseline

*"AI is not a thing in my life right now."*

Not a state in the active sense — the absence of meaningful encounter. Listed for completeness and as the entry point for the trigger layer.

**Mechanism anchor:** none (default condition).

**Exit:** any exposure event moves the person to S1.

---

### S1 — Initial Encounter

*"What is this thing?"*

First substantive contact. Stance is unformed. Emotional flavor (curiosity, skepticism, threat) depends on Identity Stakes, not on this state itself.

**Mechanism anchor:** **novelty appraisal** — the brain's first-pass classification of an unfamiliar stimulus as relevant or irrelevant, threatening or benign. Standard cognitive-appraisal terrain (Lazarus and Folkman's work on stress appraisal is the closest classical reference: people first decide *what is this and does it matter to me*, then decide *what can I do about it*).

**Transitions:**

- → **S2T Trust Evaluation** — typical for low Identity Stakes
- → **S2D Defensive Resistance** — typical for high Identity Stakes
- → **S5 Understanding** — possible for low stakes with prior conceptual familiarity

⚡ Compressed by: workplace mandates, peer adoption events, compelling demos.

---

### S2T — Trust Evaluation

*"Let me test this carefully before I commit."*

Rational, non-defensive assessment. Systematic testing on known problems, comparing AI output to personal output, evaluating reliability, calibrating expectations.

**Mechanism anchor:** **calibration under uncertainty** — the cognitive process of updating subjective probability estimates against observed evidence. Closely tied to the Technology Acceptance Model (Davis, 1989 — the idea that adoption is driven by perceived usefulness and perceived ease of use). S2T is the active testing of both perceptions.

**Entry from:**

- S1 (the common path for low Identity Stakes)
- S3B (after bargaining resolves into open evaluation)
- S5 (looping back to evaluate a new tool or model)

**Transitions:**

- → **S5 Understanding** — trust established
- → **S2D Defensive Resistance** — testing surfaces a threatening capability
- → **Practical-flavored Dropout** — fails quality or reliability standards

⚡ No external-event ⚡ marker: S2T is internally driven and is not reliably accelerated or reversed by named external events.

---

### S2D — Defensive Resistance

*"Fine, I'll try it — but I'm going to find flaws."*

Ego defense. Nitpicking, downplaying strengths, highlighting weaknesses. Identity protection, not objective evaluation. The behavior can look identical to S2T from outside; the difference is **asymmetric updating**: S2D discounts positive evidence and amplifies negative evidence.

**Mechanism anchor:** **identity-protection cognition** — the tendency to evaluate evidence in ways that defend a valued self-concept. Dan Kahan's term in the political-belief literature; the same mechanism applies to professional identity under capability threat. Festinger's cognitive dissonance (the discomfort of holding two beliefs that contradict each other) is the older and broader framing of the same dynamic.

**Transitions:**

- → **S3 Ego Shock** — defenses collapse under capability evidence
- → **S3B Bargaining** — defenses hold partially; person negotiates
- → **S1 Initial Encounter** — regression after a poor demonstration
- → **Practical-flavored Dropout** — the tool genuinely doesn't fit the workflow

⚡ Pushed to S3 by: a model release that overruns the current rebuttal.

---

### S3 — Ego Shock / Identity Disruption

*"If AI can do this… what does that make me?"*

The emotional core of the model. Anxiety, grief, fear of obsolescence, existential discomfort. Qualitative intensity scales with Identity Stakes and Task Delegation Level.

**Mechanism anchor:** **self-efficacy collapse** under domain-specific capability threat (Bandura's term — a person's belief that they can actually do the thing). When AI demonstrably performs a task the person built their self-concept around, the belief that "I can do this" no longer carries unique weight. A secondary mechanism is **terror management** in the loose sense — confrontation with one's own replaceability triggers the same kind of existential discomfort that confrontation with mortality does. The two mechanisms compound; S3 is rarely "just" one of them.

| Stakes × D-Level | Experienced as                                    |
| ----------------- | ------------------------------------------------- |
| Low × D1         | Mild surprise — "It's useful"                    |
| Low × D4         | Curiosity tinged with vertigo                     |
| High × D2        | Discomfort — "It does this faster than me"       |
| High × D3        | Identity crisis — "It can do what I trained for" |
| High × D4        | Existential — "What is my role now?"             |

**Transitions:**

- → **S3B Bargaining** — negotiate to reduce intensity
- → **S5 Understanding** — direct integration when the person can hold the full confrontation

⚡ Re-triggered from later states by: a capability jump, a junior colleague outperforming with AI.

---

### S3B — Bargaining

*"I'll use it — but only for X."*

Bounded adoption with self-imposed scope. A coping mechanism that defers full identity confrontation while allowing partial use. Not a failure state — many people remain productive here for years.

**Mechanism anchor:** **cognitive dissonance reduction via scope limitation** (Festinger). When the dissonance between "I am skilled at X" and "AI is also skilled at X" cannot be resolved by demoting AI, the person resolves it by demoting the scope of "X" — narrowing what they will use AI for so the remaining domain still belongs to them.

**Heuristic distinction from S7A.** S3B and S7A both look like "bounded adoption" from outside. The proposed distinguishing signal:

> In S3B, boundaries are renegotiated **under capability pressure**. When a new model release crosses one of the self-imposed lines, the line moves quickly without documented testing. In S7A, boundaries move **only after measured evidence** — a benchmark, a real-world failure, a controlled comparison.

This is a **heuristic**, not a measured fact. It requires longitudinal observation across multiple model releases, and is contaminated by self-report once a subject has read this model. See [Limits of operationalization](#limits-of-operationalization).

**Transitions:**

- → **S5 Understanding** — boundaries gradually recognized as artificial
- → **S3 Ego Shock** — capability jump shatters the bargain
- → **S2D Defensive Resistance** — failure validates the boundary; person retrenches

⚡ Primary destabilizer: model releases.

---

### S5 — Understanding

*"It's powerful, but it's still a tool. I can work with this."*

The first stable state. The person has a working mental model of what AI is and isn't, knows where human judgment matters, and prompts effectively.

**Mechanism anchor:** **schema integration** — the cognitive process by which a new tool is incorporated into existing mental models of work, rather than competing with them. Adjacent literature: Rogers' diffusion of innovations (the idea that adoption depends on the innovation's perceived compatibility with existing practice).

Stability has two components, both required:

- **Internal reframing** — personal mental model is coherent.
- **Social normalization** — surrounding environment treats AI use as unremarkable.

*Note: the dual-component requirement is currently conjecture. No instrument is specified for either component, and any observed discomfort can be attributed to mismatch. Treated here as a hypothesis to test, not a tested claim.*

**Transitions:**

- → **S6A–6D Overuse states** — enthusiasm or pressure tips into excess
- → **S7A Maturity** — direct stabilization for measured adopters
- → **S7B / S7C / S7F** — direct stabilization into other end states
- → **S3 Ego Shock** — regression via external trigger

---

### S6 — Overuse States (parallel)

Four parallel post-Understanding states with different drivers and different mechanism anchors. They are not phases of a single "Overuse" pattern; they are distinct attractors that pull from different upstream causes. A person can occupy more than one simultaneously — the most common combinations are S6A + S6C in startup cultures, and S6B + S6D in compliance-heavy cultures where the person feels both incompetent and surveilled.

All four states sit downstream of S5: a person who reached Understanding can still tip into excess. The exit from each is different, which is why they cannot be collapsed into a single state.

#### S6A — Enthusiastic Overuse

*"I want to use it for everything."*

Dopamine-driven experimentation. The person is energized, productive, and uncritical. Every workflow gets routed through AI even when it is the wrong tool for the task. Output volume goes up; output quality varies.

**Mechanism anchor:** **variable-reward reinforcement** — the intermittent-reward dynamic that underlies compulsive engagement with any tool whose outputs are unpredictably good. Sometimes the AI produces something exceptional, sometimes mediocre; the unpredictability is what sustains the behavior. Same construct that explains slot-machine engagement, social-media checking, and casual-game hooks.

**Transitions:**

- → **S7A Maturity** — the enthusiasm settles as the person learns where the tool fails
- → **S7B Identity Expansion** — the enthusiasm channels into a new generative identity
- → **S7D Burnout** — sustained high engagement depletes the person
- → **S5 Understanding** — mild regression after a sobering failure

⚡ Amplified by: viral demos, leaderboards, internal AI-usage metrics.

#### S6B — Dependent Overuse

*"I don't trust my own abilities anymore."*

The person uses AI as a crutch because S3 (Ego Shock) eroded their confidence in their own judgment. Surface behavior looks like S6A (high usage volume) but the affect is different — anxiety rather than enthusiasm. The person checks AI output against AI rather than against their own thinking.

**Mechanism anchor:** **self-efficacy displacement** — confidence in the AI replaces, rather than supplements, confidence in self. Bandura's construct in reverse: instead of mastery experiences building self-efficacy, repeated outsourcing erodes it. Each successful AI completion is silent evidence that the person's contribution wasn't necessary.

**Transitions:**

- → **S3 Ego Shock** — regression when the person realizes how much they have outsourced
- → **S7D Burnout** — dependence becomes exhausting to maintain
- → **S7A Maturity** — rare but possible when the person rebuilds independent judgment alongside AI use

⚡ No external-event ⚡ marker: S6B is internally driven and inherits its trigger from the upstream S3 episode rather than from any current event.

#### S6C — Driven Overuse

*"I must automate everything."*

Productivity-pressure-driven, not emotion-driven. Common in high-performance work cultures and among individuals with strong achievement orientation. The person uses AI not because they enjoy it (S6A) or because they doubt themselves (S6B), but because not using it feels like leaving performance on the table.

**Mechanism anchor:** **goal-substitution** — efficiency, originally a means to other goals (more output, better life balance, career advancement), becomes a terminal goal in itself. Adjacent literature: the cognitive-psychology work on goal hierarchies and the documented tendency of subgoals to displace the superordinate goals they were meant to serve.

**Transitions:**

- → **S7D Burnout** — the typical exit; there is no natural ceiling on "more efficient," so the person runs until depleted
- → **S7A Maturity** — if a structural change (new role, new manager, illness) forces re-evaluation

⚡ Triggered or amplified by: workplace AI-usage metrics, productivity-tracking rollouts, performance-review changes that explicitly reward AI use.

#### S6D — Social Overuse

*"Everyone else is using it; I need to keep up."*

Peer-pressure-driven adoption that exceeds the person's actual need or interest. Distinct from S6A (which is internally enthusiastic) and S6C (which is internally driven by productivity goals). The person here is following a perceived norm, not a personal goal.

**Mechanism anchor:** **normative social influence** — behavior change driven by the desire to match peer behavior, independent of personal evaluation of the behavior's merit. Asch's classic conformity work is the canonical reference; the modern variant is the documented tendency of professionals to adopt tools their peers visibly use even when their own work doesn't require them.

**Transitions:**

- → **S5 Understanding** — the typical exit when peer pressure fades or the person changes context
- → **S7D Burnout** — if the pressure persists past the person's capacity
- → **S6A** — occasional drift when external pressure converts into internal enthusiasm

⚡ Triggered by: peer-group adoption shifts, leadership announcements, industry-wide adoption events.

---

### S7 — End States (parallel, multiple-occupancy)

Long-term patterns. Not mutually exclusive — a person can occupy several at once and shift between them. Most adapted users settle into a combination (S7A + S7C is common among reflective practitioners; S7B + S7F is common among creative leaders).

Unlike S6, the S7 end states are not failure modes. They are different stable answers to the same underlying question: *what role does AI play in my life and identity now that the dust has settled?*

#### S7A — Maturity (Healthy Integration)

*"I know when to use AI and when not to."*

Bounded adoption with calibrated scope. The person has a clear internal model of where AI helps and where it does not, and routes work accordingly. Behaviorally similar to S3B (both look like "uses AI for some things, not others"), distinguished by the heuristic described under S3B: S7A boundaries move only on measured evidence; S3B boundaries move under capability pressure.

**Mechanism anchor:** **metacognitive calibration** — accurate self-assessment of when one's own judgment is better than the tool's. The mature user has an internal model of the tool's failure modes (where it hallucinates, where it sycophants, where it confidently averages out the interesting answer) and routes work to avoid those modes. Adjacent literature: the long line of research on calibration of confidence with accuracy (Lichtenstein and Fischhoff, and the modern decision-science extensions).

**Transitions:**

- → **S3 Ego Shock** — regression when a capability jump invalidates the calibration
- → **S7B / S7C / S7F** — lateral shift; S7A often co-occurs with these rather than transitioning out
- → **Practical-flavored Dropout** — even mature users leave when the tool degrades

⚡ Re-triggered by: model releases that move capability past the person's calibrated boundaries.

#### S7B — Identity Expansion

*"AI extends what I can be."*

The person develops capability or creative output they couldn't produce alone and partly defines themselves through this expansion. Distinct from S7A: S7A is stewardship of an existing identity; S7B is the construction of a new one. A novelist who uses AI carefully to polish their voice is in S7A; a person who couldn't write fiction before AI and now identifies as a writer-with-AI is in S7B.

**Mechanism anchor:** **extended-self / tool incorporation** — the documented tendency of humans to incorporate tools into their self-concept. The carpenter and the hammer; the writer and the typewriter; the photographer and the camera. With AI the integration is deeper because the tool participates in cognition rather than just executing it, which is why the identity claim feels different from "I'm good with Photoshop." Adjacent literature: Belk's work on the extended self in consumer behavior; the broader phenomenology-of-technology literature on tool-self continuity.

**Transitions:**

- → **S7D Burnout** — when the expansion outpaces sustainable effort
- → **S3 Ego Shock** — regression if a capability jump makes the person's contribution feel removable
- → **S7F Evangelism** — lateral shift when the new identity becomes generative for others

⚡ Re-triggered by: capability jumps in the person's expanded domain, particularly ones that automate parts of what felt like the person's contribution.

#### S7C — Ethical / Philosophical Integration

*"What does AI mean for society, creativity, or humanity?"*

Sustained reflection on bias, intellectual property, authenticity, labor displacement, environmental cost, societal effects. The person remains a user (this is not a refusal state) but the use is accompanied by ongoing ethical work — deciding what to use AI for and what to keep human, often making those decisions visible to others.

Rarely a sole end state. Most often co-occurs with S7A (mature use plus reflective stance) or S7B (expansion plus reckoning with what was expanded). When it appears alone, the person typically uses AI minimally and treats engagement with the technology as primarily a thinking subject.

**Mechanism anchor:** **meaning-making** — the broader cognitive process of integrating a personally significant experience into a coherent worldview. Adjacent literature: post-traumatic growth research, which documents that confrontation with destabilizing experience can yield a more articulated worldview rather than a return to the prior state. The same mechanism applies in non-traumatic contexts when an experience is large enough to require reorganization of existing beliefs.

**Transitions:**

- → **S7A** — the reflective stance settles into stable practice
- → **S7F Evangelism** — the reflection becomes externally directed
- → **S2D Defensive Resistance** — rare; the reflection concludes that prior adoption was a mistake and the person retrenches

⚡ No external-event ⚡ marker: S7C is internally driven. Triggers exist (a public AI ethics incident, a personal moral dilemma) but they amplify rather than create the state.

#### S7D — Burnout / Withdrawal

*"I need a break from this."*

Step-back from AI use, temporary or permanent. Reachable from any S6 state and from sustained S7B or S7F intensity. A legitimate outcome, not a failure. Some users return after weeks or months at lower intensity; some don't return at all.

Distinguishable from emotional dropout (see [Dropout — Two Severity Axes](#dropout--two-severity-axes)) by trajectory: S7D follows a period of high engagement; emotional dropout often happens earlier, before significant engagement was ever achieved.

**Mechanism anchor:** **resource depletion** in the cognitive-control sense — sustained high-effort engagement (whether enthusiastic in S6A, anxious in S6B, driven in S6C, or socially compelled in S6D) draws on finite regulatory resources. When depletion crosses a threshold, withdrawal restores the resource. Adjacent literature: the cognitive-control fatigue research and the broader burnout literature in occupational psychology (Maslach), allowing for the unresolved debate about whether "depletion" is a literal energy mechanism or a motivation shift.

**Transitions:**

- → **S5 Understanding** — return after recovery, often at lower intensity
- → **S7A Maturity** — return with newly calibrated scope
- → **Dropout** — the withdrawal becomes permanent

⚡ Triggered or accelerated by: workload spikes, organizational changes, personal life events that consume the same regulatory budget.

#### S7F — Influence / Evangelism

*"Let me show you what this can do."*

The person's identity becomes partly defined by their role as a guide for others' adoption: teaching, mentoring, internal advocacy, public writing, conference speaking, community-building. Distinct from S7A and S7B in that the locus of meaning is *external* — helping others through the cycle is what makes the role coherent for the person.

Most stable when the person has previously passed through S3. Lived experience of Ego Shock is what makes them credible to others currently in it; without that experience, the advocacy tends to be naive (S6A flavor) or compelled (S6D flavor) and collapses under the first hostile question.

**Mechanism anchor:** **generativity** (Erikson's term, broadened from its original developmental-stage context — the drive to invest in the next cohort's success). The same mechanism that explains why senior practitioners across many domains turn to mentoring and teaching once their own competence is settled. AI provides an unusually sharp opportunity for this because the cohort needing guidance is large and the experience required to guide them is a few years rather than a few decades.

*Note: the "S3 prerequisite for stable S7F" claim is currently conjecture. A future longitudinal study could refute it by documenting stable S7F users who never passed through identity-disruptive AI experiences.*

**Transitions:**

- → **S7D Burnout** — evangelism is high-effort; sustained advocacy depletes
- → **S6A or S6D** — collapse when the S3 prerequisite is missing
- → **S7A** — the external role recedes back into private mature practice

⚡ Re-triggered by: external demand for guidance (organizational AI rollouts, public discourse shifts, requests for talks).

---

## Regression and the Loop Property

Regression is a **property of every transition**, not a destination. Any state in S5–S7 can be pushed back to earlier states by:

- A major model release that breaks the current mental model
- A capability jump in a domain the person had bounded
- A high-profile AI failure that re-validates earlier fears
- A workplace change (new mandate, new role, new peers)
- A personal experience of being outperformed in a valued domain

Regression is normal. Most people cycle through the model more than once as AI evolves.

*Note: "more than once" is qualitative. V5 deliberately avoids numerical claims about cycle frequency. See [Limits of operationalization](#limits-of-operationalization).*

---

## External Trigger Layer

Discrete events that change transition probabilities. ⚡ markers in state descriptions point to the most common trigger types per state. The marker rule:

> A state carries ⚡ if and only if at least one named external event materially changes the probability of entering or leaving that state. States that change only through internal cognition or ambient social context do not carry ⚡.

| Trigger                   | Typical effect                                            |
| ------------------------- | --------------------------------------------------------- |
| Model release             | Forward push (S2D → S3) or regression (S5/S7 → S3)      |
| Workplace mandate         | Compresses S0–S2D; can force S5 without S3               |
| Media narrative           | Amplifies whichever state matches the narrative's framing |
| AI failure (visible)      | Regression from any state; reinforces S2D                 |
| Regulatory change         | Freezes adoption or forces re-evaluation                  |
| Personal underperformance | Re-triggers S3 from any S5–S7 state                      |

---

## Social Context Layer (ambient field)

Continuous influences on transition rates. Distinct from External Triggers (which are events).

- **Social contagion** — peer behavior modulates transition rates. Adopting team compresses S2D duration; non-adopting environment makes S5 feel isolating.
- **Cultural framing** — techno-optimistic context compresses S1–S2D; high-craft-identity context amplifies S2D, S3, and S3B.
- **Normalization** — slow social process distinct from individual understanding. S5 has both an internal (cognitive) and external (social) component.

Disambiguation rule: dated event → External Trigger layer. Undated ambient condition → Social Context layer.

---

## Dropout — Two Severity Axes

V4 split dropout into two categories: emotional and practical, with a warning that confusing them leads to wrong interventions. V5 keeps the distinction but replaces the binary categorization with **two independent severity axes**, because most real dropouts are mixed (a tool failure that happens to land in an identity-vulnerable spot).

A dropout is characterized by two scores:

- **Practical severity (0–10)** — the degree to which tool failures, workflow friction, bad outputs, prompt fatigue, or cost drove the exit.
- **Emotional severity (0–10)** — the degree to which identity threat, ego shock, fear, or exhaustion drove the exit.

A dropout is not a single point on one axis but a position on the plane.

| Region                          | Description                                         | Intervention                                                        |
| ------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------- |
| High practical / low emotional  | Tool genuinely doesn't work for them                | Better tools, training, defaults                                    |
| Low practical / high emotional  | Identity threat or exhaustion                       | Psychological support, gradual re-exposure, social context shift    |
| High practical / high emotional | Mixed — tool failed in an identity-vulnerable spot | Both interventions; address tool first to clear the rationalization |
| Low / low                       | Boredom, indifference, opportunity cost             | Often not worth intervening                                         |

**Operational test (the reversibility check).** Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit even if the cited reason was practical. This is the closest thing the model has to a clean operationalization of the dropout space.

**Mechanism anchors:**

- Practical severity → **expectancy violation** in the usability sense. The tool failed to do what its perceived capability promised.
- Emotional severity → **threat-driven avoidance**. Continuing use predicts further psychological cost, so the person stops.

Dropout is reachable from **every state**, including S7A. Severity scores are independent of which state the person dropped from.

---

## Cultural Variability

Core state structure is hypothesized to hold across cultures; intensity, duration, and dominant flavor of each state shift.

- **High craft-identity cultures** (artisans, academics, literary traditions) — amplified S2D, S3, S3B; bargaining often prolonged.
- **Techno-optimistic cultures** — compressed S1–S2D; faster path to S5; harder hit at S6A/S6C.
- **Collectivist cultures** — Social Context layer dominates; S5's social-normalization component carries more weight than internal reframing.
- **Hierarchical work cultures** — workplace mandates override individual agency; S5 entered compliantly without S3, which can surface as delayed S3 later.
- **Economic-anxiety cultures** — S3 is primarily about job loss, not identity; the existential flavor differs.

*Note: this entire section is currently conjecture. No cross-cultural data has been gathered. A finding that would force structural revision: a culture in which stable S7A users routinely enter directly from S0 without passing through S1 — that would refute the model's required initial-encounter path. Until such data exists, treat the cultural section as a working frame, not as a tested claim.*

---

## Limits of operationalization

This section makes explicit which parts of the model are testable today, which require longitudinal data, and which are currently conjecture. It exists to prevent the model from being read as more empirically grounded than it is.

### Snapshot-observable

These states or distinctions can be classified from a single observation of behavior or usage telemetry.

- **S0 vs everything else** — has the person had meaningful AI exposure?
- **S6A vs S7D** — usage volume distinguishes them trivially (high vs near-zero).
- **D-level of a specific interaction** — observable from the interaction itself.

### Longitudinal-only

These distinctions require repeated observation, typically across model releases or workflow changes.

- **S2T vs S2D** — both look like "user testing the tool" in a snapshot. Asymmetric updating on positive evidence is the operative signal, only visible across multiple evaluations.
- **S3B vs S7A** — the heuristic in S3B requires watching boundary-movement behavior across multiple model releases. Single-release observation is not enough.
- **S6B trajectory** — distinguishing "S6B currently" from "S6B that collapsed into S7D" requires usage timeseries.

### Self-report or interview only

These states cannot be directly observed and must be inferred from the person's own account, with all the contamination that implies.

- **S3 vs S5** with similar surface behavior — internal state matters.
- **S7B vs S7A** — both look like "uses AI competently." Identity expansion is internal.
- **S7C** — reflective stance is unobservable without dialogue.
- **The driver of a dropout** — practical severity and emotional severity per the two-axis split.

### Currently conjecture (not testable as written)

These claims are in the model because they are useful frames, not because they are tested. Each is marked above with an inline note. Listed here for completeness:

- The dual-component stability requirement for S5 (internal reframing + social normalization).
- The S7F-without-S3 collapse claim.
- "Most people cycle through the model more than once."
- The Cultural V	ariability section in full.

A future version may upgrade these from conjecture to tested claims if data is gathered. Until then, they should not be cited as model predictions.

### Deliberately not in V5

- **Numerical transition probabilities and dwell times.** Adding fabricated numbers is worse than admitting they don't exist. A future version may add them once data justifies it.
- **An "Adoption Ceiling" construct.** V4 introduced this as an optional extension. V5 removes the option. If a use case requires it, that use case justifies V6.

---

## What V5 deliberately does not do

- It does not number states ordinally. Identifiers are handles, not orderings.
- It does not provide a numerical intensity formula.
- It does not claim the cultural section is empirically grounded.
- It does not introduce new states, axes, or end states beyond V4.
- It does not pretend the S3B/S7A heuristic is a measured falsifier.
