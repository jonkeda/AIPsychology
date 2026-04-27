# Review Prompt Proposals — Model3.md

A collection of prompts for soliciting reviews of [Model3.md](../Model/Model3.md). Each prompt targets a different reviewer lens so the feedback set is diverse rather than redundant. Pick one, several, or run them in parallel against different LLMs / human experts.

---

## Goal 1 — Insights to Improve the Model

The prompts below are all aimed at the same outcome: *actionable improvements* to Model v3. They differ in **lens**, **rigor**, and **type of weakness** they tend to surface.

---

### Prompt A — Structural Critique (generalist reviewer)

> You are reviewing a descriptive psychological model called *The AI Psychological Adaptation Cycle (v3)*. Read it carefully and identify weaknesses in its **structure**: missing stages, overlapping stages, unclear transitions, axes that don't compose cleanly, or end states that aren't actually distinct. For each issue, propose a concrete revision (rename, merge, split, reorder, or add). Do not comment on prose quality. Prioritize the 5 changes that would most improve the model's explanatory power.

**Best for:** finding taxonomy problems, redundancy, gaps.

---

### Prompt B — Falsifiability & Predictive Power

> Treat this model as a scientific hypothesis. For each stage and transition, ask: *what observation would falsify this?* Identify claims that are unfalsifiable, tautological, or so flexible they explain every outcome post-hoc. Propose specific behavioral indicators or measurable signals that would let a researcher empirically distinguish (a) Stage 2 from Stage 4, (b) Stage 3B from Stage 5, (c) Stage 6B from Stage 7D, and (d) emotional vs. practical dropout. Where the model cannot be operationalized, say so directly.

**Best for:** tightening definitions, exposing hand-waving, forcing operational rigor.

---

### Prompt C — Adversarial / Steel-Man Critic

> You are a skeptical reviewer who believes stage models of psychological adaptation are usually folk-psychology dressed up as theory (cf. critiques of Kübler-Ross). Make the strongest possible case that this model is wrong, overfitted to anecdote, or merely renaming things practitioners already know. Then, assuming the author wants to keep the model, list the minimum changes that would make your critique no longer apply.

**Best for:** surfacing hidden assumptions, avoiding theoretical sloppiness.

---

### Prompt D — Missing Populations & Edge Cases

> Identify groups whose experience this model describes poorly or not at all. Consider at minimum: people who first encountered AI as children/teens, people in non-knowledge work (trades, manual labor, service), people with cognitive disabilities, people who use AI primarily for emotional/companionship purposes, AI researchers themselves, people who are economically dependent on *not* adopting AI (e.g., paid human-only services), and people who reject AI on ethical/religious grounds without ever passing through Stages 2–3. For each group, point to specific stages that don't fit, and propose either (a) model extensions or (b) explicit scope limits the author should declare.

**Best for:** scope clarity, finding under-modeled segments.

---

### Prompt E — Mechanism Review (cognitive science lens)

> Review this model from a cognitive-science / psychology-of-technology perspective. The model is largely *descriptive* — it names stages but rarely specifies the underlying mechanism (cognitive dissonance? threat appraisal? self-efficacy collapse? identity-protection cognition?). For each stage, name the most plausible mechanism from the existing literature, cite the relevant construct (e.g., Bandura's self-efficacy, Festinger's dissonance, terror management theory, technology acceptance model, Rogers' diffusion of innovations), and flag where the model conflicts with or duplicates existing frameworks. Recommend whether v4 should explicitly anchor each stage to a mechanism.

**Best for:** grounding the model in established theory, avoiding reinvention.

---

### Prompt F — Practitioner Utility Review

> You are a manager, coach, or change-leader who would actually *use* this model to help people adopt AI. Read it and answer: (1) Which stages can I reliably *identify* in a real person from observable behavior? (2) Which transitions can I actually *influence*, and how? (3) Which parts of the model are interesting but operationally useless? (4) What is missing that I would need to make this a working diagnostic + intervention tool? Be blunt — favor utility over theoretical elegance.

**Best for:** turning theory into something usable.

---

### Prompt G — Internal Consistency Audit

> Audit this document for internal contradictions, ambiguous transitions, and ill-defined terms. Specific checks: (1) Can a person be in two end states (7A–7F) simultaneously? The text says yes — does the rest of the model support that? (2) Stage 4 (Trust Evaluation) is reachable from Stage 1A, 3B, and 5 — are the entry experiences described differently enough to justify one stage? (3) Delegation depth (D1–D4) is introduced as an axis but only invoked at Stage 3 — should it modulate every stage explicitly? (4) The external trigger ⚡ markers — are they applied consistently? List every inconsistency you find with line-level references.

**Best for:** copy-edit-level rigor that catches real conceptual drift.

---

### Prompt H — Comparative Review

> Compare this model directly to: (a) Kübler-Ross stages of grief, (b) the Technology Acceptance Model (Davis), (c) Rogers' Diffusion of Innovations, (d) the Transtheoretical Model of behavior change (Prochaska/DiClemente), and (e) the Gartner Hype Cycle (as applied to individuals rather than markets). For each: what does Model v3 borrow, what does it add that is genuinely new, and where does an existing model do the job better? Recommend which elements of v3 are original contributions worth keeping vs. which should be replaced by referencing the prior model.

**Best for:** establishing what's actually novel vs. derivative.

---

### Prompt I — Longitudinal / Dynamics Review

> The model describes stages but is weak on *dynamics*: how long stages last, what determines transition speed, what the typical trajectories look like over months/years, and how repeated cycles (regression loops) differ from first-pass cycles. Propose what a v4 dynamics layer should specify, and identify the 3–5 dynamics questions whose answers would most change how the model is used.

**Best for:** moving from a static taxonomy to a process model.

---

### Prompt J — One-Shot "Make It Better"

> Read this model. Propose the **single most impactful change** to v4 — exactly one change — and defend why it beats every other change you considered. Then list the next 4 runners-up in priority order with one sentence each.

**Best for:** forcing prioritization; useful as a tiebreaker after running other prompts.

---

## Suggested Workflow

1. Run **A**, **B**, and **D** in parallel against different models — they cover the broadest ground with least overlap.
2. Run **E** and **H** if you want academic grounding before v4.
3. Run **F** if v4 is meant to be applied, not just published.
4. Run **J** last to force a prioritized synthesis across whatever feedback arrived.

---

## Future Goals (placeholders)

- Goal 2: Validate the model against real user interviews
- Goal 3: Translate the model into an assessment instrument
- Goal 4: Review prose / readability for a general audience
