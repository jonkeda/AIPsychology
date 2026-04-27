# Internal Consistency Audit — Model V5

## TL;DR

- **S2T Trust Evaluation marker inconsistency.** Mandates compress S1 Initial Encounter and change S2T Trust Evaluation's entrance probability; S2T Trust Evaluation should carry ⚡ but doesn't. S5 Understanding can be exited via capability jumps (explicit in transitions); should carry ⚡ but doesn't.
- **S7C Ethical Integration self-contradiction.** Marked "⚡ No external-event marker," then immediately lists triggers (public AI ethics incidents, personal moral dilemmas). The inline note contradicts the marker decision.
- **S6A Enthusiastic Overuse/S7A Maturity asymmetry, not explicitly flagged.** S6A Enthusiastic Overuse is "enthusiastic, uncritical, uses AI for everything"; S7A Maturity is "calibrated, measured." Model allows S6A Enthusiastic Overuse → S7A Maturity, but doesn't explicitly state these are incompatible simultaneously in the same domain.
- **S3 Ego Shock terror management understated.** Applied as core mechanism but marked neither as conjecture nor as novel adaptation. Sits between cited construct and untested claim without a clear epistemic label.
- **Dropout axes lack operationalization precision.** The reversibility test conflates practical failure-fixing with emotional recovery. Inter-rater agreement on 0–10 scales would be loose (±2–3, not ±1).
- **S2T Trust Evaluation/S2D Defensive Resistance fork: structure contradicts non-order claim.** S2T Trust Evaluation exits directly to S5 Understanding; S2D Defensive Resistance must exit through S3 Ego Shock or S3B Bargaining first. Model claims "no implied order," but the graph implies S2D Defensive Resistance is the emotional path requiring processing.
- **Multi-occupancy boundary undefined.** Model allows S6 multi-occupancy and S7 multi-occupancy, but never states whether S6 and S7 can coexist, or whether S3B Bargaining and S7A Maturity can coexist in the same domain.
- V5 is internally coherent at the broad level — the state graph, axes, mechanism anchors, and dropout plane mostly hang together — but several specific gaps surface under audit. The ⚡ marker rule is the single largest source of inconsistency: stated cleanly, then applied with inline exceptions and unstated distinctions. None of these are fatal; all are fixable in V6.

## Findings

### 1. Mechanism-state alignment

1. **S6A Enthusiastic Overuse exit mechanism misaligned.** S6A Enthusiastic Overuse is anchored to **variable-reward reinforcement** (intermittent-reward dynamics underlying compulsive engagement). Variable-reward theory predicts stickiness: unpredictability sustains behavior. Yet S6A Enthusiastic Overuse's transitions include → S7A Maturity "as the enthusiasm settles as the person learns where the tool fails." Learning failure modes should *increase* unpredictability of outcomes, not decrease engagement. The mechanism predicts a *fatigue* exit (rewards exhausted), but the text describes a *learning* exit (person discovers limits). Either add a secondary exit ("once satiation occurs or rewards plateau") or reframe the anchor as "novelty-driven exploration" rather than variable-reward reinforcement, since what is described is curiosity-exhaustion.

2. **S7F Evangelism prerequisite claim is stated as conjecture but lacks justification.** The note says: "The 'S3 Ego Shock prerequisite for stable S7F Evangelism' claim is currently conjecture." The text provides no mechanistic reason why generativity (the drive to mentor or nurture future generations) would require prior self-efficacy collapse. Erikson's work shows generativity does not require identity disruption; teachers and mentors come from many paths. Either provide a mechanism ("lived experience of identity disruption gives credibility to people in S3 Ego Shock, which is necessary for generative mentoring") or relax the claim to "S3 Ego Shock experience may strengthen S7F Evangelism stability" without stating it as a prerequisite.

### 2. Multi-occupancy boundaries

3. **S6 and S7 co-occupancy is undefined.** The model explicitly allows multi-occupancy within S6 and within S7. The state map shows S6 as intermediate (downstream of S5 Understanding, with arrows to S7) and S7 as end-state. The model never states whether a person can be in S6A Enthusiastic Overuse and S7A Maturity simultaneously. The transitions imply sequence (S6A Enthusiastic Overuse → S7A Maturity), not simultaneity, but regression is allowed — could a person regress from S7A Maturity to S6A Enthusiastic Overuse and stay there? The model doesn't forbid it. Add a sentence after the S7 introduction: "S6 and S7 states are not simultaneous occupancy pairs; a person exits S6 upon entering S7 and can only re-enter S6 via regression."

4. **S3B Bargaining and S7A Maturity domain-specific coexistence is not stated.** The model says "A single person can have low stakes in one domain and high stakes in another." It distinguishes S3B Bargaining and S7A Maturity by a heuristic: S3B Bargaining renegotiates boundaries *under capability pressure*; S7A Maturity only *on measured evidence*. The model never states: "In the same domain, S3B Bargaining and S7A Maturity cannot coexist because they describe mutually exclusive boundary-movement behaviors." Across-domain coexistence (S3B Bargaining in one domain plus S7A Maturity in another) is reasonable and should be stated explicitly.

### 3. The S2T Trust Evaluation/S2D Defensive Resistance fork

5. **Fork is asymmetric despite "no implied order" claim.** The model states: "Both are responses to S1 Initial Encounter; neither is sequentially before the other." The transition architecture reveals asymmetry:
   - S2T Trust Evaluation transitions: → S5 Understanding (direct), → S2D Defensive Resistance, → Dropout.
   - S2D Defensive Resistance transitions: → S3 Ego Shock, → S3B Bargaining, → S1 Initial Encounter, → Dropout. (No direct → S5 Understanding.)

   S2T Trust Evaluation has a direct escape route to stable integration (S5 Understanding). S2D Defensive Resistance has none — it must resolve through emotional shock (S3 Ego Shock) or compromise (S3B Bargaining) first. This is not a false claim, but it's an unstated asymmetry. A reader might infer (reasonably, from the graph) that S2D Defensive Resistance is the "harder" path. Acknowledge: "S2T Trust Evaluation offers a direct path to S5 Understanding; S2D Defensive Resistance requires passage through S3 Ego Shock or S3B Bargaining. This structural asymmetry reflects the difference between rational evaluation and ego-defensive evaluation, not a canonical ordering."

### 4. The two axes

6. **No violations found.** The model consistently treats Identity Stakes and Task Delegation Level as independent factors that modulate intensity but don't determine each other. The S3 Ego Shock table (Stakes × D-Level) correctly shows that intensity is a function of both, not that one implies the other.

### 5. ⚡ marker consistency

7. **S2T Trust Evaluation should carry ⚡ but doesn't.** Rule: "A state carries ⚡ if and only if at least one named external event materially changes the probability of entering or leaving that state." S1 Initial Encounter text states: "⚡ Compressed by: workplace mandates, peer adoption events, compelling demos." Compression of S1 Initial Encounter changes the probability distribution of exit times from S1 Initial Encounter, which directly affects the probability of entrance into S2T Trust Evaluation. If a mandate compresses S1 Initial Encounter, then S2T Trust Evaluation is entered sooner and with higher probability. S2T Trust Evaluation text states: "⚡ No external-event marker: S2T Trust Evaluation is internally driven and is not reliably accelerated or reversed by named external events." But mandates *do* accelerate S2T Trust Evaluation by compressing S1 Initial Encounter. Either add ⚡ to S2T Trust Evaluation with note "Compressed by: workplace mandates that accelerate S1 Initial Encounter," or redefine the rule to "external events that directly trigger or reverse this state (not secondary effects of upstream compression)."

8. **S5 Understanding should carry ⚡ but doesn't.** S5 Understanding transitions include: "→ S3 Ego Shock — regression via external trigger." Capability jumps (a named external event) materially change the probability of exiting S5 Understanding. The rule requires the ⚡ marker if an external event changes entry/exit probability. Add ⚡ marker to S5 Understanding with note "Re-triggered backwards by: capability jumps that invalidate the integrated schema."

9. **S7C Ethical Integration contradicts its own marker.** S7C Ethical Integration text states: "⚡ No external-event marker: S7C Ethical Integration is internally driven. Triggers exist (a public AI ethics incident, a personal moral dilemma) but they *amplify* rather than create the state." This is self-contradictory. The rule is "materially changes the probability of entering or leaving that state." A public AI ethics incident materially changes the probability of *entering* S7C Ethical Integration. The marker rule doesn't distinguish "amplification" from "creation"; any material change in probability triggers the marker. Either add ⚡ to S7C Ethical Integration ("Re-triggered by: public AI ethics incidents, personal moral dilemmas that force reflection"), or redefine the marker rule to explicitly distinguish creation events from amplification events.

10. **S6B Dependent Overuse marker status is ambiguous.** S6B Dependent Overuse is marked "⚡ No external-event marker: S6B Dependent Overuse is internally driven." S6B Dependent Overuse is described as entered from S3 Ego Shock (which is itself triggered by capability jumps). The entry path includes external triggers, yet S6B Dependent Overuse claims no external marker. The model's reasoning is that S6B Dependent Overuse's *maintenance* is internally driven, even though its *entrance* is downstream of external triggers. This is a plausible distinction but not stated in the rule. Clarify whether the ⚡ rule applies to state entrance, state maintenance, or both.

### 6. Conjecture tags

11. **S3 Ego Shock terror management mechanism lacks epistemic label.** The model anchors S3 Ego Shock to "self-efficacy collapse" (Bandura, cited) and "terror management in the loose sense — confrontation with one's own replaceability triggers the same kind of existential discomfort that confrontation with mortality does." Terror management theory in psychology concerns existential threat and mortality salience. Applying it to AI capability threat is a reasonable inference, but it is not cited to existing work on AI and existential threat. The model says "in the loose sense," acknowledging the adaptation, but does not mark this as conjecture. Compare with how generativity (S7F Evangelism) is cited to Erikson and explicitly marked conjecture when extended beyond Erikson's scope. Either add a note "Terror management application to AI replaceability is currently untested," or move to the Limits of operationalization section under "Currently conjecture."

12. **Two-axis dropout model is positioned as operationalized without empirical grounding.** The model introduces the severity axes and proposes the reversibility test as an "operational test." The tone suggests this is a concrete instrument, but the model has not tested it and cannot test it without dropout cases. The reversibility test has known confounds (see finding 14). Mark the section as "proposed operationalization, pending validation," or add a note in Limits: "The two-axis dropout model has been designed but not yet tested. The reversibility test is a candidate protocol, not a validated instrument."

13. **"Most people cycle through the model more than once" is marked conjecture but lacks specificity.** The model states "Regression is normal. Most people cycle through the model more than once as AI evolves" and notes "'more than once' is qualitative. V5 deliberately avoids numerical claims about cycle frequency." This is appropriately marked, but vague — "more than once" could mean 2 or 20. The note doesn't specify what cycling means operationally (does re-entering S2T Trust Evaluation count? does lateral shift within S7 count?). Define cycling in the conjecture note: "A cycle is defined as exiting S5 Understanding+ states, re-entering S1 Initial Encounter or S2, and reaching S5 Understanding+ again." This makes the claim falsifiable later.

### 7. Dropout scoring

14. **Reversibility test conflates recovery of practical function with emotional resolution.** The test says: "Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit." This assumes:
    - **A tool can isolate practical failure.** Often, the tool's failure was entangled with identity threat. An AI that made mistakes *on a high-stakes task* is practical failure plus emotional threat simultaneously. Fixing only the practical side doesn't isolate the emotional driver.
    - **Restarting proves practical severity.** A person might refuse to restart even with a fixed tool because they have internalized the failure (learned helplessness — repeated failure leads to giving up trying) or lost trust. This is emotional residue, not a measure of original practical severity.
    - **The two axes are truly independent in dropout cases.** Many dropouts are described as "the tool failed *and* I felt terrible about it." Severing practical and emotional severity artificially might not map to actual experience.

    Example: a person drops out because "AI made high-stakes errors and I lost confidence in my own judgment" (mixed practical plus emotional). You give them a better AI tool for low-stakes tasks. They restart for low stakes. The test concludes "practical severity was high." But the original dropout's practical failure was entangled with identity threat; the restart isn't proof of original severity, it's proof they can recover at lower stakes.

15. **Qualitative descriptions are too loose for ±1 inter-rater agreement.** The model provides four regions: high practical / low emotional ("Tool genuinely doesn't work"); low practical / high emotional ("Identity threat or exhaustion"); high practical / high emotional ("Mixed"); low / low ("Boredom, indifference, opportunity cost").

    For "I tried using AI for my writing, but every time I used it, I felt like I was cheating, and also the outputs were mediocre," two reviewers might score differently:
    - Reviewer A: practical 6 (mediocre outputs), emotional 7 (cheating guilt). Region: high practical / high emotional.
    - Reviewer B: practical 3 (workable with editing), emotional 8 (cheating feeling drives the exit). Region: low practical / high emotional.

    The 0–10 scale allows 11 levels of granularity, but the descriptions provide only 4–5 prototypes. Inter-rater agreement would be ±2–3, not ±1. Provide three concrete reference points (0, 5, 10) per axis with specific examples:

    Practical severity: 0 = tool works perfectly; 5 = intermittent failures (1 in 3 outputs requires heavy editing), workable; 10 = systematic failure on core task, unusable.

    Emotional severity: 0 = no identity concerns, dropped out due to opportunity cost; 5 = mild discomfort about role or authenticity, manageable; 10 = severe identity threat, person describes the tool as threatening their sense of self.

## Recommendations

1. **Fix S7C Ethical Integration marker contradiction (finding 9).** Add ⚡ marker or redefine the rule to disambiguate amplification from creation. Do this before the next version is circulated; the contradiction undermines confidence in the entire ⚡ system.

2. **Clarify ⚡ rule scope (findings 7, 8).** Decide whether the rule applies to direct triggers only or also secondary effects of upstream compression. Audit all states against the clarified rule. Add ⚡ to S2T Trust Evaluation and S5 Understanding, or revise their descriptions to match a narrower rule.

3. **Make S2T Trust Evaluation/S2D Defensive Resistance fork asymmetry explicit (finding 5).** Acknowledge that S2T Trust Evaluation has a direct path to S5 Understanding while S2D Defensive Resistance requires emotional processing. This doesn't invalidate the "no implied order" claim, but explains why the two forks feel structurally different.

4. **Mark S3 Ego Shock terror management mechanism clearly (finding 11).** Add a note that terror management application to AI replaceability is untested and should be treated as a proposed mechanism, not a confirmed one.

5. **Define S6 and S7 multi-occupancy boundaries (findings 3, 4).** State explicitly: "S6 and S7 states are not simultaneous occupancy pairs" and "S3B Bargaining and S7A Maturity are mutually exclusive within the same domain but can coexist across domains."

6. **Operationalize dropout scoring with reference points (finding 15).** Provide concrete 0/5/10 anchors for both axes. Test inter-rater agreement on 5–10 real dropout cases; if ±1 not achievable, adjust the scale or descriptions.

7. **Reframe S6A Enthusiastic Overuse exit mechanism or anchor (finding 1).** Either specify a satiation or plateau condition that makes variable-reward engagement naturally end, or switch the anchor to "novelty-driven exploration."

8. **Revise two-axis dropout model epistemic status (finding 12).** Mark the axes and reversibility test as "proposed" rather than "operational." Frame them as a tool to *explore* dropout cases, not to *measure* them definitively.
