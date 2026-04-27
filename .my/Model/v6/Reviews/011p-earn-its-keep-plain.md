This is a simpler rewrite of [011-earn-its-keep.md](011-earn-its-keep.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Earn-Its-Keep Audit — Model V6 — Plain Language

## What "earn its keep" means here

Every concept in the model should do at least one useful thing. This audit checks each concept against three questions:

1. **Does it explain something?** Does knowing this concept help you predict what a person will do?
2. **Can you use it?** If you're watching a real person, can you apply this concept without asking them directly what they're feeling?
3. **Can you prove it wrong?** Is there a test you could run whose result would force you to throw this concept out?

A concept that scores zero on all three doesn't belong in the model.

## TL;DR

- The **permanent-non-user reading of S0** scores zero on all three. It's not a concept — it's just a label for "this person is outside the model." Delete it or move it to a "scope limits" document.
- **Healthiness levels** (the file that says S7M is "sustainable" and S6D is "corrosive") are editorial comments, not model content. They don't predict anything the model doesn't already predict. Delete them or move them to a practitioner guide.
- **S7I, S7E, and S7V** look identical to S7M from the outside — you can only tell them apart by asking the person directly. That makes them unmeasurable. Consider merging them with S7M or treating them as variations of S7M rather than separate states.
- **Delegation Ceiling** is a guess with no measurement instrument and no test. It adds no prediction the model doesn't already make. Delete it or park it in "future research."
- The **S3E → S5 direct edge** (skipping the bargaining step) is indistinguishable from fast S3E → S3B → S5 on any single observation. Remove the edge; it does no work.
- **PEN Pre-emptive Non-Adoption** (someone who rejects AI on ethical grounds before seriously testing it) is hard to distinguish from S2D Defensive Resistance (someone rejecting it to protect their identity). The model's own three signals are weak and often mixed. Consider whether this is a separate state at all.
- **S3X Structural Displacement** (someone concludes their entire role is becoming non-viable) has three proposed outcomes, all marked as guesses and not tested. It's more of a dropout sub-label than a real state. Demote it.
- The **⚡ trigger system** names events that can push people into new states, but the model doesn't use those names to make any actual predictions. Useful as a reference list, not a load-bearing part of the model.

## Audit Table

| Concept | Explains something? | Useful to practitioner? | Can be proved wrong? | Verdict |
|---|---|---|---|---|
| S0 Baseline (transition) | ✓ | ✓ | ✓ | **PASS** |
| S0 Permanent non-user | ✗ | ✗ | ✗ | **FAIL** |
| S1 Initial Encounter | ✓ | ✗ | ✗ | **WEAK** |
| S2T Trust Evaluation | ✓ | ✓ | ✓ | **PASS** |
| S2D Defensive Resistance | ✓ | ✓ | ✓ | **PASS** |
| S3E Ego Shock | ✓ | ✓ | ✓ | **PASS** |
| S3B Bargaining | ✓ | ✓ | ✓ | **PASS** |
| S3X Structural Displacement | ✗ | ✗ | ✗ | **FAIL** |
| S5 Understanding | ✓ | ✓ | ✓ | **PASS** |
| S6E Enthusiastic Overuse | ✓ | ✓ | ✓ | **PASS** |
| S6D Dependent Overuse | ✓ | ✓ | ✓ | **PASS** |
| S6R Driven Overuse | ✓ | ✓ | ✗ | **PASS** |
| S6S Social Overuse | ✓ | ✓ | ✗ | **PASS** |
| S7M Maturity | ✓ | ✓ | ✓ | **PASS** |
| S7I Identity Expansion | ✗ | ✗ | ✗ | **FAIL** |
| S7E Ethical Integration | ✗ | ✗ | ✗ | **FAIL** |
| S7B Burnout | ✓ | ✓ | ✓ | **PASS** |
| S7V Evangelism | ✗ | ✗ | ✗ | **FAIL** |
| PEN Pre-emptive Non-Adoption | ✗ | ✗ | ✗ | **FAIL** |
| Identity Stakes | ✓ | ✓ | ✓ | **PASS** |
| Task Delegation Level | ✓ | ✓ | ✓ | **PASS** |
| Delegation Ceiling | ✗ | ✗ | ✗ | **FAIL** |
| Per-domain scoping | ✓ | ✓ | ✓ | **PASS** |
| Dropout two-axis | ✓ | ✓ | ✓ | **PASS** |
| Reversibility check | ✓ | ✓ | ✓ | **PASS** |
| ⚡ Trigger system | ✗ | ✗ | ✗ | **FAIL** |
| S2T → S2D edge | ✓ | ✓ | ✓ | **PASS** |
| S3E → S5 edge | ✗ | ✗ | ✗ | **FAIL** |
| Healthiness levels | ✗ | ✗ | ✗ | **FAIL** |

---

## Findings

### 1. S0 permanent-non-user reading fails all three tests

S0 is where everyone starts — no AI engagement yet. V6 adds a reading of S0 for people who *stay* there permanently: they never engage with AI and never will. The model tries to distinguish these people from S2D Defensive Resistance (not engaging because AI feels threatening) and from PEN (not engaging on ethical grounds). The permanent non-user, V6 says, has "simply not engaged and will not."

Here's why that's not a useful concept:

- **Explanatory power — zero.** This reading doesn't predict what the person will do, because the person does nothing. It doesn't help you understand anything about them.
- **Operational use — zero.** V6 itself says the model shouldn't predict that everyone eventually engages. So when a practitioner meets one of these people, the model says: you're outside our system. No intervention, no lever, no guidance.
- **Can it be proved wrong — no.** "This person has not engaged" is just a description. There's no claim about them that could turn out to be false.

This is a **scope boundary** dressed up as a state. It says "this model doesn't apply here" — which is fine, but that note belongs in a "who this model covers" document, not in the model itself.

**Fix:** Delete the permanent-non-user reading from S0. Put it in [populations.md](populations.md) as an explicit note: "This model doesn't apply to people who never encounter AI. They're outside the adoption trajectory." Don't present it as a state.

### 2. S3X Structural Displacement fails — or barely passes on explanatory power

S3X is the state someone reaches when they conclude that viable AI-collaborative work no longer exists in their field. Maybe their role got automated away. Maybe their clients disappeared. Entry comes from external confirmation (job elimination, client collapse) or from giving up after S3B Bargaining repeatedly failed.

The problems:

- **Explanatory power — weak.** S3X explains that when a job disappears, the job is gone. That's not psychology — it's a description of the labour market. The model itself concedes: "The model does not predict which roles become economically non-viable, or when. That is an economics question." So what does S3X predict about how the person actually behaves? The file lists three outcomes — transition to another field, exit entirely, or become an advocate against AI — but all three are marked **Conjecture** ("not validated against a representative sample of displaced workers"). If the outcomes are guesses, what does S3X predict?

- **Operational use — very weak.** The file frames S3X as a useful label: it tells a practitioner "this is no longer a psychology problem, it's an economic one." But then what? The model offers no intervention. Compare that to S3E (support the person's identity work) or S6D (help them rebuild self-trust) — those are actionable. S3X is basically a referral slip to another discipline.

- **Can it be proved wrong — weak.** Three claimed outcomes, none tested. The "adversarial-advocacy track" isn't even fully described yet.

There's also a structural problem: S3X bundles together an identity crisis (S3E) and a labour-market fact. That's worth naming, but it doesn't follow that S3X is its own state rather than a label for "S3E plus an economic event hitting at the same time." A simpler model would say: S3E + structural non-viability = dropout at the emotional axis or the practical axis. S3X adds a third category that predicts nothing extra.

**Fix:** Demote S3X from a full state to a **labelled dropout subtype**. Rename it "S3E + Structural Non-Viability (layered dropout)" and move it into [dropout.md](dropout.md) as a special case. This keeps the recognition that two crises compound, without claiming a separate state. If the three-outcome typology ever gets tested, promote it back. For now it's an observation, not a prediction.

### 3. S7I Identity Expansion fails — looks identical to S7M from the outside

S7I is defined as: the person develops capabilities they couldn't produce alone and starts to partly define who they are through that expanded output. S7M is: calibrated, sustainable AI use with bounded scope.

The model itself admits the core problem: "the distinction between S7M and S7I is internal — both look like 'uses AI competently' from outside. Confirming the distinction requires self-report" (asking the person directly what they feel).

Why that's a failure:

- **Explanatory power — undermined.** If a practitioner can't distinguish S7M from S7I by watching behaviour, the distinction predicts nothing different. Both lead to the same places — S7B Burnout, regression to S3E on a major capability jump. Both are "sustainable."
- **Operational use — zero.** The only tool the practitioner has is to ask "do you partly define yourself through this expanded capability?" But if the person has read the model, their answer will be in model terms and is useless. The file admits this: "the distinction is contaminated by self-report once a subject has read this model."
- **Can it be proved wrong — no.** The file marks it as Conjecture. There's no specified test that doesn't rely on asking the person.

This is a conceptual distinction with no observable footprint. It can't be measured and can't be disproved.

**Fix:** One of three options: (a) find a **behavioural signal** that distinguishes S7I without self-report — for example, the person starts working in entirely new domains where they had no prior skill, or their public self-description shifts to include AI partnership; (b) merge S7I and S7M into "S7 Integration" with a note that some people are expanding their identity through it and some are maintaining it, but both look the same from outside and are both stable; or (c) demote S7I to a **modulation of S7M** ("Identity Expansion modulation") rather than a separate state.

### 4. S7E Ethical Integration fails for the same reason as S7I

S7E is defined as: sustained reflection on AI's ethical implications — bias, intellectual property, authenticity, labour displacement, environmental cost, societal effects. The file says it "rarely appears as a sole end state" and "most often co-occurs with S7M or S7I." It also admits: "the line between healthy S7E and rumination (repetitive, unproductive worry) is qualitatively understood but not operationally specified."

The failure:

- **Explanatory power — weak.** Does S7E predict a different outcome than S7M? No. Both are sustainable. Both can tip into S7V. Both regress on major capability jumps. The difference is what's going on inside the person's head, not what they do.
- **Operational use — very weak.** A practitioner sees someone in a stable end state. To know whether it's S7M or S7E, they have to ask "are you thinking about ethics?" That's self-report. And if someone is in S7M and also reflecting on ethics, does that make them S7E? The file admits the distinction is hard: "S7E is rarely a sole end state."
- **Can it be proved wrong — weak.** The file says "the line between healthy S7E and rumination is qualitatively understood but not operationally specified." That's an admission that the boundary is fuzzy and unmeasured.

Worse: S7E is defined by what someone is *thinking* (ethical content), not by what they *do* differently. A state defined by thought content with no behavioural difference is unmeasurable.

**Fix:** Merge S7E into S7M as a modulation: "Some S7M users also engage in ethical reflection (S7E modulation)." Or, if ethical reflection is supposed to matter, specify a concrete behavioural marker. For example: does the person make visible decisions about what *not* to delegate? Do they articulate those constraints publicly? Do their actual delegation patterns differ from S7M? Until there's a behavioural marker, S7E is just "reflective S7M," not a separate state.

### 5. S7V Evangelism is a role or modulation, not a state

S7V is defined as: the person's identity becomes partly defined by guiding others through AI adoption. The model lists four ways someone gets there — through prior S3E Ego Shock, through S7I Identity Expansion, through a professional role, or through a desire to help others grow.

The structural problem:

- **Explanatory power — questionable.** What does S7V predict that S7M, S7I, or S7E don't already predict? The same transitions: regression on a major capability jump, burnout. The teaching and advocacy work is layered on top of some other underlying state, not a state in itself.
- **Operational use — weak.** A practitioner sees someone teaching others about AI. Does that tell them anything about the person's own state? No. Someone in S6D (dependent, anxious overuse) can evangelize. Someone in S6E (enthusiastic overuse) often does. Someone in S7M might. S7V describes a **role** — mentor, speaker, advocate — not a psychological state.
- **Can it be proved wrong — weak.** The claim "S7V without real depth collapses under hostile questioning" is testable in principle but describes a failure mode, not a stable-state prediction.

V6 also walks back a V5 claim. V5 implied S7V required prior S3E. V6 says: "S7V is *more common* among people with prior S3E, but stable S7V without prior S3E also exists." If you're dropping the requirement, S7V is becoming less defined, not more. The evangelist role can sit on top of any end state.

**Fix:** Rename S7V as "End-State Advocacy Modulation" and move it out of the state graph. Or keep it, but reframe it as an overlay: instead of "S7M → S7V," say "S7M occupants can take on an evangelism role." The current structure treats it as a state, but the model does no work specific to it — it's just "S7M + teaching."

### 6. Delegation Ceiling is a pure guess with no measurement and no test

The Delegation Ceiling is "the maximum amount of AI involvement a person can accept for tasks in their core identity domain, given their current state and history." The file explicitly marks it as **Conjecture**: "No measurement instrument currently exists for it. The construct is offered as vocabulary for a phenomenon practitioners report but is not empirically validated."

The three tests:

- **Explanatory power — weak to zero.** The concept is used exactly once: to explain what the file calls "coerced S5 Understanding" — where someone appears to integrate AI normally but hasn't changed their ceiling, so the resistance resurfaces later. But the model already predicts this. Someone who reaches S5 Understanding while still defending against high-delegation tasks will regress when pushed further. That's already in the model via S3B → S5 with a retained boundary, then regression. The ceiling adds a word, not a prediction.
- **Operational use — zero.** No measurement instrument exists. A practitioner cannot assess someone's ceiling. No intervention is keyed to it. It's purely retrospective: after someone regresses, you can look back and say "they had a ceiling." But you couldn't have predicted it beforehand.
- **Can it be proved wrong — no.** No specified test. The file describes it as vocabulary for something practitioners informally observe. Informal vocabulary for an observed phenomenon is not a model element; it's folk knowledge.

**Fix:** Delete it. Or, if practitioners genuinely find the vocabulary useful, move it to [limits-of-operationalization.md](limits-of-operationalization.md) as an aspiration: "Future research might develop an instrument to measure delegation ceiling. For now, it is vocabulary." Don't include it in the core model.

### 7. S0 permanent-non-user reading — already covered in Finding 1

This is a duplicate of Finding 1, included for completeness.

**Fix:** As in Finding 1 — delete or move to [populations.md](populations.md).

### 8. Healthiness levels don't meet any criterion — they're editorial commentary

The [healthiness.md](healthiness.md) file provides an interpretive layer that rates states on sustainability. S7M is "sustainable." S6E is "sustainable with cost." S3E is "transitional only." S3X is "legitimate, not pathological."

The three tests:

- **Explanatory power — zero.** The healthiness labels don't predict anything. They interpret what the model already predicts — sustainability, transition requirements, regression risk — and add moral weight to those predictions.
- **Operational use — weak to none.** The file tells a practitioner "S7M is healthy; S6D is corrosive." But the model already says S6D causes self-trust erosion and leads to S7B Burnout. The label "corrosive" adds a value judgment, not an intervention.
- **Can it be proved wrong — no.** The file explicitly disclaims model status: "This file is interpretation. The model itself is descriptive. Healthiness labels above are a reading, not a model claim." If it's not a model claim, it shouldn't be in the model.

The deeper issue: V6 is descriptive — it describes what people do, not what they should do. Normative judgments (good, bad, healthy, corrosive) don't belong in a descriptive model. If practitioners find the healthiness labels useful, that's a practitioner-guide responsibility, not a model responsibility.

**Fix:** Delete [healthiness.md](healthiness.md) or move it to an optional "practitioner guide" outside the core model. If kept, retitle it "Practitioner interpretation layer — not a model claim" and keep it clearly separate from [Model6.md](Model6.md). Don't link it from the core model.

### 9. The S3E → S5 direct edge can't be distinguished from S3E → S3B → S5

The state graph includes a direct edge from S3E (Ego Shock) to S5 (Understanding), skipping S3B Bargaining. It's marked "(rare)" and the model itself says: "Most people who appear to take it are actually doing accelerated S3B and revisiting it later. Distinguishing the direct path from a fast S3E → S3B → S5 path requires longitudinal observation; on a single observation the two are indistinguishable."

Why this fails:

- **Explanatory power — undermined.** If two paths look identical and you can't tell them apart without months of data, the distinction adds nothing to a practitioner or researcher watching in real time.
- **Operational use — zero.** A practitioner sees someone move from S3E to S5. Which path did they take? The model says you can't know without extended observation. The direct edge tells the practitioner nothing.
- **Can it be proved wrong — the model admits defeat.** "On a single observation the two are indistinguishable." In a descriptive model, if two paths look the same on every observation you can practically make, they are the same path. Drawing them separately on the graph misleads more than it helps.

**Fix:** Delete the S3E → S5 edge. Rewrite the S3E section to say: "S3E typically leads to S3B (negotiated scope) or dropout. Some people move through S3B very quickly and reach S5 fast. The distinction between rapid S3B → S5 and a direct jump can't be made on a single observation and shouldn't be drawn as a separate edge."

### 10. PEN Pre-emptive Non-Adoption is diagnostically fragile and may just be S2D with ethical language

PEN is the state someone reaches at or just after their first encounter with AI, where they decide not to adopt it based on values — not because they tested it and found it lacking, not because it felt threatening, but because it conflicts with what they stand for. The model distinguishes PEN from S2D Defensive Resistance (where someone does form a defensive stance against a perceived threat) and from S0 permanent non-use (no active reasoning involved at all).

The model offers three signals for telling PEN from S2D:
1. Cross-domain consistency — are the ethical concerns the same across all technology, or only AI?
2. Evidence response — when shown counter-evidence, do they update at all, or stay completely firm?
3. Emotional register — is the response calm and principled, or anxious and defensive?

Then it adds: "Most real cases are mixed."

The three tests:

- **Explanatory power — questionable.** Does PEN predict a different outcome than S2D? No. Both lead to stable non-adoption (or slow drift between S2D and S2T). Both resist capability evidence. If the end states and transitions are the same, is PEN a separate state or just S2D with a different internal story?
- **Operational use — very weak.** The practitioner applies the three signals and finds a mixed case. The model concedes: "A person can be simultaneously in S2D (protecting competence) and making genuine ethical arguments that are also true and genuinely held." If most cases are mixed and can't be unmixed, the distinction doesn't work in practice.
- **Can it be proved wrong — weak and slow.** One signal is testable — cross-domain consistency over multiple months. But "multiple months" isn't practical for most real-world observations. The other two signals (emotional register, evidence response) are qualitative and subjective. The file itself says: "none reliable on a single observation."

The deeper problem: S2D Defensive Resistance is defined as using your intelligence to protect your identity rather than to find the truth — you update asymmetrically, accepting evidence that confirms what you already believe and dismissing evidence that challenges it. PEN is defined as prioritising a values-based identity. Both protect something (competence or values) and both resist evidence. The verbal distinction is clear. The behavioural distinction is not.

**Fix:** One of three options: (a) merge PEN into S2D and note that some S2D cases are grounded in identity threat and others in genuine values conflict — the distinction is internal and can't be reliably observed; (b) find a robust observational signal that distinguishes them without asking the person; or (c) keep PEN but mark it explicitly as "Conjecture — not validated" and move it to limits-of-operationalization. Don't present it as a clean diagnosable state when the model's own diagnostic framing admits confusion.
