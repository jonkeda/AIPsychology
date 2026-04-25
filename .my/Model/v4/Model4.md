# The AI Psychological Adaptation Cycle — Version 4

A model of how people psychologically adapt to AI. Version 4 restructures Version 3 into an explicit **state machine** rather than a stage sequence, sharpens several state boundaries with observable markers, and tightens the axis system so each axis does exactly one job.

---

## Reading this model

**States, not stages.** The numbered labels (S1, S1.5, S2, …) are **identifiers**, not ordinals. They are short handles for memory and communication, like ticket numbers. Movement through the model is a **directed graph**: regression is a normal transition, not a failure, and several states are reachable directly without passing through their numeric predecessors. The number tells you *which* state, not *when* it happens.

**Two layers of intensity.** Every state's emotional intensity is modulated by two independent axes:

- **Identity Stakes** (low / high) — how much the person's self-concept depends on skills AI can replicate.
- **Task Delegation Level** (D1–D4) — how much cognitive authority is being handed to AI for a specific task.

Both are defined below before any state uses them.

**Triggers and ambient field.** External events and the surrounding social field shape transitions but are not states themselves. They are described in their own sections.

---

## Axis 1 — Identity Stakes

A property of the *person* relative to the *capability domain*. Replaces the earlier 1A/1B branching, which split a single state by hidden user attribute.

| Identity Stakes | Description                                                              | Effect on the model                                            |
| --------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------- |
| **Low**   | Skill or role is not a core part of self-concept                         | Resistance and shock states (S2, S3, S3B) are weak or skipped  |
| **High**  | Skill or role is closely tied to identity (craft, expertise, profession) | Resistance and shock states are amplified and often unavoidable |

A single person can have low stakes in one domain (using AI for travel planning) and high stakes in another (using AI for the craft they trained in for twenty years). Identity Stakes is per-domain, not per-person.

---

## Axis 2 — Task Delegation Level

A property of a *single interaction*. Defines how much cognitive authority is delegated for that task. Replaces V3's conflated "delegation depth," which mixed task-level and person-level meanings.

| Level                          | Example                                   | Intensity Multiplier            |
| ------------------------------ | ----------------------------------------- | ------------------------------- |
| **D1. Information**      | "Summarize this article"                  | Low — no identity engagement   |
| **D2. Task execution**   | "Write this email for me"                 | Moderate — skill relevance     |
| **D3. Creative delegation** | "Draft this design / strategy / argument" | High — core identity engaged   |
| **D4. Autonomous partnership** | "Make decisions with me"                  | Very high — agency at stake    |

Emotional intensity in any state = baseline × Identity Stakes × Task Delegation Level. A person at S3 (Ego Shock) with low stakes at D1 feels mild surprise. The same state with high stakes at D4 feels existential. The state is the same; the intensity is not.

**Optional extension — Adoption Ceiling.** If the model needs to represent users who are mature for low-delegation tasks but in shock for high-delegation tasks (a common real-world pattern), introduce **Adoption Ceiling** as a separate construct: the highest D-level the person is currently willing to operate at. State transitions are then driven by Adoption Ceiling movement; per-task intensity is driven by Task Delegation Level. V4 does not formalize Adoption Ceiling unless a use case requires it.

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
                  (low stakes)                    (high stakes)
                            │                          │
                  ┌─────────▼──────────┐     ┌─────────▼──────────────┐
                  │ S1.5 Trust         │     │ S2 Defensive Resistance│
                  │      Evaluation    │     └─────────┬──────────────┘
                  └─────────┬──────────┘               │
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
                            └─────────────►───────┴─────────┘
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

Back-edges (regression) are legal from every state and are not drawn. Practical Dropout is reachable from every state and is not drawn.

---

## States

### S0 — Baseline

*"AI is not a thing in my life right now."*

Not a stage but a baseline: the absence of meaningful encounter. Listed for completeness and as an entry point for the trigger layer.

**Exit:** any exposure event moves the person to S1.

---

### S1 — Initial Encounter

*"What is this thing?"*

First substantive contact. Stance is unformed. Emotional flavor (curiosity, skepticism, threat) depends on Identity Stakes, not on this state itself.

**Transitions:**

- → **S1.5 Trust Evaluation** — typical for low Identity Stakes
- → **S2 Defensive Resistance** — typical for high Identity Stakes
- → **S5 Understanding** — possible for low stakes with prior conceptual familiarity

⚡ Compressed by: workplace mandates, peer adoption, compelling demos.

---

### S1.5 — Trust Evaluation

*"Let me test this carefully before I commit."*

Rational, non-defensive assessment. Systematic testing on known problems, comparing AI output to personal output, evaluating reliability, calibrating expectations.

The numeric label `1.5` reflects that this state typically sits between Initial Encounter and the emotional branch (S2/S3). It is reachable directly from S1 without passing through S2.

**Entry from:**

- S1 (the common path for low Identity Stakes)
- S3B (after bargaining resolves into open evaluation)
- S5 (looping back to evaluate a new tool or model)

**Transitions:**

- → **S5 Understanding** — trust established
- → **S2 Defensive Resistance** — testing surfaces a threatening capability
- → **Practical Dropout** — fails quality or reliability standards

---

### S2 — Defensive Resistance

*"Fine, I'll try it — but I'm going to find flaws."*

Ego defense. Nitpicking, downplaying strengths, highlighting weaknesses. Identity protection, not objective evaluation. Subsumes V3's separate "Stage 1B Dismissal" — that was the same state at lower exposure.

**Transitions:**

- → **S3 Ego Shock** — defenses collapse under capability evidence
- → **S3B Bargaining** — defenses hold partially; person negotiates
- → **S1 Initial Encounter** — regression after a poor demonstration
- → **Practical Dropout** — the tool genuinely doesn't work for the person's workflow

⚡ Pushed to S3 by: a model release that overruns the current rebuttal.

---

### S3 — Ego Shock / Identity Disruption

*"If AI can do this… what does that make me?"*

The emotional core of the model. Anxiety, grief, fear of obsolescence, existential discomfort. Intensity scales with Identity Stakes and Task Delegation Level.

| Stakes × D-Level | Experienced as                                       |
| ---------------- | ---------------------------------------------------- |
| Low × D1         | Mild surprise — "It's useful"                       |
| Low × D4         | Curiosity tinged with vertigo                        |
| High × D2        | Discomfort — "It does this faster than me"          |
| High × D3        | Identity crisis — "It can do what I trained for"    |
| High × D4        | Existential — "What is my role now?"                |

**Transitions:**

- → **S3B Bargaining** — negotiate to reduce intensity
- → **S5 Understanding** — direct integration when the person can hold the full confrontation

⚡ Re-triggered from later states by: a capability jump, a junior colleague outperforming with AI.

---

### S3B — Bargaining

*"I'll use it — but only for X."*

Bounded adoption with self-imposed scope. A coping mechanism that defers full identity confrontation while allowing partial use. Not a failure state — many people remain productive here for years.

**Falsifiable marker (distinguishes S3B from S7A):**

> In S3B, boundaries are renegotiated **under capability pressure**. When a new model release crosses one of the self-imposed lines, the line moves reflexively (or the bargain collapses into S3). The trigger is pressure on the boundary itself, not new evidence of fit.

This is observable: watch what the person does in the week after a major model release. Reflexive line-moving → S3B. (Compare with S7A's marker.)

**Transitions:**

- → **S5 Understanding** — boundaries gradually recognized as artificial
- → **S3 Ego Shock** — capability jump shatters the bargain
- → **S2 Defensive Resistance** — failure validates the boundary, person retrenches

⚡ Primary destabilizer: model releases.

---

### S5 — Understanding

*"It's powerful, but it's still a tool. I can work with this."*

The first stable state. The person has a working mental model of what AI is and isn't, knows where human judgment matters, and prompts effectively.

Stability requires both:

- **Internal reframing** — personal mental model is coherent.
- **Social normalization** — surrounding environment treats AI use as unremarkable.

Mismatch between the two produces lingering discomfort even when the person is functionally adapted.

**Transitions:**

- → **S6A–6D Overuse states** — enthusiasm or pressure tips into excess
- → **S7A Maturity** — direct stabilization for measured adopters
- → **S7B / S7C / S7F** — direct stabilization into other end states
- → **S3 Ego Shock** — regression via external trigger

---

### S6A–S6D — Overuse States (parallel)

Promoted from V3 subtypes to first-class states because they have different drivers, antecedents, and exits. Not a single "Overcompensation" stage — four parallel post-Understanding states the person can fall into.

| State                     | Voice                                              | Driver                          | Typical exit                |
| ------------------------- | -------------------------------------------------- | ------------------------------- | --------------------------- |
| **S6A Enthusiastic** | "I want to use it for everything."                 | Dopamine, novelty               | → S7A or S7B              |
| **S6B Dependent**    | "I don't trust my own abilities anymore."          | Eroded confidence (from S3)     | → S3 (regression) or S7D  |
| **S6C Driven**       | "I must automate everything."                      | Productivity pressure           | → S7D                     |
| **S6D Social**       | "Everyone else is using it; I need to keep up."    | Peer pressure, FOMO             | → S5 (when pressure fades) or S7D |

A person can occupy more than one simultaneously (e.g., 6A + 6C is common in startup cultures).

⚡ Triggered or amplified by: workplace metrics, viral demos, peer-group adoption.

---

### S7 — End States (parallel, multiple-occupancy)

Long-term patterns. Not mutually exclusive — a person can occupy several at once and shift between them.

#### S7A — Maturity (Healthy Integration)

*"I know when to use AI and when not to."*

Bounded adoption with calibrated scope. Indistinguishable from S3B by behavior alone, distinguished by the marker below.

**Falsifiable marker (distinguishes S7A from S3B):**

> In S7A, boundaries are revised **only under evidence**. A new model release alone doesn't move the line; a measured outcome does — a benchmark, a real-world failure, a controlled comparison. The trigger is information, not pressure.

Test: in the week after a major model release, the person says some version of "interesting, I'll test it on three real tasks and decide." The line moves only after that testing — or doesn't move at all.

#### S7B — Identity Expansion

*"AI extends what I can be."*

The person develops capability or creative output they couldn't produce alone, and partly defines themselves through this expansion. Distinct from S7A: expansion is generative, maturity is stewardship.

#### S7C — Ethical / Philosophical Integration

*"What does AI mean for society, creativity, or humanity?"*

Sustained reflection on bias, intellectual property, authenticity, societal effects. Often co-occurs with S7A or S7B; rarely a sole end state.

#### S7D — Burnout / Withdrawal

*"I need a break from this."*

Step-back, temporary or permanent. A legitimate outcome, not a failure. Reachable from any S6 state and from sustained S7B/S7F intensity.

#### S7F — Influence / Evangelism

*"Let me show you what this can do."*

The person's identity becomes partly defined by their role as a guide for others' adoption: teaching, mentoring, advocacy, organizational leadership, community-building.

**Entry conditions.** Reachable from any other S7 state, but most stable when the person has previously passed through S3 (Ego Shock). Lived experience of the full cycle is the practical prerequisite for being credible to others going through it. S7F entered without prior S3 tends to collapse into S6A (enthusiasm without depth) or S6D (pressure-driven advocacy).

---

## Regression and the Loop Property

V3 listed "Stage 7E Regression Loop" alongside the end states. V4 removes it as a state — regression is a **property of every transition in the model**, not a destination.

Any state in S5–S7 can be pushed back to earlier states by:

- A major model release that breaks the current mental model
- A capability jump in a domain the person had bounded
- A high-profile AI failure that re-validates earlier fears
- A workplace change (new mandate, new role, new peers)
- A personal experience of being outperformed in a valued domain

Regression is normal. Most people cycle through the model more than once as AI evolves.

---

## External Trigger Layer

Discrete events that cause transitions. Distinct from the Social Context field below.

| Trigger              | Typical effect                                              |
| -------------------- | ----------------------------------------------------------- |
| Model release        | Forward push (S2 → S3) or regression (S5/S7 → S3)         |
| Workplace mandate    | Compresses S0–S2; can force S5 without S3                  |
| Media narrative      | Amplifies whichever state matches the narrative's framing  |
| AI failure (visible) | Regression from any state; reinforces S2                    |
| Regulatory change    | Freezes adoption or forces re-evaluation                    |
| Personal underperformance | Re-triggers S3 from any S5–S7 state                    |

---

## Social Context Layer (ambient field)

Continuous influences on transition probabilities. Distinct from External Triggers (which are events).

- **Social contagion** — peer behavior modulates transition rates. Adopting team collapses S2 duration; non-adopting environment makes S5 feel isolating.
- **Cultural framing** — techno-optimistic context compresses S1–S2; high-craft-identity context amplifies S2/S3/S3B.
- **Normalization** — slow social process distinct from individual understanding. S5 has both an internal (cognitive) and external (social) component; partial achievement of either produces partial stability.

A useful disambiguation rule: if it is an event with a date, it belongs in the External Trigger layer. If it is an ambient condition without a date, it belongs here.

---

## Dropout Mechanisms

People can exit the model from any state. Two distinct mechanisms:

### Emotional Dropout

Identity threat, ego shock, fear, or exhaustion. The person stops because using AI feels psychologically unsafe.

- Most common at S2, S3, S6B, S7D
- Mitigated by social support, gradual exposure, low-stakes initial tasks
- Often temporary

### Practical Dropout

Tool failures, workflow friction, bad outputs, prompt engineering fatigue, cost. The person stops because the tool doesn't work well enough.

- **Reachable from every state**, including S7A. A mature user whose tool degrades will leave for practical reasons.
- Mitigated by better tools, better training, better defaults
- Often permanent unless the tool improves materially

Confusing the two leads to wrong interventions: emotional dropout is not fixed by better documentation, and practical dropout is not fixed by psychological support.

---

## Cultural Variability

Core state structure holds across cultures; intensity, duration, and dominant flavor of each state shift.

- **High craft-identity cultures** (artisans, academics, literary traditions) — amplified S2, S3, S3B; bargaining often prolonged.
- **Techno-optimistic cultures** — compressed S1–S2; faster path to S5; harder hit at S6A/S6C.
- **Collectivist cultures** — Social Context layer dominates; S5's social-normalization component carries more weight than internal reframing.
- **Hierarchical work cultures** — workplace mandates override individual agency; S5 entered compliantly without S3, which can surface as delayed S3 later.
- **Economic-anxiety cultures** — S3 is primarily about job loss, not identity; the existential flavor differs.
