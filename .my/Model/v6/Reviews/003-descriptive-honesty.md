# 003-descriptive-honesty.md

# Descriptive Honesty — Model V6

## TL;DR

- V6 marks testable claims inline but **observation markers and transition narratives still use assertive language** that obscures their conjectural status. "Most people" claims lack conjecture markers.
- **Reversibility test for dropout is strong for low/high and high/low quadrants but has underspecified confounds** for the high/high mixed case; needs clarification that the test is diagnostic only on two axes.
- **S2T vs S2D asymmetric-updating signal is study-ready** — measurable across model releases, achievable with ~60 subjects over 12–15 months, ~$50–80k.
- **S3B vs S7M heuristic is stated too confidently** — the "where the boundary sits" and "how it moves" signals require longitudinal data but are presented as working definitions for practitioners.
- **PEN vs S2D three-signal frame is asymmetrically observable** — cross-domain consistency and evidence response are tractable; emotional register requires interview and conflates state with personality trait.
- **Clinical claims in healthiness sections** ("within range of clinical distress," six-month thresholds) are presented as observed fact without markers and exceed the model's empirical warrant.

## 1. Observation markers and transition descriptions use assertive language without conjecture grounding — not yet tested

The inline markers work well for specific testable claims (the S2T/S2D asymmetric-updating signal, boundary-movement behavior). But the narrative descriptions of how states work still sound grounded:

- S3E: "Most people who appear to take this path are actually doing accelerated S3E → S3B → S5." — Stated without a **Conjecture —** marker. This is a claim about distribution across paths, not observation.
- S3B: "Many people remain productively in S3B for years." — Stated as observed fact, no marker. Qualitative observation is reasonable but should be marked.
- S2D: "Long-residence S2D in identity-threatened domains is a signal that the org's framing or the person's situation is creating unnecessary identity threat." — This is a diagnostic inference presented without qualification.
- PEN observation markers claim "The position was formed at or shortly after first encounter" is observable. It is. But the model doesn't clarify the temporal window (one week? two weeks? a month?) before the inference becomes unreliable.

**Fix:** Add **Conjecture —** or **Testable —** markers to every transition description and observation marker. Be explicit: "Qualitative observation suggests..." for things you've seen but not counted. "We have not established how long 'at or shortly after' means" for temporal claims. Move clinical thresholds (six months for sustained S3E) to a separate "Clinical signals, not model signals" section with explicit disclaimers.

## 2. Reversibility test for dropout is strong on the axes but has unaddressed confounds on the mixed case — testable (partially)

The dropout model's reversibility test (provide a better tool; if they restart, practical severity was high) is clean for:

- High practical / low emotional: restart = practical was driving it.
- Low practical / high emotional: no restart = emotional was driving it.

But the model does not address confounds in the **high practical / high emotional** case:

- Switching tools changes domain perception. If the original failure was in ChatGPT for legal writing, offering Claude for "legal writing" might feel like a different domain to the person, masking whether practical or emotional was heavier.
- Emotional context-dependency: exhaustion that was severe at the time of dropout may have resolved. Providing better tools tests capability, not whether emotional severity remains.
- The restarting decision may address *both* practical and emotional simultaneously — if they restart, you can't tell whether practical alone was sufficient or whether emotional had also shifted.
- Social costs of restarting ("I was wrong to drop out") can block restart even if practical severity was high and the new tool solves it.

**Fix:** Reframe the reversibility test as a **two-step diagnostic, not one-step**. Step 1: observe whether they restart (tells you high/low emotional). Step 2 (if they restart): ask directly about the emotional context at dropout vs. now. Explicitly note: "This test is reliable for identifying emotional vs. practical, but does not measure the *ratio* in mixed cases; high/high cases require follow-up interviewing." Add to limits-of-operationalization.md.

## 3. S2T vs S2D asymmetric-updating signal is strong enough to support a defined study — testable

The signal is clear: S2D discounts positive evidence and amplifies negative; S2T updates symmetrically. Both S2T and S2D files mark this as **Testable —** with the caveat that it requires multiple evaluations.

This is doable:

**Study design:** Pre-test baseline beliefs about AI on a domain-relevant task. Expose subjects to AI successes and failures (video examples, real-world outputs, benchmarks). Post-test updated beliefs. Repeat quarterly across three to four model releases. Measure asymmetry: (positive evidence belief movement) / (negative evidence belief movement). In S2T this ratio should be near 1.0; in S2D it should be >2.0.

**Sample size:** ~30–40 subjects per state (trained raters pre-classify S2T vs S2D using observation markers).

**Time horizon:** 12–15 months (three to four model cycles).

**Cost estimate:** ~$50–80k (participant honoraria at $50–100 per session, rater training, online testing platform, analysis).

**Signal strength:** Measurable and distinct. Ready to scope.

**Fix:** None. Move this to a "Ready for Study" section in limits-of-operationalization.md. The claim is testable and well-specified.

## 4. S3B vs S7M heuristic signals are overstated; the distinction is testable but methodology is underspecified — testable (with caveats)

The S3B file proposes two distinguishing signals:

- **Where the boundary sits:** identity line (S3B) vs. competence line (S7M).
- **How the boundary moves:** under capability pressure quickly without testing (S3B) vs. only on measured evidence (S7M).

Both are marked **Conjecture —**, which is honest. But the "working heuristic" that follows ("if the boundary maps cleanly onto the person's professional identity, it is S3B. If the boundary maps onto where AI is and isn't reliable, it is S7M.") is stated as a working definition for practitioners without noting that it requires longitudinal validation.

Problems:

- "Where the boundary sits" requires asking people which part of their identity feels threatened and which part they're evaluating competence on. This is self-report territory with high contamination risk.
- "How the boundary moves" is more observable but requires tracking boundary position at two or more timepoints around a capability shift (new model, benchmark, peer demonstration). The model doesn't specify temporal windows or what counts as "measured evidence."
- A person can look like S3B on external behavior (boundary at identity line) while moving the boundary only on evidence (looks like S7M internally). The model acknowledges this as "transitional shape" but doesn't clarify whether this is a distinct diagnostic state or a reporting artifact.
- The claim that S3B boundaries move "quickly without documented testing" requires observing the absence of documentation — baseline level of rigor unclear.

**Fix:** Rewrite the S3B vs S7M section to separate three clarity levels: (1) "We observe two broad patterns" (the boundary difference), (2) "The movement pattern is a testable distinguisher requiring longitudinal data across model releases" (the methodology), (3) "The working heuristic for practitioners in the field" (the rule of thumb, with explicit caveat: "This heuristic is a screening tool, not a diagnosis. Definitive classification requires timeline data."). Specify what "measured evidence" means operationally (benchmark, controlled A/B test, or observational evidence of comparative testing).

## 5. PEN vs S2D three-signal frame is asymmetric in observability and conflates state with trait — testable (with reduced claims)

The PEN file lists three signals distinguishing PEN (values-grounded) from S2D (identity-threatened):

1. **Cross-domain consistency:** Does the objection apply consistently across domains?
2. **Evidence response:** Does capability improvement strengthen the ethical concern or tighten the defensive position?
3. **Emotional register:** Moral conviction/contempt (PEN) vs. anxiety/threat (S2D)?

The file marks this frame as **Testable —**. The problem is asymmetry:

- Cross-domain consistency is observable. If someone declines AI for writing (cites "data ethics") but freely uses it for spreadsheets, that's more S2D-flavored.
- Evidence response is observable: present them with capability improvements; measure response direction (does better AI validate the ethical concern or tighten the defensive stance?).
- Emotional register requires interview/self-report and conflates *state* (are they in S2D or PEN) with *trait* (is this person generally anxious or morally driven?). A person can have both moral conviction and anxiety underneath.

Additionally, the model acknowledges "Most real cases are mixed" but the signal set assumes three independent, reliable separators. They're not.

**Fix:** Downgrade the three-signal frame from "diagnostic separators" to "indicators with known asymmetry." Explicitly note: "Cross-domain consistency and evidence response are observable. Emotional register requires dialogue and has high false-positive and false-negative rates because trait anxiety and moral conviction can co-occur. Expect mixed cases; the signals are probabilistic, not deterministic." In limits-of-operationalization.md, list this as "Longitudinal-only" rather than "Snapshot-observable."

## 6. Clinical thresholds in healthiness sections (six months, "clinical distress") exceed model's warrant — not yet tested

S3E's healthiness section states:

> "Identity disruption that does not resolve after six or more months is within the range of clinical distress, not ordinary adaptation discomfort, and may warrant a referral consideration."

This is presented as a model-derived observation. It is not. The six-month threshold is:

- Not empirically derived from the model.
- Not validated against diagnostic criteria (DSM, ICD).
- Not grounded in the longitudinal studies of occupational stress or identity disruption that do exist.
- A practitioner heuristic, not a model claim.

The same applies to S3E's observation marker: "A practitioner should look for whether the person is moving through S3E (transitioning toward S3B or S5 within weeks to months) or staying." The "weeks to months" window is presented without temporal data.

**Fix:** Move all clinical thresholds (six months, weeks to months, "range of clinical distress") to a separate subsection marked **Practitioner heuristic, not validated**. Add a disclaimer: "These thresholds are based on field experience, not longitudinal studies. Use as rough signposts, not cutoffs. Refer to a mental health professional if you are concerned about a person's wellbeing; do not use this model as a diagnostic instrument." Remove the six-month claim entirely unless you have actual longitudinal data. Replace "within weeks to months" with "monitor for whether the person is actively transitioning (seeking peer support, reading about AI, trying new tools) or withdrawing further; the speed varies widely."

## 7. Identity Stakes is presented as a working construct but lacks measurement specificity — not yet tested

The axes file states:

> "Role-identity centrality (the degree to which a role is central to the self-concept) is offered as vocabulary for thinking about Identity Stakes, not as a tested cause of threat appraisal."

This is honest framing. But the table under Identity Stakes gives concrete-sounding categories ("core part of self-concept") without operational definition. Practitioners applying this model need guidance on how to assess whether stakes are high or low in a specific domain.

Example: Is a senior copywriter's identity more threatened by AI-generated copy than a senior architect's is by AI-generated designs? The model implies yes (writing is arguably more commodified), but does not provide a framework for measurement. Is it time-in-role? Reputation-dependence? Economic fragility? None of these are specified.

**Fix:** Add an operational note under Identity Stakes: "Practical assessment: Ask the person to complete this sentence in the domain being discussed: 'If AI could do this as well as I can, it would mean _______.' High-stakes domains produce identity-level completions ('it would mean I'm not really a [profession]'). Low-stakes domains produce capability-level completions ('it would mean I need to learn new tools')." Make clear this is practitioner scaffolding, not a validated instrument.

## Recommendations (priority order)

1. **Add Conjecture / Testable markers to all observation markers and transition narratives.** This is the core honesty issue. Unmarked assertions in observation sections will be treated by practitioners as grounded.

2. **Move clinical thresholds (six-month window, "range of clinical distress") out of state definitions and into a disclaimer section.** They exceed the model's warrant.

3. **Reframe S3B vs S7M as longitudinal-observable, not working-definition heuristic for snapshot triage.** Add explicit methodological note on timeline requirements.

4. **Clarify the dropout reversibility test's limits on the high/high case.** State that the test diagnoses which axis but requires follow-up for mixed cases.

5. **Downgrade PEN vs S2D emotional-register signal to "high-contamination indicator."** Note that trait and state are confounded.

6. **Spec out the S2T/S2D study protocol and move to "Ready for Study" in limits-of-operationalization.md.** This is ready; advancing it signals honest confidence in the claim.

7. **Add operational guidance for assessing Identity Stakes.** The current framing is honest but practitioners need concrete handles.