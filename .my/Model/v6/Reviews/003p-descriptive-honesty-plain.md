This is a simpler rewrite of [003-descriptive-honesty.md](003-descriptive-honesty.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Descriptive Honesty — Model V6 (Plain Language)

## TL;DR

- The model flags guesses as guesses in the right places, but **transition descriptions and observation notes still read like facts** when they're working theories. "Most people" claims have no guess labels attached.
- The **dropout reversibility test** (offer a better tool; if they restart, the tool was the problem) works for two clean cases, but falls apart when someone quit for both practical and emotional reasons at the same time.
- The **S2T vs S2D asymmetric-updating signal** (do people update their beliefs fairly, or only on bad news?) is well-specified and ready to run — about 60 people, 12–15 months, ~$50–80k.
- The **S3B vs S7M boundary distinction** is stated as a working rule for practitioners, but the data to back it does not exist yet. It needs longitudinal tracking first.
- The **PEN vs S2D three-signal test** is uneven: two signals are observable in the field, and one is not.
- **Clinical claims** ("within range of clinical distress," six-month thresholds) are written as model findings. They are not. They are rule-of-thumb estimates with no research behind them.

## Findings

### 1. Observation notes and transition descriptions sound like facts when they're guesses — not yet tested

The model labels specific testable claims correctly. But the sections that describe how states work — how people move from one state to another — still read as if someone verified them.

Examples:

- S3E (the prolonged identity-disruption state): "Most people who appear to take this path are actually doing accelerated S3E → S3B → S5." This is a claim about how common a particular path is. There is no **Conjecture —** label on it. No data is cited. It reads as fact.
- S3B (the bargaining state, where someone draws a personal line about what AI is "allowed" to do): "Many people remain productively in S3B for years." Sounds observed. Not marked as an estimate.
- S2D (Defensive Resistance — where someone discounts good news about AI and amplifies bad news): "Long-residence S2D in identity-threatened domains is a signal that the org's framing or the person's situation is creating unnecessary identity threat." This is a diagnostic conclusion presented without any qualifier.
- One observation marker says the claim "The position was formed at or shortly after first encounter" is observable. It is — but the model does not say what "shortly after" means. A week? A month? Without a defined window, the observation marker is not usable in practice.

**Fix:** Add a **Conjecture —** or **Testable —** label to every transition description and observation note. Where something is based on what you have seen but not counted, say so: "Qualitative observation suggests...". Where a time window is undefined, say so explicitly: "We have not established how long 'at or shortly after' means." Move clinical thresholds (such as the six-month one from Finding 6) to a separate section clearly marked as practitioner rules of thumb, not model claims.

### 2. The dropout reversibility test works for two cases but breaks on the mixed case — testable (partially)

When someone quits using AI, the model suggests offering them a better tool. If they come back, the practical problem was what drove the quit. If they don't, feelings were driving it.

That works cleanly for:

- **High practical, low emotional:** they restart → the tool was the issue.
- **Low practical, high emotional:** they don't restart → feelings were the issue.

The model does not handle the **high practical, high emotional** case — when both were driving the quit at once. Three problems:

- Switching tools changes how the person frames the task. If they quit ChatGPT for legal writing and you offer Claude for legal writing, they might treat this as a different situation — which hides whether practical or emotional was the bigger driver.
- The emotional load at the time of quitting may have faded by the time you offer the better tool. If stress dropped on its own, the new tool gets credit it did not earn.
- Even if the practical side was the main reason, restarting carries a social cost: "I said I was done with AI and now I'm back." That can block a restart even when the tool genuinely solves the problem.

**Fix:** Reframe this as a **two-step diagnostic, not a one-step test.** Step 1: watch whether they restart (tells you which axis was heavier). Step 2 (if they do restart): ask them what the emotional situation felt like at the time of quitting versus now. State explicitly in the model: "This test identifies which axis was dominant, but it does not measure the ratio in mixed cases. High-practical/high-emotional quitters require follow-up conversation, not just a tool offer."

### 3. The S2T vs S2D asymmetric-updating signal is ready to study — testable

S2D (Defensive Resistance) people discount positive evidence about AI and amplify negative evidence. S2T (Trust Evaluation) people update their beliefs in both directions roughly equally. Both state files flag this as **Testable —**, with a note that multiple evaluation points are needed.

This is well-specified. Here is how you would run it:

**Study design:** Measure baseline beliefs about AI on a task relevant to the subject. Show subjects AI successes and failures (videos, real outputs, benchmarks). Measure updated beliefs. Repeat quarterly across three to four model releases. Calculate asymmetry: (how much beliefs shift on good news) divided by (how much they shift on bad news). For S2T this ratio should be close to 1.0. For S2D it should be above 2.0.

**Sample size:** About 30–40 people per state. Trained raters pre-classify S2T vs S2D using the observation markers.

**Time horizon:** 12–15 months (three to four model release cycles).

**Cost estimate:** ~$50–80k (participant payments at $50–100 per session, rater training, online testing platform, analysis).

**Fix:** None needed. Move this to a "Ready for Study" section in `limits-of-operationalization.md`.

### 4. The S3B vs S7M boundary heuristic is overstated — testable (with caveats)

S3B (Bargaining) and S7M (a sub-state where someone allocates AI based on careful evidence of where it actually performs well) both look like "I use AI for some things but not others." The model gives practitioners two signals to tell them apart:

- **Where the boundary sits:** if it follows the person's professional identity (for example, "AI can help with admin but not my actual craft"), it suggests S3B. If it follows where AI is genuinely reliable versus unreliable, it suggests S7M.
- **How the boundary moves:** S3B people shift it quickly when capability pressure builds, without testing. S7M people shift it only after checking whether the new model is actually better at the relevant task.

Both signals are marked **Conjecture —**, which is correct. But the "working heuristic for practitioners" that follows reads as a usable field tool right now — and it is not. Four problems:

- "Where the boundary sits" depends on asking people which part of their identity feels threatened versus what they are actually evaluating AI's performance on. Self-report on that question is unreliable.
- "How the boundary moves" needs at least two measurement points around a capability shift — a new model release, a published benchmark, a peer demonstration. The model does not define what counts as "measured evidence" or how long a window to use.
- Someone can look like S3B from the outside (boundary tracks their professional identity) while moving it only on evidence (internal behavior of S7M). The model calls this a "transitional shape" but does not say whether it is its own diagnostic category or just measurement noise.
- Saying an S3B person moves the boundary "quickly without documented testing" requires observing the absence of testing. The baseline level of rigor expected is never defined.

**Fix:** Rewrite the S3B vs S7M section with three explicit levels: (1) "We observe two broad patterns" — the boundary difference. (2) "The movement pattern is a testable distinguisher, but testing it requires longitudinal tracking across model releases" — the methodology, with time windows specified. (3) "The working heuristic for practitioners" — a screening tool, not a diagnosis, with an explicit note: "Definitive classification requires timeline data." Define what "measured evidence" means operationally — for example, a benchmark result, a controlled A/B comparison, or documented observation of the new model performing the relevant task.

### 5. The PEN vs S2D three-signal test is uneven: two signals work, one doesn't — testable (with reduced claims)

PEN (a principled values-based objector — someone who declines AI because of genuine ethical concerns, not because AI threatens their professional identity) and S2D (Defensive Resistance — someone who declines AI because it makes them feel displaced or inadequate) can look identical from the outside. The model proposes three signals to tell them apart:

1. **Cross-domain consistency:** Does the same objection apply across different uses of AI, or only the ones that directly touch the person's work?
2. **Evidence response:** When AI gets meaningfully better, does the ethical concern get sharper — or does the defensive position just tighten further?
3. **Emotional register:** Moral conviction and contempt (suggests PEN) versus anxiety and a sense of threat (suggests S2D).

The first two signals are observable. The third is not — at least not reliably.

Cross-domain consistency: if someone objects to AI for writing (citing data ethics) but uses it freely for spreadsheets, that is a signal it is personal to their craft, not a principled ethical stance. Observable.

Evidence response: show them a meaningfully better AI model. If the ethical concern sharpens ("this makes the data privacy issue worse, actually"), that suggests PEN. If the defensive stance tightens ("they keep getting better, which is even more concerning"), that suggests S2D. Also observable.

Emotional register: this requires an interview. And it conflates two different things — what state someone is currently in (are they PEN or S2D right now?) versus what kind of person they generally are (do they tend to run anxious or do they tend to run morally driven?). A person can have genuine moral conviction and anxiety at the same time. The signal does not separate those.

The model acknowledges "most real cases are mixed," but the three-signal frame implies the signals are independent, clean separators. They are not.

**Fix:** Label the three-signal frame as "indicators with known limitations," not "diagnostic separators." Specifically: "Cross-domain consistency and evidence response are observable in the field. Emotional register requires dialogue and has high error rates — someone can have genuine moral conviction and anxiety underneath it at the same time. In mixed cases, treat these signals as probabilistic pointers, not conclusions." In `limits-of-operationalization.md`, mark emotional register as "interview-only, high contamination," not "snapshot-observable."

### 6. Clinical thresholds in the healthiness sections are presented as model findings — they are not — not yet tested

S3E's healthiness section says:

> "Identity disruption that does not resolve after six or more months is within the range of clinical distress, not ordinary adaptation discomfort, and may warrant a referral consideration."

This is written as if the model derived it. It did not. The six-month threshold:

- Is not based on data collected for this model.
- Has not been checked against standard clinical diagnostic systems (such as DSM or ICD — the manuals clinicians use to define mental health conditions).
- Is not drawn from existing research on occupational stress or identity disruption, even though that research exists.
- Is a practitioner rule of thumb — someone's working estimate, not a measured finding.

The same applies to S3E's observation note: "A practitioner should look for whether the person is moving through S3E within weeks to months." That window is stated without any data behind it.

**Fix:** Move all clinical thresholds (the six-month window, "range of clinical distress," "weeks to months") into a subsection clearly labelled **Practitioner heuristic, not validated.** Add a disclaimer: "These thresholds are based on field experience, not longitudinal studies. Use them as rough signposts, not cutoffs. If you are worried about someone's wellbeing, refer to a mental health professional. Do not use this model as a diagnostic instrument." Remove the six-month claim entirely unless you have actual longitudinal data to support it. Replace "within weeks to months" with something actionable: "Look for whether the person is actively engaging with AI — seeking peer input, trying new tools, reading about it — or withdrawing further. Speed varies widely."

### 7. Identity Stakes has no measurement guide — not yet tested

The axes file says:

> "Role-identity centrality (how central a role is to someone's sense of who they are) is offered as vocabulary for thinking about Identity Stakes, not as a tested cause of threat."

That framing is honest. But the table under Identity Stakes uses concrete-sounding categories — "core part of self-concept" — without telling anyone how to assess them in practice. A practitioner trying to decide whether a specific person's stakes are high or low has nothing operational to work with.

Example: Is a senior copywriter's professional identity more threatened by AI-generated copy than a senior architect's is by AI-generated designs? Probably yes — writing is more directly commodified right now. But the model does not give you a way to check. Is it years in the role? How much of their reputation depends on the skill? Economic fragility if the skill is automated? None of these are specified.

**Fix:** Add an operational note under Identity Stakes: "To quickly assess stakes in a specific domain, ask the person to finish this sentence: 'If AI could do this as well as I can, it would mean ___.' High-stakes answers are identity-level: 'it would mean I'm not really a [job title] anymore.' Low-stakes answers are capability-level: 'it would mean I need to learn new tools.' This is practitioner scaffolding, not a validated instrument."

## Recommendations (priority order)

1. **Add Conjecture / Testable markers to all observation notes and transition descriptions.** This is the core honesty problem. Unmarked assertions in observation sections will be read by practitioners as established fact.

2. **Move clinical thresholds (six-month window, "range of clinical distress") out of state definitions and into a clearly labelled disclaimer section.** They exceed what the model can actually claim.

3. **Rewrite S3B vs S7M as longitudinal-observable, not a working heuristic for snapshot triage.** Add explicit notes on what methodology is required and what time windows apply.

4. **Clarify the dropout reversibility test's limits on the high/high case.** State clearly that the test identifies which axis was dominant but requires follow-up for mixed cases.

5. **Downgrade the PEN vs S2D emotional-register signal to "high-error indicator."** Note that a person's current state and their general personality type are two different things, and this signal conflates them.

6. **Spec out the S2T/S2D study protocol and move it to "Ready for Study" in limits-of-operationalization.md.** This one is ready to run. Moving it signals honest confidence in the claim.

7. **Add operational guidance for assessing Identity Stakes.** The current framing is honest but gives practitioners nothing concrete to act on.
