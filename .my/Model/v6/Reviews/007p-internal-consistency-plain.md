This is a simpler rewrite of [007-internal-consistency.md](007-internal-consistency.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# V6 Internal Consistency Audit — Plain Language

## TL;DR

- **S6R + S6S contradiction.** Two of the overuse states — S6R (driven by performance targets) and S6S (driven by social pressure) — are described as "can coexist" in one sentence and "are incompatible" in another. Pick one.
- **Delegation Ceiling scope is ambiguous.** The Delegation Ceiling (the upper limit of how much AI work a person can accept) is introduced as a property of the whole person, but every example shows it varying by topic area. Clarify which.
- **Same observable behavior, different confidence labels.** One file tags the S3B-vs-S7M distinguishing signal as "just a hypothesis." The other tags the exact same signal as "testable." Same claim needs the same label.
- **Dropout severity scores have no definitions.** The 0–10 scales for measuring dropout severity have no anchors. Two practitioners rating the same case would produce different numbers.
- **The state diagram is missing a path.** The flowchart shows S0 (Baseline, pre-AI-use) leading only to S1 (first exposure). It doesn't show that S0 can be a permanent end state for people who never adopt AI.
- **Three model properties don't operate at the same level.** Identity Stakes is per-topic area. Task Delegation Level is per-interaction. Delegation Ceiling is ambiguous. If they don't all work at the same level, they can't be combined cleanly.
- **S7V (stable evangelism) has four paths in, but no prediction of stability.** V6 lists four ways someone can reach the evangelism state, but doesn't say how to predict which path someone took or whether they're at risk of collapse.
- **The S6 observation guide works for clean cases. Most cases aren't clean.** Good probes for each overuse state, but the guide itself admits most real cases show signals from multiple states at once — then gives no advice on what to do next.
- V6 is more internally consistent than V5 on most core claims. But five issues (Findings 1, 2, 3, 4, and 5) need fixes before the model is reliable enough to apply consistently.

---

## FINDINGS

### 1. The state graph says S6R + S6S both "can coexist" and "are incompatible" — contradiction

**Location:** [02-state-graph.md](02-state-graph.md#L29-L45), State Occupancy section

The state graph lists these rules for which S6 overuse states can appear in the same person at once:

- S6R (Driven Overuse — uses AI mainly because productivity metrics reward it) and S6S (Social Overuse — uses AI mainly because their team does) **can coexist** in compliance-heavy environments.
- The combination S6R + S6S is **unstable — the affective profiles do not match.**

"Affective profile" means how the person feels emotionally in that state. The text is claiming the emotional signatures of S6R and S6S don't fit together.

The problem: the first bullet says S6R + S6S can appear together. The second says they can't stably appear together. Those are contradictory.

Neither the S6R file nor the S6S file resolves this — both tag coexistence as Conjecture (a hypothesis, not directly tested), not as instability.

A practitioner trying to figure out whether someone can show both S6R and S6S at once will get conflicting instructions from the same document.

**Fix:**

Pick one reading and remove the other. If the intent is that S6R + S6S can coexist briefly but then destabilize, say that: "S6R + S6S can coexist in compliance-heavy environments but is unstable — the pairing collapses without ongoing external pressure." If they're outright incompatible, remove the bullet that says they can coexist.

Either way, define what "unstable" means in concrete terms — for example: "unstable = collapses without ongoing external reinforcement" or "unstable = typically resolves within a few weeks."

---

### 2. Delegation Ceiling is defined as per-person but every example shows it varying by topic area — definition gap

**Location:** [01-axes.md](01-axes.md#L40-L60), Delegation Ceiling section

The **Delegation Ceiling** is the highest level of AI involvement a person can accept for their work without feeling threatened. At level D1, the person does the work themselves and AI has no role. At D4, the person is directing AI work rather than doing it.

The opening text says: "A property of the person, not of the interaction." That means one number for the whole person.

But then the example says: "A person in S3B Bargaining can have a D3 ceiling for low-stakes domains while maintaining D1 for their core craft."

That sentence shows the ceiling varying by domain (topic area). That's not one number per person — it's a different number per area of work.

The word "core" narrows it slightly ("core domain" suggests one special area), but "core" is never defined. Can someone have multiple core domains? If so, the ceiling is definitely per-domain.

Practitioners don't know whether to ask "What is this person's ceiling?" (one answer) or "What is this person's ceiling for their primary domain?" (potentially many answers).

**Fix:**

Decide whether Delegation Ceiling is per-person or per-domain.

If per-person (one number): revise the examples to be consistent with that, and explain how one ceiling applies across all areas of work.

If per-domain (one number per topic area): change the intro to say "A property of the person in a specific domain, not of the interaction." This is the recommended option — it makes Delegation Ceiling structurally parallel to Identity Stakes and matches how the examples actually read.

---

### 3. Two files describe the same observation and attach opposite confidence labels — epistemic inconsistency

**Location:** [S3B-bargaining.md](states/S3B-bargaining.md#L70-L78) vs [S7M-maturity.md](states/S7M-maturity.md#L38-L40)

Both files describe the same distinguishing behavior: when a new AI model releases, does the person immediately move their personal boundary about what AI is allowed to do (that's S3B Bargaining), or do they test the new model before changing anything (that's S7M Maturity)?

The **S3B file** calls this **Conjecture** — a hypothesis that requires longitudinal data to confirm, and that is also vulnerable to self-report bias once someone has read the model. ("Self-report bias" here: once people know how S3B and S7M are supposed to differ, they may describe their own behavior in whichever way they think is expected of them.)

The **S7M file** calls the same observable behavior **Testable** — something that can be verified by watching what people do across multiple model releases.

Same observation, opposite labels. A practitioner reading S3B comes away thinking "this is a shaky hypothesis." The same practitioner reading S7M thinks "this is a claim we can verify." They should come away with the same impression, because both files are talking about the same thing.

**Fix:**

Use **Testable** in both files — watching how people respond across model releases is a concrete observation. Add the self-report caveat to the S7M file as well, since it applies there just as much.

---

### 4. Dropout severity axes have no scoring anchors — operationalization gap

**Location:** [dropout.md](dropout.md)

The model rates dropout severity on two independent 0–10 axes:

- **Practical severity:** tool failures, bad outputs, workflow friction, cost.
- **Emotional severity:** identity threat, ego shock, fear, exhaustion.

The text describes what the four quadrant combinations mean (high practical / low emotional = the tool genuinely didn't work; low practical / high emotional = identity threat or exhaustion; and so on). That qualitative description is clear.

But there are no definitions for what each number on the scale actually means. Is "the tool is slow" a 3 or a 6 on the practical axis? Is "I'm not confident I can do this without AI anymore" a 4 or a 7 on the emotional axis? Two practitioners rating the same person would likely disagree — and not by a small amount.

The model acknowledges this: "**Conjecture** — inter-rater reliability (whether two independent raters would agree on scores) of the 0–10 axes has not been established."

The reversibility test (offer a better tool and see if the person restarts) is concrete and useful, but it only distinguishes high-practical / low-emotional dropout from everything else. It doesn't define the axes.

The model presents the axes as something practitioners can **measure**. In their current form, they can't. Practitioners will score the same case differently.

**Fix:**

One of three options:

1. **Add scoring anchors.** Define what 0–3, 4–6, and 7–10 mean on each axis with behavioral examples. For practical severity: 0–3 = "tool meets my needs with minor friction"; 4–6 = "significant gaps but core tasks still work"; 7–10 = "tool fails critical tasks or is unusable." Same level of detail for emotional severity.

2. **Drop the numbers, use four labeled quadrants.** Change "two 0–10 scales" to "four quadrant regions" (high/low on each axis). Less precise but honest about what you can actually measure.

3. **Make the reversibility test the primary measure.** Run the test first, then use the quadrant labels as a post-hoc frame once the test result is known.

Recommendation: Option 1. Add concrete anchors. Without them, the framework is not executable.

---

### 5. The state diagram only shows S0 leading to S1 — the permanent non-user path is missing

**Location:** [02-state-graph.md](02-state-graph.md#L23-L50), main diagram

The Mermaid diagram (a text-based format for flowcharts) shows:

```
S0 --> S1 : exposure
```

That's it for S0. The diagram shows S0 (Baseline) as a starting point that leads to S1 (first exposure to AI).

But the text immediately below says S0 has two readings: a transitional state (before first exposure) and a **terminal state** — meaning someone who is aware of AI and has decided not to use it, with no expectation of change. Terminal means it can be a permanent end state, not just a stepping stone.

A practitioner reading the diagram without the text would assume S0 always leads to S1. That contradicts the model's explicit claim.

**Fix:**

Add the terminal path to the diagram. For example:

```
S0 --> S1 : exposure
S0 --> S0 : (terminal — permanent non-user)
```

Or add a node annotation: `S0: Baseline (transitional or terminal)`.

Also make sure the diagram caption explicitly names both readings.

---

### 6. The three modulating properties operate at different levels — structural coherence gap

**Location:** [01-axes.md](01-axes.md), overall structure

The model has three properties that together describe how a person approaches AI delegation:

1. **Identity Stakes** — how much a person's professional identity is tied to a given topic area. Per-domain.
2. **Task Delegation Level (D1–D4)** — how much of the actual work the person hands to AI for a specific task. Per-interaction.
3. **Delegation Ceiling** — the highest delegation level a person can accept. Described as per-person, but examples show it as per-domain (see Finding 2).

These sit at different levels. If Delegation Ceiling is per-person, you're combining:
- A per-domain property (Identity Stakes)
- A per-interaction property (Task Delegation Level)
- A per-person property (Delegation Ceiling)

That mismatch makes the three properties harder to use together consistently. A practitioner asking "how do these three interact?" can't answer cleanly when they operate at different scopes.

If Delegation Ceiling is per-domain, the structure becomes coherent: pick a domain (which fixes Identity Stakes and Delegation Ceiling for that domain), then within that domain, choose a Delegation Level for each individual task.

**Fix:**

Confirm Delegation Ceiling is per-domain, and restructure the axes section to group the properties explicitly:

- **Per-domain:** Identity Stakes, Delegation Ceiling
- **Per-interaction:** Task Delegation Level

---

### 7. S7V can be reached four different ways but the model doesn't predict stability — predictive gap

**Location:** [S7V-evangelism.md](states/S7V-evangelism.md#L17-L30)

**S7V** is the stable evangelism state — people who have worked through their own identity questions about AI and are now helping others through theirs.

V5 strongly implied that S7V came mainly from S3E Ego Shock (the state of identity disruption — when AI being competent at your job makes you feel threatened or obsolete). The logic: you can't credibly guide someone through that disruption if you've never had it.

V6 weakens this to: stable S7V is more common in people with prior S3E experience, but four paths can lead to S7V:

1. Through S3E Ego Shock (lived experience of identity disruption)
2. Through S7I Identity Expansion (built a new, expanded sense of professional identity)
3. Through professional role (educator, consultant, team lead — the job itself makes you a guide)
4. Through generativity drive (some people are just oriented toward helping others develop)

The problem: the model gives no heuristics for inferring which path someone took. And stability depends on path. The model warns that S7V with only "S6E flavor" — someone who became enthusiastic about AI without real depth of experience — tends to collapse under hostile questioning or when their team stops rewarding advocacy. But it defines "depth" only as "can speak from examples of failure as well as success," without saying how many failures or what counts as enough.

A practitioner working with someone in S7V can't tell whether that person is stable or at risk of collapse.

**Fix:**

One or more of:

1. **Define depth operationally.** For example: "can describe at least one specific failure in their domain and what they actually changed as a result; can explain at least one concrete limitation of AI in their work; has at least six months of sustained use."

2. **Add path inference heuristics.** For example: "S7V reached through S3E often shows an initial resistance phase in their history before advocacy; S7V through professional role often shows a consistent stance from the start, without an early resistance phase."

3. **Downgrade the stability claim.** If the four paths are truly parallel and depth is genuinely hard to measure, state clearly that some people in S7V are at risk of collapse, and practitioners should probe for depth before relying on them as guides.

---

### 8. The S6 observation guide is built for clean cases — most cases aren't clean

**Location:** [observation-guide.md](observation-guide.md#L1-L90)

The guide provides concrete interview probes for each of the four S6 overuse states:

- **S6E (Enthusiastic Overuse):** "When was the last time AI surprised you in a bad way?" — An S6E person has no answer, or immediately pivots back to positive examples.
- **S6D (Dependent Overuse):** "If AI were unavailable for a week, what would you do?" — An S6D person expresses disproportionate anxiety.
- **S6R (Driven Overuse):** "If performance metrics stopped tracking AI use tomorrow, how would your usage change?" — An S6R person admits usage would drop.
- **S6S (Social Overuse):** "What would you do with AI if you were working entirely alone, with no one watching?" — An S6S person gives an answer that differs from their observed behavior.

These probes are good and concrete.

But then the guide concludes: "Most real cases are mixed."

And provides no guidance on:
- How to classify someone showing signals of both S6E and S6D (enthusiastic about new features, anxious about high-stakes decisions)?
- How to weight conflicting signals?
- Which intervention to route them into when the model assumes one primary S6 state per person?

The state coexistence rules say S6E and S6D are mutually exclusive (the emotional signatures are opposite). But a person who is "excited about AI generally, worried about relying on it for anything that really matters" looks like mixed S6E + S6D. How do you classify them?

**Fix:**

Add a "Handling mixed S6 cases" section to the observation guide. It should include:

1. **Common mixed patterns:**
   - S6E + S6D: enthusiastic about low-stakes tasks, anxious about high-stakes ones
   - S6R + S6E: driven by metrics, also energized by demos and showing others
   - S6S + S6D: conforming to team adoption while privately doubting their own capability

2. **A method for picking the primary state:**
   - What is the person's overall affect when not focused on a specific incident? (S6E = energized; S6D = anxious; S6R = stressed; S6S = compliant)
   - Which signal is most consistent across weeks?

3. **Intervention routing for the common mixed patterns:**
   - Mixed S6E + S6D: address S6D first (rebuild independent judgment), then let the S6E enthusiasm settle naturally.
   - Mixed S6R + S6S: identify which driver is primary — productivity pressure or peer pressure — and address that context first.

---

### 9. Related-literature anchors are internally consistent but not validated — worth flagging for practitioners

**Location:** Scattered across state files

Each state in the model lists related constructs from existing psychology research. This review checked whether those constructs match the state's described transition behavior.

They do. No contradictions found. For example:

- S3E (Ego Shock) anchored to "self-efficacy collapse" (the feeling of *I'm not good at my job anymore*) and "terror management" (psychological defenses against threats to one's sense of purpose). Both are plausible for the identity disruption that characterizes S3E. The transitions out — to S3B Bargaining, S5 Understanding, or S3X Exit — all make sense under those constructs.
- S6E (Enthusiastic Overuse) anchored to "variable-reward reinforcement" (AI sometimes gives great results, sometimes doesn't — the same pattern that makes slot machines compelling). The transitions out to S7M Maturity, or back to S3E when the enthusiasm hits a wall, are plausible consequences of that dynamic.

The caveat: the model borrowed these constructs as labels, not as explanations. The related-literature lines say "this state resembles what psychology research calls X" — they don't say "X is why the transitions happen." And the model doesn't validate that real-world behavior under these constructs actually matches the predicted transitions. The model itself is honest about this.

**No fix needed.** But practitioners who read the literature anchors and expect them to predict behavior should be warned that the connection is plausible, not tested.

---

### 10. S2T and S2D have no fixed order, but their transitions are one-way — clarification needed

**Location:** [02-state-graph.md](02-state-graph.md#L6-L13), S1 fork section

**S2T (Trust Evaluation)** = the person is willing to test AI on its merits. Epistemically open (willing to update based on what they observe).

**S2D (Defensive Resistance)** = the person evaluates AI through the lens of protecting their professional identity. Epistemically closed — they focus on failures and minimize successes because accepting that AI is capable feels like a threat.

V6 correctly says these two states have no implied order — you can go directly from S1 (first exposure) to either one. Identity Stakes (how much someone's professional identity is tied to the domain) tends to predict which way you go, but it's not a fixed rule.

The slight confusion: S2T can shift to S2D during testing, if the testing surfaces a real identity threat. But S2D cannot shift to S2T — once in the defensive posture, you don't just become open again without some kind of regression event first.

The phrase "no implied order" might be read as "no tendency either way" — which is wrong. High Identity Stakes does tend toward S2D, it's just not guaranteed.

**Fix:**

Revise the note in [02-state-graph.md](02-state-graph.md) to separate two distinct points:

- **No prerequisite:** you don't need to pass through S2T to reach S2D, or the reverse.
- **Asymmetric transitions:** S2T can shift to S2D when testing reveals a threat; S2D cannot shift to S2T without a regression event first. This isn't arbitrary — it reflects how identity-protective thinking works.

Suggested wording: "The fork after S1 (S2T versus S2D) is driven by Identity Stakes as a tendency, not a rule. Neither state is a prerequisite for the other; either can be entered directly from S1. The transitions between them are asymmetric: S2T → S2D can happen when testing surfaces a threat; S2D → S2T does not happen without a regression event, because defensive posture does not revert to open evaluation on its own."

---

## RECOMMENDATIONS

### Priority 1: Fix logical contradictions

1. **S6R + S6S coexistence (Finding 1).** Resolve the contradiction. Either remove the "can coexist" bullet, or reframe it: "can coexist briefly but is unstable — collapses without ongoing external pressure."

2. **Dropout severity scoring (Finding 4).** Add behavioral anchors to both 0–10 axes. Without them, two practitioners rating the same case will score it differently and the framework isn't usable.

3. **S0 terminal path in diagram (Finding 5).** Add the S0 → (terminal) path to the Mermaid diagram so the visualization matches the text.

### Priority 2: Clarify ambiguous definitions

4. **Delegation Ceiling scope (Findings 2 and 6).** Confirm it is per-domain, revise the intro sentence to say so, and restructure the axes section to group per-domain and per-interaction properties separately.

5. **S3B vs S7M epistemic label (Finding 3).** Use **Testable** in both files, with a note in S3B that the signal requires longitudinal data and is vulnerable to self-report once someone has read the model.

6. **S7V depth criteria (Finding 7).** Define "sufficient depth" with concrete behavioral markers.

### Priority 3: Improve applicability

7. **S6 mixed-case guidance (Finding 8).** Add a "Handling mixed S6 cases" section to the observation guide.

8. **S2T/S2D asymmetry (Finding 10).** State explicitly in the state-graph file that the transition is asymmetric: S2T → S2D is possible; S2D → S2T requires a regression event.

### Priority 4: No immediate fix

9. **Related-literature causality gap (Finding 9).** Add a short note for practitioners: the literature anchors are labels, not validated mechanisms. The model is already honest about this — it just needs to be said somewhere practitioners will see it.
