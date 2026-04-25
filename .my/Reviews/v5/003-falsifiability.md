# Falsifiability Review — Model V5

## TL;DR

- V5's downgrade of claims from "falsifiable" to "conjecture" or "heuristic" is honest and complete. No remaining whiplash between what's claimed as testable and what actually is.
- Four key conjectures (dual-component S5 stability, S7F-without-S3, "cycle more than once", cultural variability) are genuinely operationalizable with 12–24 month longitudinal studies on 30–80 participants each. The downgrade could affordably become an upgrade.
- The reversibility test for dropout (offer fixed tool, check if dropout restarts) cleanly splits practical vs. emotional causation but does not map to the four quadrants without follow-up interview data on emotional severity.
- The S2T vs. S2D asymmetric-updating signal is measurable (controlled behavioral task showing identity-protecting evidence weighting) but V5 needs to specify which evidence types trigger the asymmetry, otherwise a study might confound priors with motivated reasoning.

## Verdict

V5 disciplines the falsifiability problem well. It marks the epistemically honest distinctions: snapshot-observable, longitudinal-only, self-report-only, conjecture. The model no longer oversells its reach. However, the practical consequence is that four major conjectures remain underdeveloped. The reversibility test and asymmetric-updating signal both look operationalizable but both have exposed confounds that a study design would need to control. V5 is ready for empirical work but the studies need refinement on the confound side.

## Findings

### 1. Did the downgrade go far enough?

**Verdict: Yes.** The model explicitly marks which claims are tested and which are conjecture. No major claim remains presented as falsifiable without acknowledgment of its limits. The "Limits of operationalization" section does the work of epistemic honesty.

However, two soft spots remain:

**Finding 1.1: The mechanism anchors are explanatory, not predictive.** States are anchored to psychological mechanisms (S3 to "self-efficacy collapse and terror management"; S2D to "identity-protection cognition"; S6C to "goal-substitution"). These explain *why* someone is in that state but do not tell you how to test the state itself. If someone appears to be in S3 (identity disrupted, existential discomfort), you might attribute the mechanism to self-efficacy collapse, but you have no way to falsify that attribution. The mechanism could be different (say, financial anxiety triggered by obsolescence fears rather than deep identity disruption).

**Proposed fix:** Add a note under "Mechanism anchors" in the State map section: "Mechanism anchors are explanatory glosses, not testable predictions. They are useful for understanding *why* a person is in a state, not for distinguishing which state they are in."

**Finding 1.2: The ⚡ markers deserve scrutiny.** The model uses ⚡ to mark states where "at least one named external event materially changes the probability of entering or leaving that state." Good rule. But S3B carries ⚡ with "Primary destabilizer: model releases" — is this really the primary destabilizer, or is the primary destabilizer internal (the cognitive dissonance between "I am skilled at X" and "AI is also skilled at X")? Model releases are a trigger, but they're not the only path into S3B from S2D. A person in S2D might internally resolve the cognitive dissonance without waiting for a new model.

**Proposed fix:** Clarify S3B's ⚡ marker to: "Accelerated by: model releases. Entered from: S2D via internal cognitive dissonance resolution." Remove "primary."

---

### 2. Did the downgrade go too far?

**Verdict: Partway.** Four conjectures are genuinely operationalizable with modest resources and should be upgraded to "testable" status once a study design exists:

**Finding 2.1: "Most people cycle through the model more than once."** Currently marked as qualitative conjecture. But this is testable: gather 60 people in S5/S7, follow them for 18 months, code state transitions quarterly, count how many regress to S2D/S3 and then return to S5/S7. If fewer than 30% show cycling, the claim fails. Budget: ~$80k for a longitudinal panel study with quarterly interviews.

**Finding 2.2: The dual-component stability requirement for S5.** Currently marked as conjecture: "Stability has two components, both required: Internal reframing — personal mental model is coherent. Social normalization — surrounding environment treats AI use as unremarkable."

Both are measurable: (1) internal reframing via interview (ask them to explain when/how they use AI, rate the coherence of their account); (2) social normalization via survey (how often do they mention AI use in meetings without explanation? How often do colleagues mention it to them?). Design: 50 people identified as in S5, measure both components on entry, follow them 12 months, code whether erosion of either component predicts regression. Budget: ~$60k.

**Finding 2.3: The S7F-without-S3 collapse claim.** Currently marked as conjecture. "Most stable when the person has previously passed through S3. Lived experience of Ego Shock is what makes them credible to others currently in it." Test via interview: recruit 25 active AI mentors/evangelists, ask them directly whether they experienced S3 discomfort in their own adoption. Follow them for a year; if any S7F advocates who never felt threatened collapse into S6D (social-pressure-driven), the claim holds. If S7F advocates without S3 remain stable, the claim fails. Budget: ~$20k for 25 interviews + 12-month check-ins.

**Finding 2.4: The heuristic distinction in S3B vs. S7A.** Currently marked as heuristic, not measured: "In S3B, boundaries are renegotiated **under capability pressure**. When a new model release crosses one of the self-imposed lines, the line moves quickly without documented testing. In S7A, boundaries move **only after measured evidence** — a benchmark, a real-world failure, a controlled comparison."

Testable via longitudinal behavioral tracking: recruit 40 people (20 in S3B, 20 in S7A), track their AI-use scope across two model releases (expect 6–12 month gap between releases), code whether boundary movement is preceded by explicit testing/benchmarking. Budget: ~$50k (requires participant availability and detailed behavioral logging).

---

### 3. The reversibility test for dropout

The model proposes: "Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit."

**The test is clean but incomplete.** It cleanly separates two groups (restarters vs. non-restarters) but does not map precisely to the four quadrants of the practical × emotional plane.

**Finding 3.1: Confounds that defeat the test.**

- **Tool-switching friction.** A better tool still carries learning cost, habit discontinuity, sunk-cost justification (they've already publicly abandoned AI). Non-restart might reflect switching cost, not emotional severity. Control: offer the tool with full training + onboarding + 2-week "follow-along" period. If they still don't restart, emotional severity was likely high.

- **Social saving-face.** If the person publicly said "I'm done with AI," restarting looks like flip-flopping. Emotional sunk cost in the public stance might prevent restart. Control: offer the tool under a private study frame, not a public "look what changed" frame.

- **Mixed causality and shame entanglement.** Practical failure (slow tool) can trigger identity shame (I'm incompetent). Fixing the tool alone might not restore use because the shame lingers. Control: include a post-restart interview asking "Did fixing the tool remove *all* your reluctance, or did something else still feel uncomfortable?" If the latter, emotional severity was high even in the practical-failure case.

- **Stress-cycle regression to mean.** If they dropped during high stress, restart during low stress might look like the tool fix worked but was actually ambient stress recovery. Control: test the tool during similarly stressful periods as the original dropout, or stratify dropout by stress level.

**Finding 3.2: The four-quadrant mapping is indirect.** The test cleanly separates:

- Restarters → practical severity was high (may have low or high emotional)
- Non-restarters → emotional severity was high (may have low or high practical)

To map the four quadrants, you need:
- Interview all restarters: "Did identity threat / fear contribute to your original exit?" Restarters + no emotional factor = high practical / low emotional.
- Interview all non-restarters: "Would you say the tool genuinely didn't work, or did it feel risky / identity-threatening?" Non-restarters + practical complaints = high practical / high emotional (mixed).
- Re-offer the tool to non-restarters 6 months later (after emotional recovery): if they restart then, you had high practical / high emotional. If they still don't restart, it's high emotional / low practical.

**Verdict:** The reversibility test works for rough practical/emotional splitting but requires follow-up measurement (interview + delayed re-offer) to map the four quadrants cleanly.

**Proposed fix:** Rename the section to "Reversibility Test (Screening Instrument)" and add: "The test separates practical-driven from emotional-driven dropouts at first pass. To map mixed causality (high practical / high emotional) and to measure emotional severity quantitatively, follow with a structured interview asking about identity threat / confidence erosion, and consider re-offering the tool 6 months later after emotional recovery."

---

### 4. The S2T vs. S2D asymmetric-updating signal

The model claims: "In S2D, asymmetric updating: S2D discounts positive evidence and amplifies negative evidence." Listed as longitudinal-only because both states look like "testing" in a snapshot; the asymmetry is only visible across multiple evaluations.

**Finding 4.1: The signal is measurable and grounded in known psychology.**

Asymmetric updating is a real phenomenon (identity-protective cognition, Dan Kahan's work on political belief; Festinger on cognitive dissonance). You can measure it in a controlled task: show 40 S2T and 40 S2D people a series of AI outputs (8 strong, 8 weak), ask them to estimate "What fraction of outputs would you expect to be this strong/weak?", measure whether S2D people weight negative examples more heavily than S2T people. This is standard behavioral-judgment methodology and the mechanism is strong enough to support a hypothesis.

**Finding 4.2: There's a critical confound that must be controlled.**

S2T and S2D people might simply have different *prior beliefs* about AI capabilities. If S2D people genuinely think "AI is weak at this task" and S2T people think "AI is strong," they'd naturally discount/amplify different evidence types without any identity-protection mechanism. The asymmetry would be a Bayesian belief update, not motivated reasoning.

To test asymmetric updating *as identity protection*, you must:

1. Elicit their prior belief explicitly ("Before today, what fraction of AI outputs at this task would you have guessed were good?")
2. Show evidence that contradicts their prior
3. Measure belief change: S2D people should resist updating their belief more than S2T people, even when the evidence is identical

**Finding 4.3: V5 lacks specificity on which evidence types matter.**

The model says asymmetric updating happens on "positive evidence" (good AI outputs). But does it happen on *all* positive evidence, or only on evidence in high-stakes domains? If someone is S2D about AI for creative design (high stakes) but S2T about AI for email summaries (low stakes), would asymmetric updating show up equally?

**Proposed fix:** Specify: "Asymmetric updating in S2D is strongest for evidence in the domain where identity stakes are high (e.g., a designer's core craft). Evidence in low-stakes domains may not trigger asymmetry."

**Verdict:** The signal is strong enough to support a study (~80 participants, 2-hour session per person, controlled evidence evaluation task), but the design must: (1) control for prior beliefs; (2) use evidence that contradicts the prior; (3) measure belief change after exposure, not just judgment of output quality; (4) specify which evidence types (high-stakes domain + salient capability threat) trigger asymmetry.

---

## Recommendations

**Immediate (before next version):**

1. Add a clarifying note under "Mechanism anchors": They are explanatory, not testable predictions.
2. Revise S3B's ⚡ marker: Remove "primary destabilizer" and specify that model releases accelerate (do not uniquely trigger) the state.
3. Add a subsection to S3B: "Operationalizing the S3B/S7A distinction" — specify that longitudinal observation requires coding boundary-movement behavior across 2+ model releases.
4. Rename "Reversibility Test" to "Reversibility Test (Screening Instrument)" and add follow-up guidance: interview for emotional severity; consider re-offer after 6 months.

**Medium-term (testable in 12–24 months with modest budgets):**

5. Commission a 12–18 month longitudinal study on S5 dual-component stability (50 participants, quarterly measurement, ~$60k).
6. Commission a 12–month cycling-and-regression study (60 participants, 18-month track, ~$80k). This directly tests "Most people cycle through the model more than once."

**Longer-term (high-value, higher-cost):**

7. Design and validate a controlled behavioral task for S2T vs. S2D asymmetric-updating (80 participants, controlled evidence evaluation, controlled priors, ~$40k). Use this to replace "longitudinal-only" with "testable via controlled task."
8. Commission a 25-person interview study on S7F stability with and without prior S3 (check for collapse under pressure at 12 months, ~$20k).
