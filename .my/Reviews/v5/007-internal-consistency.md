# Internal Consistency Audit — Model V5

## TL;DR

- **S2T marker inconsistency**: Mandates compress S1 and change S2T's entrance probability; S2T should carry ⚡ but doesn't. S5 can be exited via capability jumps (explicit in transitions); should carry ⚡ but doesn't.
- **S7C self-contradiction**: Marked "⚡ No external-event marker," then immediately lists triggers (public AI ethics incidents, personal moral dilemmas). Inline note contradicts the marker decision.
- **S6A/S7A asymmetry, not explicitly flagged**: S6A is "enthusiastic, uncritical, uses AI for everything"; S7A is "calibrated, measured." Model allows S6A → S7A, but doesn't explicitly state these are incompatible simultaneously in the same domain. Implicit but not stated.
- **S3 terror management understated**: Applied as core mechanism but marked neither as conjecture nor as novel adaptation. Sits between "cited construct" and "untested claim" without clear epistemic label.
- **Dropout axes lack operationalization precision**: The reversibility test conflates practical failure-fixing with emotional recovery. A person might restart for a low-stakes domain without identity-threat resolution, or refuse to restart due to learned helplessness even when the tool failure is fixed. Inter-rater agreement on 0–10 scales would be loose (±2–3, not ±1).
- **S2T/S2D fork: structure contradicts non-order claim**: S2T exits directly to S5; S2D must exit through S3 or S3B first. Model claims "no implied order," but graph implies S2D is the emotional path requiring processing. Not a false claim, but an unstated asymmetry.
- **Multi-occupancy boundary undefined**: Model allows S6 multi-occupancy and S7 multi-occupancy, but never explicitly states whether S6 and S7 can coexist, or whether S3B and S7A can coexist in the same domain.

## Verdict

V5 is internally coherent at the broad level — the state graph, axes, mechanism anchors, and dropout plane mostly hang together — but several specific consistency gaps surface under audit. The ⚡ marker rule is the single largest source of inconsistency: it is stated cleanly, then applied with inline exceptions and unstated distinctions (creation vs. amplification, direct trigger vs. upstream compression). The "no implied order" claim about the S2T/S2D fork is contradicted by the transition graph, which gives S2T a direct route to S5 and forces S2D through emotional processing first. Multi-occupancy rules need to be tightened so practitioners can classify cases without guessing. None of these are fatal — they are the kind of issues that surface on a careful audit and are fixable in V6.

---

## Findings

### 1. Mechanism-State Alignment

**1.1 — S6A exit mechanism misaligned.** S6A is anchored to **variable-reward reinforcement** — "the intermittent-reward dynamic that underlies compulsive engagement." Variable-reward theory predicts stickiness: unpredictability sustains behavior. Yet S6A's transitions include → S7A "as the enthusiasm settles as the person learns where the tool fails." Learning failure modes should *increase* the unpredictability of outcomes (sometimes it fails, sometimes it works), not decrease engagement. The mechanism predicts the person stays *longer* in S6A if outcomes are unpredictable, not that they naturally transition out. The text describes a *learning* exit (person discovers limits), but the mechanism predicts a *fatigue* exit (rewards are exhausted, slots stop paying). This is a weak point that surfaces when you ask "what makes S6A *end* according to its mechanism?"

Recommendation: Either (a) add a secondary exit mechanism to S6A (e.g., "once satiation occurs or rewards plateau," to match variable-reward theory more precisely), or (b) reframe the anchor as "novelty-driven exploration" rather than "variable-reward reinforcement," since what's actually described is curiosity-exhaustion.

**1.2 — S7F prerequisite claim is stated as conjecture but lacks justification.** The note says: "The 'S3 prerequisite for stable S7F' claim is currently conjecture." But the text provides no mechanistic reason why generativity (the S7F anchor) would require prior self-efficacy collapse (S3). Erikson's generativity doesn't require identity disruption; teachers and mentors come from many paths. The model asserts a prerequisite without mechanism support. This is weaker than the other conjecture tags because it doesn't explain *why* you're conjecturing.

Recommendation: Either provide a mechanistic explanation for why S3 experience makes S7F stable (e.g., "lived experience of identity disruption gives credibility to people in S3, which is necessary for generative mentoring"), or relax the claim to "S3 experience may strengthen S7F stability" without stating it as a prerequisite.

### 2. Multi-Occupancy Boundaries

**2.1 — S6 and S7 co-occupancy is undefined.** The model explicitly allows multi-occupancy within S6 ("combinations are S6A + S6C… S6B + S6D") and within S7 ("S7A + S7C is common"). The state map shows S6 as intermediate (downstream of S5, with arrows to S7) and S7 as end-state. The model never explicitly states whether a person can be in S6A and S7A simultaneously. The transitions imply sequence (S6A → S7A), not simultaneity. But regression is allowed, so could a person regress from S7A to S6A and stay there? The model doesn't forbid it. For users (practitioners trying to categorize people), this ambiguity creates classification uncertainty.

Recommendation: Add a sentence after the S7 introduction: "S6 and S7 states are not simultaneous occupancy pairs; a person exits S6 upon entering S7 and can only re-enter S6 via regression."

**2.2 — S3B and S7A domain-specific coexistence is not stated.** The model says "A single person can have low stakes in one domain and high stakes in another." It also distinguishes S3B and S7A by a heuristic: S3B renegotiates boundaries *under capability pressure*; S7A renegotiates only *on measured evidence*. The model never explicitly states: "In the same domain, S3B and S7A cannot coexist because they describe mutually exclusive boundary-movement behaviors." A reader could infer this, but across-domain coexistence (S3B in one domain + S7A in another) is reasonable and should be stated explicitly.

Recommendation: Clarify in the S3B section: "S3B and S7A are domain-specific states; a person can be in S3B for high-stakes domains while in S7A for low-stakes domains. In the same domain, they are mutually exclusive because they describe opposite boundary-movement drivers."

### 3. The S2T / S2D Fork

**3.1 — Fork is asymmetric despite "no implied order" claim.** The model states: "Both are responses to S1; neither is sequentially 'before' the other." But the transition architecture reveals asymmetry:

- S2T transitions: → S5 (direct), → S2D, → Dropout.
- S2D transitions: → S3, → S3B, → S1, → Dropout. (No direct → S5.)

S2T has a direct escape route to stable integration (S5). S2D has no direct escape; it must resolve through emotional shock (S3) or compromise (S3B) first. The model claims these are equal forks, but the structure implies S2D is the path requiring emotional processing while S2T can skip it.

This is not a *false* claim — the model doesn't explicitly say "both reach S5 at equal rates" — but it's an unstated asymmetry that contradicts the "no implied order" framing. A reader might infer (reasonably, from the graph) that S2D is the "harder" path.

Recommendation: Acknowledge the asymmetry explicitly in the S2T/S2D section: "S2T offers a direct path to S5; S2D requires passage through S3 or S3B. This structural asymmetry reflects the difference between rational evaluation (S2T) and ego-defensive evaluation (S2D), not a canonical ordering. Both are valid responses to S1."

### 4. The Two Axes

**4.1 — No violations found.** The model consistently treats Identity Stakes and Task Delegation Level as independent factors that modulate intensity but don't determine each other. The S3 table (Stakes × D-Level) correctly shows that intensity is a *function* of both, not that one implies the other.

### 5. ⚡ Marker Consistency

**5.1 — S2T should carry ⚡ but doesn't.** Rule: "A state carries ⚡ if and only if at least one named external event materially changes the *probability* of entering or leaving that state."

S1 text states: "⚡ Compressed by: workplace mandates, peer adoption events, compelling demos." Compression of S1 changes the probability distribution of exit times from S1, which directly affects the probability of entrance into S2T and S2D. If a mandate compresses S1 (speeds it up), then S2T is entered sooner and with higher probability. S2T text states: "⚡ No external-event ⚡ marker: S2T is internally driven and is not reliably accelerated or reversed by named external events." But mandates *do* accelerate S2T by compressing S1. The text contradicts the marker rule as stated. Either S2T should carry ⚡, or the rule should be narrowed to "external events that directly trigger this state, not events that compress upstream states."

Recommendation: Either add ⚡ to S2T with note "Compressed by: workplace mandates that accelerate S1," or redefine the ⚡ rule to "named external events that directly trigger or reverse this state (not secondary effects of upstream compression)."

**5.2 — S5 should carry ⚡ but doesn't.** S5 transitions include: "→ **S3 Ego Shock** — regression via external trigger." Capability jumps (a named external event) materially change the probability of exiting S5. The rule requires the ⚡ marker if an external event changes entry/exit probability. S5 has no ⚡ marker and no note about external triggers in its state description, yet the transition section explicitly names capability jumps as regression triggers.

Recommendation: Add ⚡ marker to S5 with note "Re-triggered backwards by: capability jumps that invalidate the integrated schema."

**5.3 — S7C contradicts its own marker.** S7C text states: "⚡ No external-event ⚡ marker: S7C is internally driven. Triggers exist (a public AI ethics incident, a personal moral dilemma) but they *amplify* rather than create the state." This is self-contradictory. The rule is "materially changes the probability of entering or leaving that state." A public AI ethics incident materially changes the probability of *entering* S7C (a person not previously reflecting suddenly must reflect publicly). The marker rule doesn't distinguish "amplification" from "creation"; any material change in probability triggers the marker. The note's distinction between "triggers that create vs. amplify" isn't part of the stated rule.

Recommendation: Either add ⚡ to S7C ("Re-triggered by: public AI ethics incidents, personal moral dilemmas that force reflection"), or redefine the marker rule to explicitly distinguish "creation events" from "amplification events" and state which triggers the marker.

**5.4 — S6B marker status is ambiguous.** S6B is marked "⚡ No external-event marker: S6B is internally driven." S6B is described as entered from S3 (which is itself triggered by capability jumps, a named external event). The entry path includes external triggers (S3 is triggered externally), yet S6B claims no external marker. If S6B is downstream of triggered S3, is S6B itself not externally triggered? The model's reasoning is that S6B's *maintenance* (low self-efficacy displacement) is internally driven, even though its *entrance* is downstream of external triggers. This is a plausible distinction (entrance vs. maintenance), but it's not stated in the rule.

Recommendation: Clarify whether the ⚡ rule applies to state entrance, state maintenance, or both. If both, S6B should carry ⚡ (entered via externally-triggered S3). If only maintenance, add that clarification to the rule.

### 6. Conjecture Tags

**6.1 — S3 terror management mechanism lacks epistemic label.** The model anchors S3 to "self-efficacy collapse" (Bandura, cited) and "terror management in the loose sense — confrontation with one's own replaceability triggers the same kind of existential discomfort that confrontation with mortality does." Terror management theory in psychology concerns existential threat and mortality salience. Applying it to AI capability threat is a reasonable inference, but it's not cited to existing work on AI and existential threat. The model says "in the loose sense," acknowledging the adaptation, but does not mark this as conjecture or experimental. Compare this to how "generativity (S7F)" is cited to Erikson and then explicitly marked conjecture when extended beyond Erikson's scope (S3 prerequisite). The terror management claim deserves similar treatment.

Recommendation: Either add a note "Terror management application to AI replaceability is currently untested; this section should be treated as a proposed mechanism, not a confirmed one," or move the claim to the "Limits of operationalization" section under "Currently conjecture."

**6.2 — Two-axis dropout model (practical × emotional severity) is positioned as operationalized without empirical grounding.** The model introduces the severity axes and then proposes the reversibility test as an "operational test." The tone suggests this is a concrete instrument, but the model has not tested it and cannot test it without dropout cases. The reversibility test has known confounds (see Finding 7.1 below). The two axes themselves are presented without citation to existing severity/comorbidity models for dropout, suggesting they are novel constructs. Compared to how "Adoption Ceiling" was removed in V5 because the model couldn't operationalize it, the two-axis dropout model is presented more confidently than justified.

Recommendation: Mark the two-axis dropout section as "proposed operationalization, pending validation" or add a note in "Limits of operationalization": "The two-axis dropout model (practical × emotional severity) has been designed but not yet tested. The reversibility test is a candidate protocol, not a validated instrument."

**6.3 — "Most people cycle through the model more than once" is marked conjecture but lacks specificity.** The model states "Regression is normal. Most people cycle through the model more than once as AI evolves" and then notes "'more than once' is qualitative. V5 deliberately avoids numerical claims about cycle frequency." This is appropriately marked as conjecture, but the conjecture itself is vague ("more than once" could mean 2× or 20×). The note explains why the model doesn't quantify, but it doesn't specify what "cycling" means operationally (does re-entering S2T count? does lateral shift within S7 count?). This makes the claim hard to test later.

Recommendation: Define "cycling" explicitly in the conjecture note: "A cycle is defined as: exiting S5+ states, re-entering S1 or S2, and reaching S5+ again. The claim 'most people cycle more than once' is qualitative and untested." This makes the claim falsifiable later.

### 7. Dropout Scoring

**7.1 — Reversibility test conflates recovery of practical function with emotional resolution.** The test says: "Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit." This assumes:

- **A tool can isolate practical failure:** Often, the tool's failure was entangled with identity threat. An AI that made mistakes *on a high-stakes task* is practical failure + emotional threat simultaneously. Fixing only the practical side (better AI, lower stakes) doesn't isolate the emotional driver. A person might restart for low-stakes use (practical recovery) without their identity-threat emotion being resolved.
- **Restarting proves practical severity:** A person might refuse to restart even with a fixed tool because they've internalized the failure (learned helplessness) or lost trust. This is emotional residue from the original dropout, not a measure of the original practical severity. The test measures "willingness to retry with a better tool," not "practical severity of the original dropout."
- **The two axes are truly independent in dropout cases:** In reality, many dropouts are described as "the tool failed *and I felt terrible about it*." Severing practical and emotional severity artificially might not map to actual human experience.

Example: A person drops out because "AI made high-stakes errors and I lost confidence in my own judgment" (mixed practical + emotional, with S6B-style trajectory). You give them a better AI tool for low-stakes tasks. They restart for low stakes. The test concludes "practical severity was high." But the original dropout's practical failure was entangled with identity threat; the restart isn't proof of the original practical severity, it's proof they can recover *at lower stakes*. The test conflates "tool failure" with "the original failure severity."

**7.2 — Qualitative descriptions are too loose for ±1 inter-rater agreement.** The model provides four regions:

- "High practical / low emotional: Tool genuinely doesn't work for them."
- "Low practical / high emotional: Identity threat or exhaustion."
- "High practical / high emotional: Mixed — tool failed in an identity-vulnerable spot."
- "Low / low: Boredom, indifference, opportunity cost."

For a case like "I tried using AI for my writing, but every time I used it, I felt like I was cheating, and also the outputs were mediocre," two reviewers might score this differently:

- Reviewer A: Practical severity 6 (outputs are mediocre), emotional severity 7 (identity/cheating guilt). Region: high practical / high emotional.
- Reviewer B: Practical severity 3 (mediocre but workable with editing), emotional severity 8 (the cheating feeling is the driver). Region: low practical / high emotional.

The qualitative descriptions don't provide enough precision to pin down scores. The 0–10 scale allows 11 levels of granularity, but the descriptions provide only 4–5 prototypes. Inter-rater agreement would be ±2–3, not ±1.

Recommendation: For each axis, provide three concrete reference points (0, 5, 10) with specific examples. Example:

Practical severity:
- 0: Tool works perfectly for their use case; no failures cited.
- 5: Tool has intermittent failures (e.g., 1 in 3 outputs requires heavy editing); person can work around them.
- 10: Tool fails systematically on their core task; unusable without redesign.

Emotional severity:
- 0: No identity concerns; person dropped out due to opportunity cost or indifference.
- 5: Mild discomfort about role or authenticity; person feels some tension but manageable.
- 10: Severe identity threat or existential discomfort; person describes using the tool as threatening their sense of self.

---

## Recommendations

**Priority 1: Fix S7C marker contradiction** (Finding 5.3). Add ⚡ marker or redefine the marker rule to disambiguate "amplification" from "creation." Do this before the next version is circulated; the contradiction undermines confidence in the entire ⚡ system.

**Priority 2: Clarify ⚡ rule scope** (Findings 5.1, 5.2). Decide whether the rule applies to direct triggers only or also secondary effects of upstream compression. Audit all states against the clarified rule. Add ⚡ to S2T and S5 or revise their descriptions to match a narrower rule.

**Priority 3: Make S2T/S2D fork asymmetry explicit** (Finding 3.1). Acknowledge that S2T has a direct path to S5 while S2D requires emotional processing. This doesn't invalidate the "no implied order" claim, but it explains why the two forks feel structurally different.

**Priority 4: Mark S3 terror management mechanism clearly** (Finding 6.1). Add a note that terror management application to AI replaceability is untested and should be treated as a proposed mechanism, not a confirmed one. This maintains intellectual honesty without removing the mechanism anchor.

**Priority 5: Define S6 and S7 multi-occupancy boundaries** (Finding 2.1). State explicitly: "S6 and S7 states are not simultaneous occupancy pairs" and "S3B and S7A are mutually exclusive within the same domain but can coexist across domains." This removes ambiguity for practitioners using the model.

**Priority 6: Operationalize dropout scoring with reference points** (Finding 7.2). Provide concrete 0/5/10 anchors for both practical and emotional severity axes. Test inter-rater agreement on a small sample (5–10 real dropout cases) to see if ±1 is achievable; if not, adjust the scale or the descriptions.

**Priority 7: Reframe S6A exit mechanism or anchor** (Finding 1.1). Either specify a satiation or plateau condition that makes variable-reward engagement naturally end, or switch the anchor to "novelty-driven exploration" which better predicts learning-driven exit. This strengthens the mechanistic grounding that V5 was supposed to add.

**Priority 8: Revise two-axis dropout model epistemic status** (Finding 6.2). Mark the axes and reversibility test as "proposed" rather than "operational." This prevents practitioners from over-relying on a test that has known confounds and hasn't been validated. Frame it as a tool to *explore* dropout cases, not to *measure* them definitively.
