# Falsifiability Review — Model4

Reviewer lens: Prompt B from [005-prompts-v4.md](../005-prompts-v4.md). Treat the model as a scientific hypothesis. Ask what would falsify it. Operationalize the four key distinctions, or admit they can't be operationalized.

Source: [Model4.md](../../Model/v4/Model4.md).

---

## TL;DR

- **The headline falsifiability claim is weak.** V4 added explicit "falsifiable markers" to S3B and S7A. They are in-principle testable but not operationalized. They depend on a triggering event (model release) and on attributing intent ("reflexive" vs "evidence-driven"), which is itself a judgment call.
- **S2 vs S1.5 has no observable test in a single encounter.** Both states show the same surface behavior (probing, listing weaknesses). The only credible separator — asymmetric updating on positive evidence — needs repeated measures over weeks.
- **S6B vs S7D is a non-problem stated as a problem.** They have *opposite* behavioral signatures (heavy use vs withdrawal). The real confusion is longitudinal (S6B people who later collapse into S7D), and that's solvable with usage telemetry.
- **The emotional/practical dropout split is operationally fragile.** The model insists confusing them leads to wrong interventions, but most real dropouts are mixed, and classification depends on the dropout's self-report of internal state.
- **Several claims in V4 are unfalsifiable as written.** The intensity formula (`baseline × Identity Stakes × Task Delegation Level`) has no units. The "internal reframing + social normalization" requirement for S5 stability is unfalsifiable. The S7F-without-S3 collapse claim is post-hoc.
- **You do not need a V5.** The fixes are mostly local: sharper markers with study protocols, delete the pseudo-formula, mark unfalsifiable claims as scoped or speculative, add a "Limits of operationalization" section. Save V5 for when actual empirical data forces structural change.

**Verdict:** V4 is structurally sound but oversells its empirical rigor. The word "falsifiable" appears twice in the model and both uses are aspirational, not delivered. Most of the model's claims are descriptive scaffolding rather than testable predictions, and that's fine — but V4 should say so plainly instead of dressing scaffolding up as hypotheses. **Patch to V4.1 rather than ship V5.**

---

## Contents

1. [The four distinctions](#1-the-four-distinctions)
2. [Other unfalsifiable claims](#2-other-unfalsifiable-claims)
3. [Recommendations](#3-recommendations)
4. [Should you ship V5?](#4-should-you-ship-v5)

---

## 1. The four distinctions

### 1.1 S2 (Defensive Resistance) vs S1.5 (Trust Evaluation)

**Behavioral overlap.** Both states involve the same surface activity: the user runs tasks against the AI, compares output to their own, lists weaknesses. The model's only conceptual separator is *intent* — S2 is "ego defense," S1.5 is "rational assessment." Intent is not directly observable.

**The closest measurable signal: asymmetric updating.**

- S1.5 updates on evidence in both directions. A clear win shifts the verdict toward adoption; a clear loss shifts it away.
- S2 discounts positive evidence ("it got lucky," "easy case," "the prompt was leading") and amplifies negative evidence.

This is testable, but only with **repeated measures over weeks** and a paired design (same user evaluating multiple AI outputs of varying quality). Single-encounter classification is not credible.

**Other proposed signals:**

- *Criterion drift.* S1.5 sets pass/fail criteria up front and holds them. S2 keeps moving the goalposts as the AI clears them. Observable in writing, conversation logs, or interview if the criteria were ever stated.
- *Affect markers.* S2 carries defensive language ("just a", "merely", "trick", "stochastic parrot") at higher rates than S1.5. Lexical analysis of written feedback could differentiate.
- *Attention asymmetry.* S2 reads outputs for failure modes; S1.5 reads for fit. Could be measured in time-on-passage if you had eye-tracking or annotation logs — most settings will not.

**What the model gets wrong.** The model's definition of S2 ("identity protection, not objective evaluation") puts the falsifiability burden on the analyst's ability to know what's "objective." That's not a measurement, it's an editorial judgment.

**Verdict on this distinction.** Operationalizable, but only longitudinally and only with explicit study design. Not separable from a single behavioral snapshot.

### 1.2 S3B (Bargaining) vs S7A (Maturity)

This is V4's headline falsifiability claim. The model's own marker:

> S3B: boundaries are renegotiated **under capability pressure** (a new model release crosses the line, and the line moves reflexively).
> S7A: boundaries are revised **only under evidence** (a benchmark, a real-world failure, a controlled comparison).

In principle, this is the right kind of distinction. In practice, it has five problems.

**Problem 1: temporal coupling of pressure and evidence.** Most users in tech do both at once — they read the release notes (pressure) *and* run a few tests (evidence). The marker requires you to attribute which caused the line to move. That attribution is not in the data; it's an interpretation overlaid on the data.

**Problem 2: self-report contamination.** Anyone in S3B who has read this model will narrate their own behavior as S7A. The marker is highly suggestible. Any study using interviews after exposure to the model is compromised.

**Problem 3: arbitrary observation window.** "In the week after a major model release" — why a week? Some real testing cycles are months. The window is not justified, and shorter or longer windows would yield different classifications.

**Problem 4: classification void between releases.** The marker requires a triggering event. Between major releases — which can be months — the model has no way to distinguish S3B from S7A. The model is silent about this.

**Problem 5: "reflexive" is interpretive.** "The line moves reflexively" is not a measurement. It is a judgment about a person's deliberation depth, made from outside.

**An operationalization that would work** (rough sketch, not in the model):

- Pre-register each subject's stated boundary ("I don't use AI for X").
- Track the next *N* model releases over 12 months.
- For each release, log: (a) did the boundary change within 30 days, (b) was the change preceded by documented testing on real tasks (artifacts, not memory), (c) what was the stated reason in a same-week interview (before model exposure).
- S3B = boundary moves without documented testing in the window. S7A = boundary moves only after documented testing or doesn't move.

This is doable, expensive, and the model doesn't propose anything like it. The marker is presented as if it's been operationalized when it has been described.

**Verdict on this distinction.** Conceptually defensible, methodologically thin. The model overstates its rigor here.

### 1.3 S6B (Dependent overuse) vs S7D (Burnout / Withdrawal)

The prompt asks to distinguish these. The model itself describes them with **opposite behavior**:

- S6B = "I don't trust my own abilities anymore" → high AI use, low autonomous work.
- S7D = "I need a break" → low or zero AI use.

So in a single snapshot they are easy to tell apart by usage volume alone. The genuine confusion is two cases:

**Case A: longitudinal collapse.** S6B → S7D is a documented path in the model. A person who was over-using AI eventually crashes and withdraws. If you observe them only during the withdrawal phase, you can't tell whether they came from S6B or from a different state (S7B saturation, S6C burnout, S6D peer-pressure exhaustion). Solution: usage telemetry. A timeseries with a high plateau followed by collapse implicates S6B; a tapering or sudden stop without prior peak implicates other paths. **This is operationalizable** with workplace tool logs.

**Case B: confidence vs exhaustion attribution.** Even with telemetry, you can't tell *why* someone withdrew. The model's drivers ("eroded confidence" for S6B, "exhaustion" for S7D) are unobservable internal states. Distinguishing them needs an interview or self-report instrument, and self-report is unreliable here for the same reason as 1.2.

**Verdict on this distinction.** Snapshot distinction is trivial (just count interactions). Driver attribution is not directly observable and requires self-report. The model could be honest about that.

### 1.4 Emotional dropout vs Practical dropout

**The model's claim:** confusing them leads to wrong interventions. Emotional needs psychological support; practical needs better tools or training.

**The operational problem:** classification depends on the dropout's reported reason for stopping, which is exactly the kind of self-report most contaminated by post-hoc rationalization. A user whose tool genuinely failed will often describe the failure in identity terms ("it made me feel stupid"). A user with identity threat will often cite tool failures ("the outputs were bad"). The dichotomy does not survive contact with real cases.

**Signals that could help, ranked by reliability:**

1. **Reversibility test (highest).** Hand the dropout a tool that demonstrably solves their cited failure. If they restart, it was practical. If they don't, it was emotional. Requires actually building or providing the fixed tool.
2. **Comparison-shopping behavior.** Practical dropouts tend to try alternatives (Claude → GPT → Gemini → quit). Emotional dropouts tend to quit the category. Observable from usage logs.
3. **Specificity of complaints.** Practical complaints cite tasks ("it hallucinated three citations in my brief"). Emotional complaints cite categories ("AI is just not for me"). Lexical signal, modest reliability.
4. **Identity-language presence.** Emotional dropouts use first-person identity framing ("I'm a writer, not a prompter"). Detectable in interviews, not strong enough to classify alone.

**The dichotomy itself is suspect.** Most real dropouts are mixed: a tool fails *and* the failure lands in an identity-vulnerable spot. The model presents the split as binary and clean. It isn't. V4 should admit a third bucket — *mixed dropout* — or treat the split as two axes (practical severity × emotional severity) rather than two categories.

**Verdict on this distinction.** Partially operationalizable via the reversibility test and usage logs. The binary framing is wrong. Recommend axis representation.

---

## 2. Other unfalsifiable claims

These are claims in V4 that no observation could refute, regardless of the four distinctions above.

### 2.1 The intensity formula

> Emotional intensity in any state = baseline × Identity Stakes × Task Delegation Level.

This looks like math. It isn't. There are no units, no scale, no prediction. "Baseline" is undefined. "Identity Stakes" has two values (low/high), and "Task Delegation Level" has four (D1–D4). Multiplying a binary by a 4-level ordinal by an undefined baseline produces a number that means nothing. The table that follows ("mild surprise," "vertigo," "existential") is a qualitative gloss, not a formula output.

**Either delete the formula or specify it.** Specifying it means: define baseline, define a measurable intensity scale (e.g., self-reported on a 1–10), pre-register the multiplicative structure, and run a study to see if the prediction holds. Until then it's decoration.

### 2.2 S5 stability requires "internal reframing + social normalization"

> Mismatch between the two produces lingering discomfort even when the person is functionally adapted.

Whatever discomfort is observed can be attributed to mismatch. Whatever isn't observed means alignment was achieved. There is no specified instrument for either component, no threshold for "mismatch," no defined "lingering." This is not a claim about the world; it is a frame for narrating any outcome.

**Fix:** specify what counts as internal reframing (a self-report scale?), what counts as social normalization (workplace policy + peer behavior + supervisor language?), and what observable would refute the joint requirement (e.g., a stable S5 user with documented internal coherence but in a hostile social environment — the model predicts they shouldn't exist).

### 2.3 The S7F-without-S3 collapse claim

> S7F entered without prior S3 tends to collapse into S6A (enthusiasm without depth) or S6D (pressure-driven advocacy).

This is convenient: any stable S7F person can be retroactively credited with prior S3, and any unstable S7F person can be credited with skipping it. The only way to falsify is a longitudinal study with pre-S7F state tracking, which the model doesn't propose. As stated, the claim is post-hoc.

### 2.4 "Most people cycle through the model more than once"

No count, no time window, no operational definition of "cycle." Could mean anything. Cannot be wrong.

### 2.5 The Cultural Variability section

Every cultural pattern is described as a modulation of intensity, duration, or "dominant flavor." No observation about a specific culture could refute the claim that "core state structure holds" — any deviation gets absorbed into intensity/duration/flavor parameters. This is a research-protection claim, not a research claim.

**Fix:** name one cultural pattern that, if observed, would force structural revision. (Example: "If a culture routinely produces stable S7A users who never passed through S1 — direct entry from S0 — the state machine's required path through Initial Encounter is wrong.")

### 2.6 Adoption Ceiling "optional extension"

The model introduces this construct, then refuses to formalize it, then says it can be added "if a use case requires it." This is an escape hatch. Any case the current model fails to predict can be retrofitted by activating the optional extension. Either commit to it or remove it.

### 2.7 The ⚡ trigger markers

Some states carry them, some don't. There is no rule for when a trigger should be marked. They function as illustrative annotation, not predictive structure. Fine — but the model presents them as if they encode something.

---

## 3. Recommendations

Prioritized. Each is a concrete edit, not an open question.

### Priority 1 — Operationalize or downgrade the S3B/S7A marker

This is the model's headline falsifiability claim. Either:

- **Operationalize it.** Add a "Study protocol" appendix specifying: pre-registered boundary statement, observation window justification, what counts as "documented testing," how to handle the between-release void, and how to defeat self-report contamination.
- **Or downgrade it.** Replace "Falsifiable marker" with "Heuristic distinction" and admit it requires longitudinal data plus interview to apply.

Doing neither is the current state and is the worst option.

### Priority 2 — Delete or specify the intensity formula

If you can't define baseline and an intensity scale, the formula is decoration that pretends to be math. Replace with: "Intensity is shaped by Identity Stakes and Task Delegation Level; the table below gives qualitative anchors."

### Priority 3 — Add a "Limits of operationalization" section

One short section saying plainly:

- Which states can be identified from a single behavioral snapshot (probably S0, S6A by usage volume, S7D by withdrawal).
- Which states require longitudinal data (S2 vs S1.5, S3B vs S7A, S6B trajectory).
- Which states require self-report or interview (S3, S7B, S7C, dropout classification).
- Which claims in the model are descriptive scaffolding rather than testable predictions (most of the cultural and dynamics claims).

This is the single most credibility-improving edit available. It costs little and disarms most of the "you're dressing folk psychology as theory" critique.

### Priority 4 — Replace the binary dropout split with two axes

Practical severity (0–10) × Emotional severity (0–10). Most real dropouts live in the middle. Add the reversibility test as the primary operational instrument.

### Priority 5 — Mark unfalsifiable claims explicitly

For the S5 stability requirement, the S7F-without-S3 claim, the cycling claim, and the Cultural Variability section: add a brief inline note that the claim is currently unfalsifiable and what evidence would change that. Don't delete the claims — they may be true. Just mark them as conjecture instead of result.

### Priority 6 — Resolve Adoption Ceiling

Either define it as a first-class construct with rules for when it applies, or remove the optional-extension paragraph. The half-state is worse than either.

---

## 4. Should you ship V5?

**No.** Ship V4.1 with the six edits above.

**Why not V5.** The structural skeleton of V4 — the state set, the graph, the two axes, the trigger and ambient layers — is not what's broken. None of the findings here demand a new state, the removal of an existing state, a new axis, or a re-graphing. The headline V4 changes (S1.5 promotion, S6 split, dropout mechanism, the markers) are still defensible. What's broken is the *epistemic register*: V4 talks like a tested model and isn't one. That's an editing problem, not an architecture problem.

**When you would ship V5.** Three triggers, any one of which justifies V5:

1. You actually run a study (even a small one, even a survey + telemetry pilot) and the data force a structural change — for example, you find S3B and S7A are statistically inseparable and need to be merged.
2. You add a dynamics layer (transition probabilities, dwell times). That's an architectural change, not a patch.
3. You decide to anchor each state to an existing cognitive-science mechanism (Prompt E in the prompt set). That changes the model's grounding and is a V5-scale move.

Until one of those happens, V4.1 is the correct next release. Patch the falsifiability story; keep the structure.
