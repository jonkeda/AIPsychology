# Review Prompt Proposals — Model V6

A collection of prompts for soliciting reviews of [Model6.md](../Model/Model6.md) and the supporting V6 files. Each prompt targets a different reviewer lens so the feedback set is diverse rather than redundant.

V6 is a **descriptive-first** rewrite of V5. The substantive shape (states, axes, transitions) is preserved. The substantive V6 changes that prompts below should focus on:

- **Descriptive-first stance.** V6 explicitly disclaims being predictive, diagnostic, or empirically validated. Conjecture and Testable markers are inline.
- **"Related literature" replaces "Mechanism anchor."** Connections are reframed as vocabulary, not causal claims. A diagnostic disclaimer in `Model6.md` says related literature does not predict or diagnose.
- **Two new states.** **S3X Structural Displacement** (reached from S3E when the role is concluded economically non-viable) and **PEN Pre-emptive Non-Adoption** (values-grounded refusal at S1, before capability testing).
- **New edges.** S2T → S2D when threat surfaces during testing. Direct S3E → S5 (rare, marked as such).
- **State ID rename.** S3 → S3E (Ego Shock); S6 family → S6E/S6D/S6R/S6S; S7 family → S7M/S7I/S7E/S7B/S7V. All five S6 and five S7 states have meaningful letter codes now.
- **Identity-domain scoping made explicit.** Identity Stakes is per-domain. The same person can be S2D in one domain and S7M in another. Defensive evaluation only fires inside identity-threatened domains.
- **Multi-occupancy rules spelled out** in `02-state-graph.md`.
- **S0 has two readings.** Pre-encounter (transitional) and permanent non-user (terminal, no stance, distinct from S2D and PEN).
- **Files split.** One file per state under `states/`. Mermaid diagrams. Top-level: `Model6.md`, `01-axes.md`, `02-state-graph.md`, `triggers.md`, `social-context.md`, `dropout.md`, `populations.md`, `healthiness.md`, `usage.md`, `observation-guide.md`, `limits-of-operationalization.md`.
- **Grief language removed from S3E.**

V6 entry point: [Model6.md](../Model/Model6.md). Folder root: `.my/Model/v6/Model/`.

---

## Goal — Insights to Improve the Model

The prompts below are all aimed at the same outcome: *actionable improvements* to Model V6. They differ in **lens**, **rigor**, and **type of weakness** they tend to surface.

---

### Prompt A — Structural Critique (generalist reviewer)

> You are reviewing a descriptive psychological model called *The AI Psychological Adaptation Cycle (V6)*. V6 is a directed graph of states with two modulating axes (Identity Stakes, Task Delegation Level) and a third per-person property (Delegation Ceiling). Read it carefully and identify weaknesses in its **structure**: missing states, overlapping states, unclear transitions, axes that don't compose cleanly, end states that aren't actually distinct, or graph edges that are asserted but not justified.
>
> Pay particular attention to:
>
> 1. The S2T / S2D fork plus the new S2T → S2D edge — is the fork still a clean dichotomy or has the new edge collapsed it into a continuum?
> 2. Whether the four S6 states (Enthusiastic, Dependent, Driven, Social) are genuinely parallel or partially ordered.
> 3. Whether S7M, S7I, S7E, and S7V are behaviourally distinguishable when you only have related-literature anchors to go on.
> 4. Whether **S3X Structural Displacement** is a state or a label for an exit. Is it actually different from a labeled dropout?
> 5. Whether **PEN Pre-emptive Non-Adoption** is distinguishable from S2D in practice, or whether it is S2D plus a story about values.
> 6. Whether **S0 Baseline's two readings** (transitional pre-encounter vs terminal permanent non-user) collapse two different things into one box.
> 7. Whether the new **direct S3E → S5 edge** ("rare") undermines the model by giving every awkward case an escape hatch.
>
> For each issue, propose a concrete revision (rename, merge, split, reorder, add edge, remove edge, promote to its own file, demote to a footnote). Do not comment on prose quality. Prioritise the 5 changes that would most improve the model's explanatory power.

**Best for:** finding taxonomy problems, redundancy, gaps. Highest yield on the V6 structural additions.

---

### Prompt B — Related-Literature Audit

> V6's headline framing change is that V5's "Mechanism anchors" were renamed to **"Related literature"** and explicitly reframed as *vocabulary, not mechanism*. The disclaimer in `Model6.md` says related literature anchors a state in existing thinking and points the reader at further reading, but does not predict behaviour, identify states, or claim causal mechanisms.
>
> Evaluate this move on three dimensions:
>
> 1. **Honesty.** Was the rename a genuine epistemic correction (the V5 anchors were oversold as mechanisms when they were really vocabulary), or a retreat (the model gave up on mechanism claims to avoid having to defend them)?
> 2. **Load-bearing.** Each state still has its related-literature line. Pick three states (recommend S3E Ego Shock, S6E Enthusiastic Overuse, S7M Maturity). For each: does the related-literature line do any work — clarify what the state is, distinguish it from neighbours, suggest interventions — or is it decorative academic dressing?
> 3. **Accuracy.** Are the named constructs (self-efficacy, terror management, dissonance reduction by scope limitation, variable-reward, metacognitive calibration, generativity, resource depletion) the right ones for the states they are paired with? Flag any pairing that is wrong, weakly defended, or where a more obvious construct exists.
>
> For S3E specifically, V6 keeps the V5 compound anchor (self-efficacy collapse + terror management). Is that a defensible compound, or two hedges stapled together?

**Best for:** stress-testing whether V6's core framing change is honest or evasive.

---

### Prompt C — Descriptive-First: Honest or Evasive?

> V6 declares itself **descriptive**, not predictive. It says explicitly: no transition probabilities, no empirical validation, no diagnostic instruments, no treatment protocols. It marks claims **Conjecture** when the model uses them as useful frames without observation, and **Testable** when they could be falsified by a defined study.
>
> Treat V6 as a model that has openly chosen the descriptive lane. For each major claim and transition, ask:
>
> 1. **Did the descriptive labelling go far enough?** Are there claims still presented as if they were observed when they are conjectural?
> 2. **Did it go too far?** Are there claims now labelled descriptive that could be operationalised with a reasonable study?
> 3. **The reversibility test for dropout.** V6 keeps it. Stress-test it. What confounds defeat it? Does it disambiguate the four quadrants of the practical × emotional plane, or only the two pure axes?
> 4. **The S2T vs S2D asymmetric-updating signal.** V6 keeps this as longitudinal. Is the signal strong enough to support a study, or does it need refinement first?
> 5. **The new S3B vs S7M two-axis distinction** (where the boundary sits — identity vs competence; how the boundary moves — reactive vs evidence-driven). Is this actually testable, or descriptive-with-aspiration?
> 6. **The PEN vs S2D distinction.** V6 lists three signals (cross-domain consistency, evidence response, emotional register). Are these strong enough to actually separate the two states, or is the distinction a story?
>
> Where V6 still cannot be operationalised, say so directly. Don't invent plausible-sounding measures. The question is not whether V6 should claim to be testable — it explicitly does not — but whether its claims about its own descriptive status are accurate.

**Best for:** checking whether V6 actually achieved the epistemic honesty it claims.

---

### Prompt D — Adversarial / Steel-Man Critic

> You are a skeptical reviewer who believes stage-and-state models of psychological adaptation are usually folk-psychology dressed up as theory (compare with critiques of Kübler-Ross). V6 has renamed mechanism anchors to related literature, added a descriptive-first disclaimer, added two new states (S3X, PEN), made identity-domain scoping explicit, and split into per-state files.
>
> Make the strongest possible case that V6 is still cosmetic — that it is V5 with framing polish, two new boxes drawn around things that were already implicit, and a more humble tone — but the same underlying structural commitments and the same lack of empirical grounding. Specifically address:
>
> 1. Does the rename to "related literature" + the disclaimer "this is not mechanism, this is vocabulary" buy any explanatory power, or does it just lower the bar to where any vocabulary-level claim is defensible?
> 2. Does the descriptive-first declaration give the model immunity from criticism it doesn't deserve? (Compare with: "this isn't a theory, it's just a useful way of thinking about it" as a defensive move.)
> 3. Are S3X and PEN substantive additions or labels for things V5 already implicitly handled (S3X as a flavour of dropout; PEN as a sub-case of S2D)?
> 4. Is the per-domain scoping a real refinement or an ad-hoc rescue (whenever the model misclassifies someone, declare a different domain)?
>
> Then, assuming the author wants to keep the model, list the minimum changes that would make your critique no longer apply.

**Best for:** surfacing hidden assumptions, checking whether V6 advanced past V5 on substance.

---

### Prompt E — Missing Populations & Edge Cases

> V6 added an explicit scope statement and a `populations.md` file covering: AI-native users, non-knowledge-work, assistive tech, permanent non-users (in S0), and economic access barriers. Plus the new S3X state for structural displacement.
>
> Identify groups whose experience this model still describes poorly or not at all. Consider at minimum: people who first encountered AI as children/teens, people in non-knowledge work, people with cognitive disabilities, people who use AI primarily for emotional/companionship purposes, AI researchers themselves, people economically dependent on *not* adopting AI, people who reject AI on ethical/religious grounds, and people whose primary AI exposure is involuntary (AI used *on* them by employers, insurers, schools).
>
> For each group, point to specific states or transitions that don't fit, and propose either (a) further model extensions or (b) explicit scope limits that should be added to `populations.md`. Specifically:
>
> 1. Does **PEN** actually cover values-based ethical rejection adequately, or only a narrow Western-secular flavour of it?
> 2. Does **S3X** cover all forms of structural displacement, or only the white-collar version (translator, paralegal)?
> 3. Does the **AI-native pathway** description in `populations.md` say enough, or is it a placeholder that should either be expanded or moved out of scope?
> 4. **Permanent non-users in S0** — is this a real population the model can describe, or just a label for "this model doesn't apply"? Is there value in S0-as-terminal beyond completeness?

**Best for:** scope clarity, finding under-modelled segments.

---

### Prompt F — Practitioner Utility Review

> You are a manager, coach, or change-leader who would actually *use* V6 to help people adopt AI. Read the model and answer:
>
> 1. Which states can I reliably *identify* in a real person from observable behaviour in under one conversation? V6 added an `observation-guide.md` with concrete behavioural markers — does it help?
> 2. Which transitions can I actually *influence*, and how?
> 3. Do the related-literature lines help me intervene differently, or are they only useful for academic credibility?
> 4. The two-axis dropout (practical × emotional severity) plus the reversibility test — is it executable in a real workplace, or does it require resources practitioners don't have?
> 5. The new **S3X Structural Displacement** state — when an employee reaches it, does V6 give me anything useful to do? Or does it correctly say "this is no longer a psychology problem, it is an economic one"?
> 6. The new **PEN Pre-emptive Non-Adoption** state — is the diagnostic guidance for distinguishing PEN from S2D good enough that I would not mistake one for the other in a real conversation?
> 7. **Healthiness framing.** V6 added `healthiness.md` with per-state healthiness levels. Does this match what I see in practice, or pathologise normal variation?
> 8. What is missing that I would need to make this a working diagnostic + intervention tool?
>
> Be blunt — favour utility over theoretical elegance.

**Best for:** turning theory into something usable.

---

### Prompt G — Internal Consistency Audit

> Audit V6 for internal contradictions, ambiguous transitions, and ill-defined terms across all the files in `.my/Model/v6/Model/`. Specific checks:
>
> 1. **Related-literature alignment.** Does any state's transition behaviour contradict the construct it is paired with?
> 2. **Multi-occupancy rules in `02-state-graph.md`.** Are the coexistence claims (S6E + S6D mutually exclusive; S6R + S6S can coexist; all S7 states can coexist) consistent with each state's individual file?
> 3. **The S2T / S2D fork plus the new S2T → S2D edge.** V6 says these are "responses to S1, with no implied order between them" but also that S2T can transition to S2D when threat surfaces. Does the rest of the model honour the no-implied-order claim?
> 4. **The two axes.** Identity Stakes (per-domain) and Task Delegation Level (per-interaction) are independent. Find any place where they are treated as if one implies the other.
> 5. **Per-domain scoping.** V6 says the same person can be in different states for different domains. Find cases where the model writes about "the person's state" as if it were singular.
> 6. **⚡ marker consistency.** V6 inherits V5's marker rule. Is the rule applied consistently across `triggers.md` and the state files?
> 7. **Conjecture and Testable tags.** Are there claims of similar epistemic status that aren't tagged? Any claims tagged inconsistently?
> 8. **Dropout scoring.** Are the descriptions concrete enough that two reviewers would score the same case within ±1?
> 9. **S0's two readings.** Find places where the wrong reading is implicitly assumed.
>
> List every inconsistency with file-and-section-level references.

**Best for:** copy-edit-level rigor that catches real conceptual drift.

---

### Prompt H — Comparative Review

> Compare V6 directly to: (a) Kübler-Ross stages of grief, (b) the Technology Acceptance Model (Davis), (c) Rogers' Diffusion of Innovations, (d) the Transtheoretical Model of behaviour change (Prochaska/DiClemente), and (e) the Gartner Hype Cycle (as applied to individuals rather than markets). V6's `00-relationship-to-prior.md` already takes a position on each — read it and evaluate its claims.
>
> For each prior framework: what does V6 borrow, what does it add that is genuinely new, and where does an existing model do the job better? V6's specific original claims:
>
> 1. The **Identity Stakes × Task Delegation Level** two-axis modulation.
> 2. The four-way **S6 split** with distinct vocabulary anchors.
> 3. The **practical × emotional severity dropout plane** plus reversibility test.
> 4. The **explicit `limits-of-operationalization.md`**.
> 5. **NEW in V6:** the per-domain identity-stakes scoping.
> 6. **NEW in V6:** S3X Structural Displacement as a graph branch.
> 7. **NEW in V6:** PEN Pre-emptive Non-Adoption from S1.
> 8. **NEW in V6:** the descriptive-first stance with inline Conjecture / Testable markers.
>
> Evaluate each. Recommend which V6 elements are original contributions worth keeping vs which should be replaced by referencing the prior model.

**Best for:** establishing what's actually novel vs derivative.

---

### Prompt I — Longitudinal / Dynamics Review

> V6 is deliberately silent on numerical dynamics — no transition probabilities, no dwell times. Propose what a V7 dynamics layer should specify, and identify the 3–5 dynamics questions whose answers would most change how the model is used. Design a minimum viable study (panel size, duration, instruments, rough cost) that would yield enough data to add the first numerical transitions honestly.
>
> Specific questions worth prioritising:
>
> 1. **How long do people stay in S3E?** Without dwell-time estimates the model cannot tell a practitioner whether to intervene now or wait.
> 2. **What fraction of S5 people regress to S3E on a capability jump?**
> 3. **What fraction of S2T testers end up in S5 vs S2D?**
> 4. **Time-to-burnout from sustained S6E or S6R.**
> 5. **How stable is S3X over years?** If most S3X people transition to a new domain within months, S3X is a phase. If they stay, it is an end state.

**Best for:** scoping the V7 empirical work.

---

### Prompt J — V5 → V6 Diff Review

> V6 is a revision of V5. Read both ([Model5.md](../../v5/Model5.md) and the V6 files under `.my/Model/v6/Model/`) and evaluate the changes as a diff:
>
> 1. **"Mechanism anchor" → "Related literature" rename** plus the diagnostic disclaimer. Improvement, lateral, or evasion?
> 2. **Descriptive-first stance** declared explicitly. Does this change anything substantive?
> 3. **Inline `Conjecture` and `Testable` markers** instead of a single bottom-of-document section. Improvement or noise?
> 4. **State ID rename** (S3 → S3E, S6A/B/C/D → S6E/D/R/S, S7A/B/C/D/F → S7M/I/E/B/V). Worth the disruption, or churn for its own sake?
> 5. **New edges:** S2T → S2D and direct S3E → S5. Each one — improvement, lateral, or regression?
> 6. **New states:** S3X Structural Displacement and PEN Pre-emptive Non-Adoption. Each one — does it earn its keep?
> 7. **Per-domain identity-stakes scoping.** V5 implied this; V6 says it explicitly. Did the rest of the model get rewritten consistently with the explicit version?
> 8. **Multi-occupancy rules** spelled out in `02-state-graph.md`. Improvement or over-specification?
> 9. **S0 expanded** to cover permanent non-users. Real coverage or token gesture?
> 10. **Grief language stripped from S3E.** Was V5's grief framing wrong, and does the V6 replacement language capture the same thing or weaken it?
> 11. **File split.** One state per file under `states/`. Useful navigation or fragmentation?
> 12. **Healthiness, usage, observation-guide as separate top-level files.** Help or noise?
>
> For each change: improvement, lateral move, or regression? Which V5 elements should have been changed but weren't? Which V6 changes should be reverted in V7?

**Best for:** evaluating whether V6 actually advanced the model.

---

### Prompt K — Earn-Its-Keep Audit

> Each construct in V6 should pay its way on at least one of three criteria:
>
> 1. **Explanatory power** — predicts an outcome a simpler model gets wrong.
> 2. **Operational use** — lets a practitioner intervene differently.
> 3. **Falsifiability** — makes a prediction that could be wrong (a Conjecture-marked claim that points at a future falsifiable test still counts).
>
> Audit every named construct in V6 against these three criteria. Pay particular attention to constructs added in V6:
>
> - S3X Structural Displacement
> - PEN Pre-emptive Non-Adoption
> - The new S2T → S2D edge
> - The direct S3E → S5 edge
> - S0's permanent-non-user reading
> - Per-domain identity-stakes scoping
> - The per-state healthiness levels
> - The Delegation Ceiling third axis
>
> List any construct that fails all three. Propose deletions.

**Best for:** counteracting feature creep.

---

### Prompt L — One-Shot "Make It Better"

> Read V6 (start at [Model6.md](../Model/Model6.md), then the supporting files). Propose the **single most impactful change** to V7 — exactly one change — and defend why it beats every other change you considered. Then list the next 4 runners-up in priority order with one sentence each.

**Best for:** forcing prioritisation.

---

## Output convention

Every review must be written into `.my/Model/v6/Reviews/` as `NNN-<slug>.md`, numbered sequentially starting at `001`. The naming and structure rules in [.github/instructions/reviews.instructions.md](../../../../.github/instructions/reviews.instructions.md) apply: blunt tone, TL;DR first, findings as numbered verdicts, `Fix:` inside each finding, plain-English glosses on state labels every time they appear in a new finding.
