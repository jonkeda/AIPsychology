# 004c — V6 Change Plan (from 004a)

Implementation plan derived from [004a-adversarial-response.md](004a-adversarial-response.md). Each item maps to a specific file and a specific change. Items are ordered by priority; P1 changes affect the model's framing, P2 changes affect structure, P3 changes add content to existing state files.

---

## P1 — Framing changes (model entry point)

### P1.1 — Move the "speculative hypothesis" statement to the opening of Model6.md

**File:** `Model6.md`
**Current state:** The pre-empirical framing sits in § "What kind of model this is", which is the fourth or fifth heading a reader encounters.
**Change:** Add a short paragraph at the very top of the file — immediately after the title, before § Scope — that states:

> This model is a **speculative conceptual framework under construction**. The states and transitions are written as concrete descriptions to make the vocabulary usable and testable, not because they have been empirically validated. Validation is the next step; this document is the hypothesis. Everything marked **Conjecture —** is explicitly untested. Everything marked **Testable —** points at a study that could confirm or refute the claim. Everything without a marker is a well-grounded but unvalidated hypothesis.

**Why:** Anyone who reads the model should encounter the epistemic status before reading state descriptions, not after.

---

### P1.2 — Add a measurement-independence warning to the Identity Stakes section

**File:** `01-axes.md`
**Section:** Axis 1 — Identity Stakes
**Change:** Add a note at the end of the Identity Stakes section:

> **Measurement note:** Identity Stakes must be assessed independently of the outcome being explained. Assessing stakes after observing which fork a person took (S2T vs S2D) is circular — the fork is the outcome the stakes are supposed to predict. For stakes to function as a predictor, they must be measured before the observation: for example, years invested in the domain, proportion of income from it, or a short self-report interview administered before any AI interaction is observed. The validation protocol should operationalize Identity Stakes this way. The model flags this explicitly because post-hoc redeclaration of stakes is the main way the S1 fork prediction can be made unfalsifiable.

**Why:** Directly closes the "per-domain stakes as escape hatch" critique accepted in 004a § 5c.

---

## P2 — Structural changes

### P2.1 — Rename PEN to S2P throughout the model

**Rationale from 004a § 4a:** PEN is a full state. Using a non-numeric identifier creates ambiguity. It enters from S1 alongside S2T and S2D, placing it structurally in the S2 family.

**Files to change:**

| File | Change |
|---|---|
| `states/PEN-pre-emptive-non-adoption.md` | Rename file to `S2P-pre-emptive-non-adoption.md`. Change heading to `# S2P — Pre-emptive Non-Adoption`. Update all internal self-references from PEN to S2P. |
| `02-state-graph.md` | Change `PEN: PEN Pre-emptive Non-Adoption` → `S2P: S2P Pre-emptive Non-Adoption`. Change all three PEN edges to S2P. |
| `Model6.md` | Update any inline references from PEN → S2P. |
| `01-axes.md` | Update any inline references. |
| `limits-of-operationalization.md` | Update `PEN vs S2D dressed in ethical language` → `S2P vs S2D dressed in ethical language`. |
| `observation-guide.md` | Update section heading and all inline references. |
| `dropout.md` | Update "Not PEN Pre-emptive Non-Adoption" → "Not S2P Pre-emptive Non-Adoption". |
| `states/S0-baseline.md` | Update PEN reference in the "Two readings" section. |
| `states/S1-initial-encounter.md` | Update transition line and link. |
| `states/S2D-defensive-resistance.md` | Update any cross-references. |
| `states/S7E-ethical-integration.md` | Update any cross-references. |

**After rename:** Update `00-relationship-to-prior.md` if it references PEN.

---

### P2.2 — Add better S2P/S2D diagnostic signals to the S2P file

**File:** `states/S2P-pre-emptive-non-adoption.md` (after rename)
**Section:** Diagnostic difficulty section (currently the last section)
**Change:** Add the three improved signals from 004a § 4 as an additional subsection inside the existing diagnostic difficulty section:

> **Additional signals under investigation (Conjecture — not yet validated):**
>
> 1. **Domain transfer test.** Observe whether the objection persists in a domain where the person's professional identity is not at stake. An S2D person operating in a low-stakes domain typically shows no objection there. An S2P person typically maintains the objection regardless of domain. This is the strongest single signal if observable.
> 2. **Concern-addressed test.** Observe the response when the person's stated ethical concern is materially addressed — relevant legislation passes, the specific company they objected to changes practices, data provenance concerns are resolved. S2P typically does not resolve even then, because the values position runs deeper than the specific stated concern. S2D is unlikely to have generated a values-framed concern in the first place.
> 3. **Baseline affect.** S2D has anxiety in the baseline reading; the underlying threat is ongoing. S2P is more likely to show equanimity or moral conviction in the baseline. This is self-report and is contaminated by social desirability, but the affective signature differs.
>
> The primary stability test: **remove the identity threat** (reassign the person to a role where AI does not compete with their core skill). If the state resolves, it was S2D. If it persists, S2P is more likely. This test has not been run as a controlled study.

---

### P2.3 — Add S3X falsifiable inter-rater test to the S3X file

**File:** `states/S3X-structural-displacement.md`
**Section:** Open questions (add or extend)
**Change:** Add:

> **Testable — state validity test:** Recruit a sample of people who have left a domain they attribute to AI disruption. Blind-rate each case as either S3X Structural Displacement or high-practical-severity dropout using only behavioral and interview signals, without using the person's stated reason. If inter-rater reliability (Cohen's kappa) is below 0.6, S3X cannot be reliably distinguished from high-practical dropout on behavioral grounds and should be demoted to a documented dropout variant. If kappa is above 0.7, the separate state is justified.

---

## P3 — Add one falsifiable prediction to each state file

**Scope:** All 18 state files. Each gets one `Testable —` entry in its **Open Questions** section specifying: what to observe, what result confirms the state, what result requires revision.

Files without an Open Questions section should have one added at the end.

The predictions below are the proposed text. Each should be added verbatim (or close to it) as a bullet under **Open Questions**.

---

### S0 — Baseline

**File:** `states/S0-baseline.md`

> **Testable — terminal vs transitional classification:** A person classified as permanent-non-user S0 (terminal) via interview at time 1 should remain in S0 at 24-month follow-up at a rate above 80%. If a substantial fraction (above 30%) has entered S1 by follow-up, the terminal-S0 classification criteria need tightening.

---

### S1 — Initial Encounter

**File:** `states/S1-initial-encounter.md`

> **Testable — appraisal-to-fork timing:** The S1 → S2T vs S2D fork is predicted to happen rapidly (within the first substantive session, not over weeks). If a significant proportion of people measured after 30 minutes of first use show no stable fork tendency — equally open and defensive in the same session — the fork model needs restructuring as a gradual differentiation rather than an early branch point.

---

### S2T — Trust Evaluation

**File:** `states/S2T-trust-evaluation.md`

> **Testable — symmetric updating:** S2T people should update their stated view of AI capability in both directions — incorporating both positive and negative evidence. Measure stated views before and after five AI interactions across mixed outcomes. If fewer than 60% of S2T-classified people update in both directions, S2T is not distinguishable from S2D by the updating criterion and the primary discriminating signal needs revision.

---

### S2D — Defensive Resistance

**File:** `states/S2D-defensive-resistance.md`

> **Testable — asymmetric updating:** S2D people should show asymmetric updating: failures are incorporated into their view of AI; successes are attributed to their prompting skill, to the low-stakes nature of the task, or to coincidence. Measure attributions across five or more AI interactions with mixed outcomes. If updating is symmetric across more than 40% of S2D-classified people, S2D as a distinct state from S2T is not supported by the updating criterion.

---

### S2P — Pre-emptive Non-Adoption

**File:** `states/S2P-pre-emptive-non-adoption.md`

> **Testable — stability under threat removal:** Identify a sample classified as S2P. Observe whether the state persists when the person is placed in a role or context where AI does not compete with their core professional identity. If a substantial proportion (above 40%) resolves within six months under this condition, the state is better described as S2D with ethical language (identity-threat-dependent), not a distinct values-grounded state.

---

### S3E — Ego Shock

**File:** `states/S3E-ego-shock.md`

> **Testable — self-efficacy decline:** People with high Identity Stakes in a domain should show a measurable decline in domain-specific self-efficacy scores (measured by validated self-efficacy instrument) within four weeks of a major AI capability release in that domain. If no reliable decline is observed in a sample of high-stakes practitioners, S3E's anchor in self-efficacy disruption overstates the mechanism.

---

### S3B — Bargaining

**File:** `states/S3B-bargaining.md`

> **Testable — boundary location:** S3B boundaries should map onto the person's professional identity domain rather than onto AI's reliability profile. Operationalize: ask the person where their AI boundary sits, then independently assess whether that boundary aligns with (a) where AI is currently unreliable or (b) where the person's core identity is invested. In a sample, S3B boundaries should correlate more strongly with identity centrality than with AI failure rate. If the correlation is reversed, the identity-location claim is wrong.

---

### S3X — Structural Displacement

**File:** `states/S3X-structural-displacement.md`

> **Testable — state vs dropout discrimination:** See inter-rater reliability test above (§ P2.3). Additionally: S3X people should report the primary framing of their exit as "there is nowhere to go" (structural), not "it costs too much to continue" (emotional) or "the tool doesn't work" (practical). If the primary framing is indistinguishable from high-practical dropout framing in more than 50% of classified cases, the state boundary is not holding.

---

### S5 — Understanding

**File:** `states/S5-understanding.md`

> **Testable — dual-component stability:** S5 is predicted to require both internal reframing (the person has resolved the identity question) and social normalisation (the person's environment has accepted their AI-collaborative work as legitimate). Identify people classified as S5. Then remove social normalisation (move them to an environment where AI-collaborative work is stigmatised). If a significant proportion regress to S3B or S2D without any change in their internal state or AI capability, the social-normalisation component is load-bearing and the dual-component claim is supported.

---

### S6E — Enthusiastic Overuse

**File:** `states/S6E-enthusiastic-overuse.md`

> **Testable — reward-contingent usage:** S6E usage should track reward events (model releases, positive team reactions, demos). Remove the variable reward for 30 days — no public sharing of AI outputs, no leaderboard, no visible team comparison. If usage drops by more than 40% or shifts to more deliberate, lower-frequency patterns, the reward-contingency driver is confirmed. If usage is stable, S6E may be better described as intrinsic enthusiasm rather than reward-contingent overuse.

---

### S6D — Dependent Overuse

**File:** `states/S6D-dependent-overuse.md`

> **Testable — competence erosion:** S6D people should show declining performance on domain tasks performed without AI assistance, measured at 6-month intervals into sustained S6D residence. Assess performance on domain tasks with AI unavailable at baseline (S6D entry) and at 6 months. If performance is stable or improves, the dependency dynamic described in S6D does not produce the competence-erosion consequence the state implies, and the state description needs revision.

---

### S6R — Driven Overuse

**File:** `states/S6R-driven-overuse.md`

> **Testable — metric-contingent usage:** S6R usage should track productivity reporting cycles. Remove productivity tracking for 30 days. If usage drops significantly or patterns shift from high-volume to more selective, the performance-target driver is confirmed. If usage is stable without tracking, the driver is something other than external performance pressure and the S6R anchor needs revision.

---

### S6S — Social Overuse

**File:** `states/S6S-social-overuse.md`

> **Testable — social-contingency:** S6S people should show different AI behavior when working alone versus in a visible team context. Measure AI usage during solo-work periods versus collaborative or visible-to-management periods. If usage is equivalent in both contexts, the social-conformity driver is not the primary explanation and the S6S definition needs revision.

---

### S7M — Maturity

**File:** `states/S7M-maturity.md`

> **Testable — competence-based boundary movement:** When a new AI model releases with improved capability in an S7M person's domain, their boundary should move only after they have run a deliberate test — not immediately and not under social pressure. Measure boundary-movement timing and trigger across at least three model releases. If more than 40% of boundary movements in S7M-classified people happen before the person reports deliberate testing, the evidence-based boundary claim is not supported.

---

### S7I — Identity Expansion

**File:** `states/S7I-identity-expansion.md`

> **Testable — identity change measure:** S7I involves a genuine expansion of professional self-concept — "I am someone who works with AI as a creative collaborator" is a new identity claim, not just a behavioral change. Measure professional identity descriptions at S5 entry and again after 12 months. S7I people should show reliably different self-descriptions that incorporate AI as part of professional identity, distinct from S7M people who show behavioral change without identity-label change.

---

### S7E — Ethical Integration

**File:** `states/S7E-ethical-integration.md`

> **Testable — reflective depth:** S7E involves sustained, substantive ethical reflection on AI use — not surface-level discomfort. Operationalize: in a semi-structured interview, S7E people should be able to describe (a) at least one specific ethical concern they have about their own AI use, (b) a concrete change they made or declined to make because of that concern, and (c) a case where the ethical answer was genuinely unclear to them. If more than 50% of S7E-classified people cannot meet all three criteria, the state is conflated with general discomfort (closer to S7B precursor territory).

---

### S7B — Burnout

**File:** `states/S7B-burnout.md`

> **Testable — overuse precursor:** S7B should be preceded by a period of overuse (S6E, S6D, S6R, or S6S) in a substantial majority of cases. In a retrospective sample of people currently in S7B, more than 60% should report or show usage data consistent with a preceding S6 state. If a significant proportion report no overuse phase — S7B appearing to arrive directly from S5 without an S6 precursor — the current graph (which routes all S7B through S6) needs additional direct edges or S7B needs a revised entry condition.

---

### S7V — Evangelism

**File:** `states/S7V-evangelism.md`

> **Testable — depth and stability:** S7V is claimed to be more stable when grounded in prior S3E experience. In a sample of people identified as S7V, compare stability over 12 months between those with documented S3E history and those without. Stability operationalized as: still actively and positively advocating for AI adoption, not having publicly reversed their position, and able to engage with substantive objections without deflection. If stability rates are not significantly different between S3E-history and no-S3E-history groups, the S3E-depth claim is not supported.

---

## Change summary

| Priority | Item | Files affected | Type |
|---|---|---|---|
| P1.1 | Add speculative-hypothesis opening to Model6.md | `Model6.md` | Framing |
| P1.2 | Add measurement-independence note to Identity Stakes | `01-axes.md` | Framing |
| P2.1 | Rename PEN → S2P throughout | 11 files | Rename + update |
| P2.2 | Add improved S2P/S2D diagnostic signals | `S2P-pre-emptive-non-adoption.md` | Content |
| P2.3 | Add S3X inter-rater falsifiable test | `S3X-structural-displacement.md` | Content |
| P3.x | Add one falsifiable Testable prediction per state | All 18 state files | Content |

Total files touched: `Model6.md`, `01-axes.md`, 11 files for PEN→S2P rename, and 18 state files for falsifiable predictions. Several state files appear in both the rename pass and the falsifiable prediction pass.
