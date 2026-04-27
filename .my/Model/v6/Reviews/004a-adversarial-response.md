# 004a — Author's Response to the Adversarial Critique

This document responds to [004-adversarial.md](004-adversarial.md) (plain version: [004p-adversarial-plain.md](004p-adversarial-plain.md)). It addresses the critique point by point, accepts what is valid, and pushes back where the critique is aimed at the wrong target.

---

## 1. The model's epistemic position: hypothesis under construction

The adversarial review's sharpest charge is that V6 uses "descriptive-first" framing as a shield — it describes transitions as typical patterns while refusing to commit to predictions, so it can never be proved wrong.

This charge assumes the model is presenting itself as more than a hypothesis. It is not.

The model is a **speculative conceptual framework under construction**. It is the first step in a research programme, not the result of one. The sequence is deliberate:

1. Build the model — name the states, describe the transitions, make the vocabulary usable.
2. Validate the model — test whether the states exist as described, whether the transitions are real, whether the axes predict what they claim to predict.

Gathering data before having a model produces models from the wrong questions. The alternative — building a model that is maximally hedged and qualified at every sentence — produces a document that nobody can use.

The state files are written as if the states are real because they need to be clear enough to be tested. If a practitioner cannot understand what S3E means clearly enough to say "yes, I see this in my client" or "no, this doesn't match what I observe," the model cannot be validated at all. Confident prose is a prerequisite for useful falsification, not an obstacle to it.

This is the most honest position available at this stage: **we have built a structured hypothesis; we know it requires validation; we are not pretending otherwise**. The `limits-of-operationalization.md` file exists precisely to make the epistemic status explicit. The `Conjecture` and `Testable` markers exist to tag individual claims by confidence level. The framing of the model as pre-empirical is not a new admission — it is stated in `Model6.md` § "What kind of model this is."

What the adversarial review asks for — falsifiable transition probabilities, locked-in study designs, pre-observation identity-stakes measures — is the content of the validation programme, not the content of the model. Those belong in a research protocol document, not in a conceptual framework. The two should not be confused.

### Implication for how the adversarial critique should read

Most of Findings 1, 2, and 6 are critiquing the model for not being its own validation. The reframe that makes the critique useful: instead of "this isn't falsifiable," ask "what would a study look like that tested this claim?" That is productive. The adversarial critique's minimum-changes list at the end (items 1, 3, and 5) is a reasonable list of what the validation programme should include. That list is accepted as input to the research design, not as a list of model defects.

---

## 2. The adversarial critique should engage with content

Once the model's status as a speculative hypothesis is accepted, most of Findings 1, 2, and 6 become methodology comments, not content critiques.

The more useful adversarial question is: **are the content claims plausible?**

- Is the S3E → S3B transition actually more common than S3E → S5 direct? Why, or why not?
- Is the S2T → S2D edge driven by identity stakes specifically, or are there other predictors that belong in the model?
- Are the four S6 drivers (reward, anxiety, performance targets, social conformity) the right four? Are there others that belong?
- Is the S3E state's anchor in self-efficacy collapse (Bandura) a plausible mechanism, or does a different construct fit the observable better?
- Does the per-domain scoping of identity stakes actually match what practitioners observe, or do they see people who are consistently high-stakes across domains?

These are content questions. They produce better models. The methodology questions ("this isn't tested") produce research protocols, which are also needed — but they are not the same thing.

The adversarial review should be the place where the conceptual claims get challenged on their own terms. Future versions of this document should hold that standard.

---

## 3. S3X Structural Displacement: not yet resolved, kept as a state for now

The adversarial critique argues that S3X is a documented dropout path, not a distinct state — specifically a "high practical severity dropout with a structural cause."

This is a reasonable structural argument. S3X does share characteristics with practical-severity dropout. The challenge is that the psychological experience of S3X does not feel like dropout to the people in it, and the intervention logic differs. A dropout is an exit the person can potentially re-enter. S3X is entry into a situation where the domain itself is no longer available as a viable option. The work is not re-engagement — it is reorientation.

Whether that difference is large enough to justify a separate state is an open question. The current position: **keep S3X as a state for V6 because the category is easier to reason about and communicate as a distinct node**. The adversarial critique has named the decision point clearly. If validation shows that practitioners cannot reliably distinguish S3X from high-practical dropout, the case for demotion to documented path becomes strong. That is a reasonable study to run.

**Proposed falsifiable test for S3X:** Recruit a sample of people who have left a domain they attribute to AI disruption. Blind-rate their cases as either S3X or practical-high dropout using only behavioral signals (not their stated reason). If inter-rater reliability is below 0.6, S3X cannot be reliably distinguished and should be demoted. If reliability is above 0.7, it justifies the separate state.

---

## 4. PEN and S2D are genuinely different states

The adversarial critique argues PEN is "S2D Defensive Resistance with genuine values in the mix" and should be demoted to an annotation inside S2D.

This is rejected. The distinction is conceptual and, the hypothesis holds, behavioral — but the signals require longitudinal observation to separate, which makes it look like they cannot be separated at all. They can; it is just slow.

The operative difference is not the surface behavior (both decline to engage, both discount capability evidence) — it is the **reason the state is stable**.

- **S2D is stable because identity threat is ongoing.** Remove the threat — reassign the person to a role where AI is not competing with their core skill — and S2D often resolves without further intervention.
- **PEN is stable because the values position is ongoing.** Remove the threat — improve AI capability, reduce economic displacement concerns, address whatever the stated concern is — and PEN typically does not resolve. The position holds regardless of capability improvement.

This is the testable claim. If a person exits their S2D-looking state when the identity threat is removed but not when the capability concern is addressed, that is S2D. If the state is stable regardless of how the capability concern is addressed, that is more likely PEN.

This prediction has not been tested. It is a conjecture about the underlying mechanism that drives the stability difference. The model needs better diagnostics, not a demotion.

**Better diagnostic signals to explore in V7:**

- What happens when the person is exposed to AI use in a domain where their identity is not at stake at all? An S2D person often shows no objection there. A PEN person often maintains the objection.
- What happens when the person's stated ethical concern is materially addressed (relevant legislation passes, the company they objected to changes practices)? PEN may not resolve even then if the values position is deeper than the stated concern. S2D is unlikely to have generated the stated concern in the first place.
- Longitudinal affect: S2D has anxiety in the baseline; PEN is more likely to show equanimity or moral conviction in the baseline. This is self-report, but it is different self-report from "do you use AI?"

### 4a. PEN should get a state number

Currently PEN uses a non-numeric identifier. This is inconsistent with the rest of the model and creates ambiguity about whether it is a full state. It is a full state. It needs a number.

**The question is where in the numbering it belongs.**

PEN is entered from S1 Initial Encounter — the same entry point as S2T and S2D. Structurally it is a parallel fork from S1. This places it naturally in the S2 family: **S2P** (P for Pre-emptive) would be consistent with S2T and S2D.

However, S2P may obscure something important: PEN is not a temporary evaluation state like S2T or S2D. Most people in S2T and S2D eventually move. Many people in PEN do not. It is more structurally similar to the S7 terminal states in stability, even though it is entered at S1.

**Options:**

| Option | Identifier | Rationale |
| --- | --- | --- |
| S2 family | **S2P** | Entered from S1 alongside S2T and S2D; correct in graph position |
| Standalone | **S8P** (or S8) | Signals it is a different kind of state — stable, values-rooted — analogous to S7 terminal states but entered at first encounter |
| Descriptive prefix | **PEN** → **P1** or **P0** | Marks it as a non-adoption track entirely separate from the adaptation track |

**Recommendation: S2P.** The state is entered from S1 and the graph position is correct. The stability difference from S2T/S2D is already captured by the state description. Adding a new prefix family for one state is more complexity than the distinction justifies.

This decision is flagged for review when V7 is planned.

---

## 5. Falsifiable statements should be added to the states

The adversarial critique's Finding 6 — three escape hatches stacked together — is the most structurally important finding. Even within the "speculative hypothesis" framing, a model that provides no path to falsification is not useful as a hypothesis.

The response is not to defend the escape hatches. It is to close them where possible.

**Accepted actions:**

**a. Add a falsifiable statement to each state file.** Each state should include one concrete, study-able prediction in its Open Questions section under a `Testable —` marker. The prediction should specify: what to observe, what result would confirm the state exists as described, and what result would require the state to be revised or removed.

Examples:
- **S3E:** "Testable — people with high Identity Stakes in a domain show a measurable decline in domain-specific self-efficacy scores within four weeks of a major capability release in that domain. If no decline is observed, the S3E description overstates the identity-disruption mechanism."
- **S2D:** "Testable — S2D people update their stated view of AI capability asymmetrically: failures are incorporated into their view; successes are attributed to their prompting skill or to low-stakes context. If updating is symmetric across five or more evaluations, S2D as a distinct state from S2T is not supported."
- **S6D:** "Testable — S6D people show declining performance on domain tasks performed without AI assistance, measured six months into sustained S6D residence. If performance is stable, the dependency dynamic described in S6D does not have the competence-erosion consequence the state implies."

**b. Acknowledge the model is a speculative hypothesis in the model entry point explicitly.** `Model6.md` already does this in § "What kind of model this is." It should be moved to a more prominent position — opening paragraph — so that anyone reading the model encounters it before reading state descriptions, not after.

**c. The per-domain identity stakes problem is real but the solution is a study design, not a model change.** The adversarial critique correctly notes that identity stakes can be redeclared after the fact. The fix is to operationalize stakes before observation — years in domain, income dependency, a short self-report instrument. This belongs in the validation protocol. The model should note in `01-axes.md` that identity stakes must be measured independently of outcome to be a useful predictor, and flag the risk of post-hoc redeclaration explicitly.

---

## 6. Summary: what this response accepts and what it rejects

| Adversarial finding | Accept? | Notes |
| --- | --- | --- |
| Literature anchors commit to nothing | **Partial.** | The function is vocabulary, not mechanism — this is intentional. But each anchor needs a falsifiable prediction alongside it. |
| "Descriptive" framing as a shield | **Reject.** | The model is a speculative hypothesis under construction. Descriptive framing is accurate, not evasive. The validation programme is where predictions get locked. |
| S3X is a labeled dropout path, not a state | **Held open.** | Plausible structurally. Kept as a state until validation provides an inter-rater test. A falsifiable test is proposed above. |
| PEN is S2D with genuine values | **Reject.** | They are genuinely different. The stability mechanism differs. Better diagnostics are needed; demotion is not the answer. |
| Per-domain stakes is an escape hatch | **Accept.** | Stakes must be measured before outcome. The validation protocol needs a pre-observation stakes measure. The model should flag this risk explicitly. |
| Add falsifiable statements to states | **Accept in full.** | Each state should get a concrete Testable prediction with a stated falsification condition. |
| Commit to transition probabilities now | **Reject.** | Fabricated probabilities are worse than honest uncertainty. Probabilities come from the longitudinal panel study, not from the model. |
