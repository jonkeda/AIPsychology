# Review Prompt Proposals — Model5.md

A collection of prompts for soliciting reviews of [Model5.md](../Model/v5/Model5.md). Each prompt targets a different reviewer lens so the feedback set is diverse rather than redundant. Pick one, several, or run them in parallel against different LLMs / human experts.

V5 keeps V4's state-machine structure and the two-axis modulation (Identity Stakes × Task Delegation Level). The substantive V5 changes that prompts below should focus on:

- **Mechanism anchors per state** — each state is now tied to an underlying cognitive-science construct.
- **S1.5 → S2T / S2 → S2D rename.** Both are responses to S1; neither is sequentially "before" the other.
- **Two-axis dropout** (practical severity × emotional severity) replaced V4's binary split.
- **"Limits of operationalization" section** — explicit catalog of what's snapshot-observable, longitudinal-only, self-report-only, or currently conjecture.
- **Downgrades** — pseudo-formula deleted; "falsifiable marker" relabeled as "heuristic distinction"; Adoption Ceiling removed; conjecture claims explicitly tagged.

Prompts below use V5 state labels (S0, S1, S2T, S2D, S3, S3B, S5, S6A–D, S7A–F). Where a prompt is inherited from [005-prompts-v4.md](005-prompts-v4.md), the V4 labels have been remapped and the V5-specific scope added.

---

## Goal — Insights to Improve the Model

The prompts below are all aimed at the same outcome: *actionable improvements* to Model V5. They differ in **lens**, **rigor**, and **type of weakness** they tend to surface.

---

### Prompt A — Structural Critique (generalist reviewer)

> You are reviewing a descriptive psychological model called *The AI Psychological Adaptation Cycle (V5)*. V5 is a state machine with mechanism anchors per state. Read it carefully and identify weaknesses in its **structure**: missing states, overlapping states, unclear transitions, axes that don't compose cleanly, end states that aren't actually distinct, or graph edges that are asserted but not justified. Pay particular attention to: (a) whether the S2T / S2D fork is a clean dichotomy or a continuum that's been forced into two boxes, (b) whether the four S6 states are genuinely parallel or partially ordered, (c) whether S7A, S7B, and S7F are behaviorally distinguishable when you only have the mechanism anchors to go on, (d) whether removing Adoption Ceiling created any unmodeled cases. For each issue, propose a concrete revision (rename, merge, split, reorder, add edge, remove edge). Do not comment on prose quality. Prioritize the 5 changes that would most improve the model's explanatory power.

**Best for:** finding taxonomy problems, redundancy, gaps.

---

### Prompt B — Mechanism Anchor Audit

> V5's headline change is that each state is now anchored to an underlying cognitive-science mechanism: novelty appraisal (S1), calibration under uncertainty (S2T), identity-protection cognition + dissonance (S2D), self-efficacy collapse + terror management (S3), dissonance reduction via scope limitation (S3B), schema integration (S5), variable-reward / self-efficacy displacement / goal-substitution / normative social influence (S6A–D), metacognitive calibration (S7A), extended-self (S7B), meaning-making (S7C), resource depletion (S7D), generativity (S7F). For each anchor, ask three questions:
>
> 1. **Fit.** Is this the most plausible mechanism for the state, or is it the most familiar one the author reached for?
> 2. **Conflict.** Does the anchor predict behavior the model contradicts, or does it predict behavior the model leaves out?
> 3. **Falsifiability gain.** Does anchoring to this mechanism actually make any state's claims more testable, or is the anchor decorative?
>
> Flag any anchor that is wrong, weakly defended, or non-load-bearing. Propose replacements where applicable. Pay special attention to S3 — V4 already called it "the emotional core of the model" and V5 anchors it to two mechanisms (self-efficacy + terror management). Is that a defensible compound anchor or a hedge?

**Best for:** stress-testing the V5 grounding move. **Highest-priority prompt for V5** because the mechanism anchoring is what justifies the version bump; if the anchors don't hold, V5 is mostly a rename of V4.

---

### Prompt C — Falsifiability & Predictive Power (V5 edition)

> V5 walked back several V4 claims of falsifiability. The S3B/S7A "falsifiable marker" is now a "heuristic distinction"; the intensity formula is gone; conjecture claims are tagged as such; a "Limits of operationalization" section catalogs what's snapshot-observable, longitudinal-only, self-report-only, or currently conjecture. Treat V5 as a scientific hypothesis with an honest epistemic register. For each state and transition, ask:
>
> 1. **Did the downgrade go far enough?** Are there any remaining claims that are presented as testable but actually aren't?
> 2. **Did the downgrade go too far?** Are there claims now labeled as conjecture that could be operationalized with a reasonable study?
> 3. **The reversibility test for dropout** — V5's clean operational instrument for the dropout space. Stress-test it. What confounds defeat it? Does it actually disambiguate the four quadrants of the practical × emotional plane, or only the two pure axes?
> 4. **The S2T vs S2D asymmetric-updating signal** — V5 keeps this as a longitudinal-only distinction. Is the signal strong enough to support a study, or does it need refinement before anyone could measure it?
>
> Where the model still cannot be operationalized, say so directly. Don't invent plausible-sounding measures.

**Best for:** checking whether V5 actually achieved the epistemic honesty it claims.

---

### Prompt D — Adversarial / Steel-Man Critic

> You are a skeptical reviewer who believes stage-and-state models of psychological adaptation are usually folk-psychology dressed up as theory (compare with critiques of Kübler-Ross). V5 has added mechanism anchors, downgraded falsifiability claims, and added a "Limits of operationalization" section. Make the strongest possible case that this is still cosmetic — that V5 is V4 with citation polish and a more humble tone, but the same underlying structural commitments and the same lack of empirical grounding. Then, assuming the author wants to keep the model, list the minimum changes that would make your critique no longer apply. Specifically address: do mechanism anchors buy any explanatory power if no anchor's prediction has actually been tested against the model's claims?

**Best for:** surfacing hidden assumptions, checking whether V5 advanced past V4 on substance.

---

### Prompt E — Missing Populations & Edge Cases

> Identify groups whose experience this model describes poorly or not at all. Consider at minimum: people who first encountered AI as children/teens, people in non-knowledge work (trades, manual labor, service), people with cognitive disabilities, people who use AI primarily for emotional/companionship purposes, AI researchers themselves, people economically dependent on *not* adopting AI (paid human-only services), and people who reject AI on ethical/religious grounds without ever passing through S2D/S3. For each group, point to specific states or transitions that don't fit, and propose either (a) model extensions or (b) explicit scope limits the author should declare. V5 removed Adoption Ceiling — does that removal create a gap for users who are mature at low D-levels but in shock at high D-levels?

**Best for:** scope clarity, finding under-modeled segments.

---

### Prompt F — Practitioner Utility Review

> You are a manager, coach, or change-leader who would actually *use* V5 to help people adopt AI. Read it and answer:
>
> 1. Which states can I reliably *identify* in a real person from observable behavior in under one conversation?
> 2. Which transitions can I actually *influence*, and how?
> 3. Do the mechanism anchors help me intervene differently, or are they only useful for academic credibility?
> 4. The two-axis dropout (practical × emotional severity) — does this graded reading change my intervention vs. V4's binary split? If yes, how? If no, the change is overhead with no benefit.
> 5. The reversibility test — is it actually executable in a real workplace, or does it require resources practitioners don't have?
> 6. What is missing that I would need to make this a working diagnostic + intervention tool?
>
> Be blunt — favor utility over theoretical elegance.

**Best for:** turning theory into something usable; specifically validating that V5's complexity is paying its way.

---

### Prompt G — Internal Consistency Audit

> Audit V5 for internal contradictions, ambiguous transitions, and ill-defined terms. Specific checks:
>
> 1. **Mechanism-state alignment.** Does any state's transition behavior contradict its declared mechanism anchor? (Example: if S3 is anchored to self-efficacy collapse + terror management, do its transitions match what those constructs would predict?)
> 2. **Multi-occupancy.** S7 end states are explicitly multi-occupancy; S6 states "can occupy more than one simultaneously." Can a person be in S6A and S7A at once? S3B and S7A?
> 3. **The S2T / S2D fork.** V5 says these are "responses to S1, with no implied order between them" — does the rest of the model honor that, or do later sections still treat S2D as the canonical path?
> 4. **The two axes.** Identity Stakes (per-domain) and Task Delegation Level (per-interaction) are independent. Find any place in the state descriptions where they're treated as if one implies the other.
> 5. **⚡ marker consistency.** V5 declared a strict marker rule (named external event must materially change a transition probability). Is the rule applied consistently? Are there states that should carry ⚡ and don't, or vice versa?
> 6. **Conjecture tags.** V5 marks several claims as conjecture. Are there other claims of similar epistemic status that aren't tagged?
> 7. **Dropout scoring.** The two severity axes go 0–10. Are the descriptions concrete enough that two reviewers would score the same dropout case within ±1?
>
> List every inconsistency with line-level references.

**Best for:** copy-edit-level rigor that catches real conceptual drift.

---

### Prompt H — Comparative Review

> Compare V5 directly to: (a) Kübler-Ross stages of grief, (b) the Technology Acceptance Model (Davis), (c) Rogers' Diffusion of Innovations, (d) the Transtheoretical Model of behavior change (Prochaska/DiClemente), and (e) the Gartner Hype Cycle (as applied to individuals rather than markets). For each: what does V5 borrow, what does it add that is genuinely new, and where does an existing model do the job better? V5's specific original claims appear to be (i) the Identity Stakes × Task Delegation Level two-axis modulation, (ii) the four-way S6 split with distinct mechanisms, (iii) the practical × emotional severity dropout plane plus the reversibility test, and (iv) the explicit "Limits of operationalization" section. Evaluate each. Recommend which V5 elements are original contributions worth keeping vs. which should be replaced by referencing the prior model.

**Best for:** establishing what's actually novel vs. derivative.

---

### Prompt I — Longitudinal / Dynamics Review

> V5 still calls itself a state machine but is deliberately silent on numerical dynamics — no transition probabilities, no dwell times. The "Deliberately not in V5" section says these should be added only when data justifies it. Propose what a V6 dynamics layer should specify, and identify the 3–5 dynamics questions whose answers would most change how the model is used. Also: design a minimum viable study (panel size, duration, instruments) that would yield enough data to add the first numerical transitions honestly.

**Best for:** scoping the V6 empirical work; planning what to measure first.

---

### Prompt J — V4 → V5 Diff Review

> V5 is a revision of V4. Read both and evaluate the changes as a diff:
>
> 1. **Mechanism anchors per state.** Improvement, lateral, or overreach?
> 2. **S1.5 → S2T and S2 → S2D rename.** Does the new labeling actually clarify the post-S1 fork, or does it just replace one label confusion with another?
> 3. **Pseudo-formula deletion** (intensity = baseline × Stakes × Delegation).
> 4. **"Falsifiable marker" → "heuristic distinction"** on S3B/S7A.
> 5. **Two-axis dropout** replacing the binary emotional/practical split, plus the reversibility test.
> 6. **"Limits of operationalization" section** added.
> 7. **Conjecture tags** on S5 dual-component stability, S7F-without-S3, "most people cycle more than once," and the Cultural Variability section.
> 8. **Adoption Ceiling removed.**
>
> For each change: improvement, lateral move, or regression? Which V4 elements should have been changed but weren't? Which V5 changes should be reverted in V6?

**Best for:** evaluating whether V5 actually advanced the model or just polished the rhetoric.

---

### Prompt K — Earn-Its-Keep Audit

> The model has grown across V2 → V3 → V4 → V5 (more states, more axes, more layers, more sections). Each construct in V5 should pay its way on at least one of three criteria: (1) **explanatory power** — predicts an outcome a simpler model gets wrong, (2) **operational use** — lets a practitioner intervene differently, (3) **falsifiability** — makes a prediction that could be wrong. Audit every named construct in V5 against these three criteria. List any construct that fails all three. Propose deletions. The simpler V6 that survives this audit is the recommendation.

**Best for:** counteracting feature creep; the right prompt to run before any V6 starts adding more.

---

### Prompt L — One-Shot "Make It Better"

> Read V5. Propose the **single most impactful change** to V6 — exactly one change — and defend why it beats every other change you considered. Then list the next 4 runners-up in priority order with one sentence each.

**Best for:** forcing prioritization; useful as a tiebreaker after running other prompts.

---

## Suggested Workflow

1. Run **B** first. V5's headline change is the mechanism anchoring; if the anchors don't hold up, V5 is decorative over V4.
2. Run **J** second to check whether V5 actually advanced past V4 on substance.
3. Run **K** third to catch any feature creep before it carries into V6.
4. Run **A**, **E**, and **G** in parallel — broad coverage with little overlap.
5. Run **C** if you want to verify V5's epistemic honesty claim.
6. Run **F** to validate that the added complexity is paying its way for practitioners.
7. Run **H** if you want academic grounding before V6.
8. Run **I** if V6 is meant to add a dynamics layer.
9. Run **L** last to force a prioritized synthesis across whatever feedback arrived.
