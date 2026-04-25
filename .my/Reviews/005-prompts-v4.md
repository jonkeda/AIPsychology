# Review Prompt Proposals — Model4.md

A collection of prompts for soliciting reviews of [Model4.md](../Model/v4/Model4.md). Each prompt targets a different reviewer lens so the feedback set is diverse rather than redundant. Pick one, several, or run them in parallel against different LLMs / human experts.

V4 changes the vocabulary from V3 ("stages" → "states", S0/S1/S1.5/S2/S3/S3B/S5/S6A–D/S7A–F). Prompts below use V4 state labels. Where a prompt is inherited from [002-prompts-v3.md](002-prompts-v3.md), the V3 stage numbers have been remapped.

---

## Goal — Insights to Improve the Model

The prompts below are all aimed at the same outcome: *actionable improvements* to Model V4. They differ in **lens**, **rigor**, and **type of weakness** they tend to surface.

---

### Prompt A — Structural Critique (generalist reviewer)

> You are reviewing a descriptive psychological model called *The AI Psychological Adaptation Cycle (V4)*. V4 is presented as a state machine, not a stage sequence. Read it carefully and identify weaknesses in its **structure**: missing states, overlapping states, unclear transitions, axes that don't compose cleanly, end states that aren't actually distinct, or graph edges that are asserted but not justified. Pay particular attention to: (a) whether S1.5 earns its own identity vs. being a mode of S1, (b) whether the four S6 states are genuinely parallel or partially ordered, (c) whether S7A, S7B, and S7F are behaviorally distinguishable. For each issue, propose a concrete revision (rename, merge, split, reorder, add edge, remove edge). Do not comment on prose quality. Prioritize the 5 changes that would most improve the model's explanatory power.

**Best for:** finding taxonomy problems, redundancy, gaps.

---

### Prompt B — Falsifiability & Predictive Power

> Treat this model as a scientific hypothesis. For each state and transition, ask: *what observation would falsify this?* Identify claims that are unfalsifiable, tautological, or so flexible they explain every outcome post-hoc. Propose specific behavioral indicators or measurable signals that would let a researcher empirically distinguish:
>
> 1. **S2 (Defensive Resistance) from S1.5 (Trust Evaluation)** — both can look like "the user is testing the tool and finding flaws." What measurable signal separates ego defense from rational evaluation?
> 2. **S3B (Bargaining) from S7A (Maturity)** — the model itself flags these as behaviorally identical and offers a marker (line-moves under capability pressure vs. under measured evidence). Stress-test that marker: how would you operationalize it in a study? What confounds would defeat it?
> 3. **S6B (Dependent overuse) from S7D (Burnout / Withdrawal)** — both involve eroded confidence or fatigue. What distinguishes "I don't trust my own abilities" from "I need a break"?
> 4. **Emotional dropout vs. practical dropout** — the model insists confusing the two leads to wrong interventions. What instrument or interview protocol would reliably classify a real dropout case into one bucket?
>
> Where the model cannot be operationalized, say so directly. Don't invent plausible-sounding measures; flag the gap.

**Best for:** tightening definitions, exposing hand-waving, forcing operational rigor. **This is the highest-priority prompt for V4** because V4 explicitly added "falsifiable markers" to S3B and S7A — those markers should be the first thing a skeptical reviewer attacks.

---

### Prompt C — Adversarial / Steel-Man Critic

> You are a skeptical reviewer who believes stage-and-state models of psychological adaptation are usually folk-psychology dressed up as theory (compare with critiques of Kübler-Ross). V4 has rebranded "stages" as "states" and added a state-machine diagram. Make the strongest possible case that this is cosmetic — that V4 is V3 with new labels and the same underlying problems. Then, assuming the author wants to keep the model, list the minimum changes that would make your critique no longer apply. Specifically address: does calling something a "state machine" buy any explanatory power if the transition probabilities are never specified?

**Best for:** surfacing hidden assumptions, avoiding theoretical sloppiness, checking whether the V3→V4 changes are substantive.

---

### Prompt D — Missing Populations & Edge Cases

> Identify groups whose experience this model describes poorly or not at all. Consider at minimum: people who first encountered AI as children/teens, people in non-knowledge work (trades, manual labor, service), people with cognitive disabilities, people who use AI primarily for emotional/companionship purposes, AI researchers themselves, people economically dependent on *not* adopting AI (paid human-only services), and people who reject AI on ethical/religious grounds without ever passing through S2/S3. For each group, point to specific states or transitions that don't fit, and propose either (a) model extensions or (b) explicit scope limits the author should declare. Note: V4's Identity Stakes axis is per-domain — does that solve the multi-domain user problem, or just push it into the axis?

**Best for:** scope clarity, finding under-modeled segments.

---

### Prompt E — Mechanism Review (cognitive science lens)

> Review V4 from a cognitive-science / psychology-of-technology perspective. The model is largely *descriptive* — it names states but rarely specifies the underlying mechanism (cognitive dissonance? threat appraisal? self-efficacy collapse? identity-protection cognition?). For each state (S1 through S7F), name the most plausible mechanism from existing literature and the relevant construct (for example: Bandura's self-efficacy, Festinger's dissonance, terror management theory, technology acceptance model, Rogers' diffusion of innovations). Flag where V4 conflicts with or duplicates existing frameworks. Pay special attention to S3 (Ego Shock), which V4 calls "the emotional core of the model" — does it map cleanly to a single mechanism or is it a conflation? Recommend whether V5 should explicitly anchor each state to a mechanism.

**Best for:** grounding the model in established theory, avoiding reinvention.

---

### Prompt F — Practitioner Utility Review

> You are a manager, coach, or change-leader who would actually *use* V4 to help people adopt AI. Read it and answer: (1) Which states can I reliably *identify* in a real person from observable behavior in under one conversation? (2) Which transitions can I actually *influence*, and how? (3) Which parts of the model are interesting but operationally useless? (4) The model claims regression is "normal, not failure" — does that framing help or hurt me when reporting to leadership? (5) What is missing that I would need to make this a working diagnostic + intervention tool? Be blunt — favor utility over theoretical elegance.

**Best for:** turning theory into something usable.

---

### Prompt G — Internal Consistency Audit

> Audit V4 for internal contradictions, ambiguous transitions, and ill-defined terms. Specific checks:
>
> 1. **Multiple-occupancy claim.** S7 end states are explicitly multi-occupancy; S6 states "can occupy more than one simultaneously." Does the rest of the model support multi-occupancy? Can a person be in S6A and S7A at once? S3B and S7A?
> 2. **S1.5 entry points.** S1.5 is reachable from S1, S3B, and S5. Are the entry experiences described differently enough to justify one state, or is "Trust Evaluation" three different activities sharing a label?
> 3. **The two axes.** Identity Stakes (per-domain) and Task Delegation Level (per-interaction) are introduced as independent. Find any place in the state descriptions where they are treated as if one implies the other.
> 4. **Optional Adoption Ceiling.** V4 introduces this construct then refuses to formalize it. Does any state description quietly depend on it anyway?
> 5. **Trigger consistency.** ⚡ markers — are they applied consistently? Are there states with obvious external triggers that don't carry the marker?
> 6. **Regression as a property, not a state.** V4 removed V3's "Stage 7E Regression Loop." Does any text still treat regression as a destination?
>
> List every inconsistency with line-level references.

**Best for:** copy-edit-level rigor that catches real conceptual drift.

---

### Prompt H — Comparative Review

> Compare V4 directly to: (a) Kübler-Ross stages of grief, (b) the Technology Acceptance Model (Davis), (c) Rogers' Diffusion of Innovations, (d) the Transtheoretical Model of behavior change (Prochaska/DiClemente), and (e) the Gartner Hype Cycle (as applied to individuals rather than markets). For each: what does V4 borrow, what does it add that is genuinely new, and where does an existing model do the job better? V4's specific original claims appear to be (i) the Identity Stakes × Task Delegation Level intensity calculus, (ii) the falsifiable markers separating S3B from S7A, and (iii) the explicit emotional-vs-practical dropout split. Evaluate each. Recommend which V4 elements are original contributions worth keeping vs. which should be replaced by referencing the prior model.

**Best for:** establishing what's actually novel vs. derivative.

---

### Prompt I — Longitudinal / Dynamics Review

> V4 calls itself a state machine but is silent on *dynamics*: transition probabilities, dwell times, what determines transition speed, what typical multi-year trajectories look like, and how repeated cycles (regression) differ from first-pass cycles. The model says "most people cycle through the model more than once" — but never says how the second pass differs from the first. Propose what a V5 dynamics layer should specify, and identify the 3–5 dynamics questions whose answers would most change how the model is used. Also: does V4 actually need to be a state machine, or would a different formalism (Markov chain, dynamical system, agent-based) fit better?

**Best for:** moving from a static taxonomy to a process model.

---

### Prompt J — V3 → V4 Diff Review

> V4 is a revision of V3. Read both and evaluate the changes as a diff: (1) Renaming "stages" to "states" — substantive or cosmetic? (2) Promoting S1.5 (Trust Evaluation) out of the V3 emotional path. (3) Removing V3's Stage 1B Dismissal and folding it into S2. (4) Splitting V3's single "Overcompensation" into four parallel S6 states. (5) Adding falsifiable markers to S3B and S7A. (6) Removing V3's Stage 7E Regression Loop and recasting regression as a transition property. (7) Adding the Identity Stakes × Task Delegation Level intensity calculus. (8) Adding the dropout-mechanism split. For each change: was it an improvement, a lateral move, or a regression? Which V3 elements should have been changed but weren't? Which V4 changes should be reverted in V5?

**Best for:** evaluating whether V4 actually advanced the model or just rearranged it.

---

### Prompt K — One-Shot "Make It Better"

> Read V4. Propose the **single most impactful change** to V5 — exactly one change — and defend why it beats every other change you considered. Then list the next 4 runners-up in priority order with one sentence each.

**Best for:** forcing prioritization; useful as a tiebreaker after running other prompts.

---

## Suggested Workflow

1. Run **B** first. V4's headline claim is that it added falsifiable markers; if those don't survive scrutiny, the rest of V4 is decorative.
2. Run **J** second to check whether V4 actually advanced past V3 on substance.
3. Run **A**, **D**, and **G** in parallel — broad coverage with little overlap.
4. Run **E** and **H** if you want academic grounding before V5.
5. Run **F** if V5 is meant to be applied, not just published.
6. Run **K** last to force a prioritized synthesis across whatever feedback arrived.
