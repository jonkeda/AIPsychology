This is a simpler rewrite of [009-longitudinal.md](009-longitudinal.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Longitudinal Data Gaps — Plain-Language Version

## TL;DR

- V6 deliberately avoids putting numbers on how long people stay in each state or how often they move between states. That choice is honest — the numbers don't exist yet. But it leaves anyone trying to use the model without answers to the most practical timing questions.
- The most important unanswered question: how long does someone typically stay in **S3E Ego Shock** (the state where they realize AI can replicate the skill their job is built on)? Without that number, you can't decide whether to wait, intervene, or refer someone for help.
- Five specific numbers would change how the model gets used: how long people stay in S3E; how often people in S5 Understanding slide back after a capability jump; how many S2T Trust Evaluation testers end up at S5 versus S2D Defensive Resistance; how long until S6E/S6R overuse leads to burnout; and whether S3X Structural Displacement conclusions hold over years. All five can be measured with a study that follows the same people over time.
- A minimum study to get these numbers would take 18–24 months, span two major model releases, follow roughly 150 knowledge workers with quarterly check-ins, and cost roughly $80–120k. That is the first practical step toward a version of the model with real numbers in it.

---

## Findings

### 1. V6 has no dwell-time estimates, making intervention timing impossible — not yet tested

**Dwell time** (how long someone stays in a given state before moving on) is absent from V6 by design. The model's own documentation lists "numerical transition probabilities and dwell times" — that is, the chances of moving between states and how long each stay lasts — under "Deliberately not in V6." The stated reason: adding made-up numbers is worse than admitting the numbers don't exist yet.

That is the right call. But it creates a real problem for anyone trying to use the model in practice.

When a practitioner — a coach, manager, or HR person — sees someone stuck in **S3E Ego Shock** (the state where a person is confronting the fact that AI can replicate the skill their professional identity is built on), the model says:

- S3E is meant to be temporary. Healthy as a passage; harmful as a long stay. Sustained S3E without movement within weeks to months warrants attention.

"Weeks to months" is not a number. A manager watching an employee in S3E cannot answer: do I give them two weeks? Two months? Is this the start of a six-month crisis? The model describes what happens *after* the person exits S3E — moving toward S3B Bargaining or S5 Understanding. It does not say *when* that exit happens.

The same gap shows up with regressions. Any state from S5 onward can get pushed back to S3E by changes in the AI environment. Without regression rate data, a practitioner cannot estimate: of my team currently at S5 Understanding (the stable, comfortable state with AI), what fraction will fall back to S3E after the next capability jump?

**Fix:** Commission an 18-month study that follows the same people over time, spanning two model releases, to establish how long people typically stay in S3E, S5, and S6 states. Report medians, quartiles (the spread of the distribution), and what goes wrong when a normal exit doesn't happen. See Recommendation 1.

---

### 2. S3E dwell time is the load-bearing question — testable

Among the five priority timing questions, how long people stay in S3E comes first. It is the most decision-critical and the highest-leverage number to have.

S3E is also the state most tied to a person's sense of professional identity. Someone still stuck there after month three is at risk of clinical distress (needing professional mental health support). Someone still there at month six is likely in crisis. A practitioner needs:

- Median dwell time — for example, "most people take 4–8 weeks to reach S3B Bargaining or S5 Understanding."
- The probability of not exiting normally — for example, "15% of people in S3E for more than 6 weeks drop out emotionally rather than moving forward."
- Whether **Identity Stakes** (how much your professional identity depends on the skill being replaced) affects timing. High-stakes domains likely mean longer stays; low-stakes domains faster exits.
- What triggers an extended stay: repeated capability jumps? Loss of the boundaries around their domain? Watching a junior colleague outperform them with AI?

The model's observation guide already tells practitioners to watch for whether someone is "moving through S3E within weeks to months or staying unresolved after six or more months." That heuristic is reasonable. But it is based on qualitative observation, not data. A study can replace the vague range with a real distribution.

**Fix:** Make S3E dwell time the primary outcome of the first study. Oversample high-stakes domains (engineering, law, translation, creative writing) where the model predicts longer stays. Report medians broken down by domain.

---

### 3. S5 "stability" cannot be claimed without regression rates — testable

V6 describes **S5 Understanding** as "the first stable state" and marks it sustainable. But "stable" without data is an assumption, not a finding.

Whether S5 is actually stable depends on what happens when the AI environment changes. The state graph shows explicitly that any state from S5 through S7 can be pushed back to earlier states by changes in the AI environment. The triggers include capability jumps, access changes, tooling shifts, workplace changes, and personal events. Capability jumps are the most common.

Without data, V6 cannot answer:

- What fraction of people in S5 fall back to S3E when a new capability lands in their domain?
- How long does that regression last? Do they come back to S5, or drop out?
- Is S5 genuinely stable, or is it "stable until the next shock"?

Anyone redesigning a support program needs to know whether S5 is an end state or a platform that needs re-stabilizing every 6–12 months — roughly every major model release.

**Fix:** Embed regression rate measurement in the second-year analysis of the longitudinal study. Track groups across at least two major AI capability releases. Report what fraction regress, how long the regression lasts, and what fraction return to S5.

---

### 4. The S2T Trust Evaluation fork outcome ratios are unmeasured — testable

After a person's first encounter with AI, the model sends them down one of two paths:

- **S2T Trust Evaluation** — low-stakes testing, no particular threat to identity.
- **S2D Defensive Resistance** — high-stakes reaction, protective stance.

S2T can tip into S2D mid-testing if the person stumbles on a capability that unexpectedly threatens them. But V6 has no data on:

- What fraction of S2T testers actually reach S5 Understanding?
- What fraction tip into S2D partway through testing?
- What fraction quit for practical reasons — the tool doesn't meet their quality or reliability bar?
- How long does the S2T testing period typically last?

These numbers matter for triage and timing. If 80% of S2T testers reach S5, the evaluation period is healthy and you can afford to be patient with them. If 40% tip into S2D and only 30% reach S5, S2T is riskier than the model implies and needs earlier intervention.

**Fix:** Add S2T outcome tracking to the longitudinal study. Follow people for 8–12 weeks from their first AI exposure and classify where they end up: S5, S2D, or one of two dropout types (practical or emotional). Report proportions broken down by Identity Stakes.

---

### 5. S6E and S6R have no burnout timeline — testable

V6 describes **S6E Enthusiastic Overuse** as excitement-driven experimentation — the person is energized, productive, and uncritical about AI. It calls this "healthy short-term, costly long-term" but does not specify how short or how long.

**S6R Driven Overuse** is pressure-driven — pushed by productivity demands rather than enthusiasm. The model says it is sustainable "only as long as external pressure does not exceed personal capacity. Past that point, S7B Burnout follows." But it does not say when that point arrives.

Without time-to-burnout data, neither the person nor the practitioner knows what "short-term" and "only as long as" actually mean. Is S6E sustainable for four weeks? Four months? Four years?

The model's own documentation says: "The duration of healthy S6E before it becomes corrosive is qualitatively understood (weeks to months) but not numerically established." That is exactly the gap the next version of the model needs to close.

Burnout is measurable: usage collapses, the person withdraws, their attitude turns cynical or depleted. Time-to-burnout is the critical number for:

- Estimating how many people are currently at risk at any given moment.
- Designing intervention windows — for example, "check in with high-volume users monthly to catch early burnout signals."
- Giving people honest guidance about whether their current pace is sustainable.

**Fix:** Establish time-to-burnout distributions from S6E and S6R by tracking monthly usage volume and mood measures for people in those states. Report median time to exit (whether that is S7B Burnout or a slide back to S5), what goes wrong when normal exit doesn't happen, and how Identity Stakes and **Delegation Level** (how much of the work you hand off to AI) correlate with the timeline.

---

### 6. S3X Structural Displacement stability is unmeasured — testable

V6 introduces **S3X Structural Displacement** as its own distinct state — reached when "viable AI-collaborative work no longer exists in their domain." In plain terms: the person concludes, or is forced to accept, that their economic position is gone.

But the model does not specify:

- How long do people stay in S3X before reaching one of three outcomes: moving to a different field, leaving knowledge work entirely, or becoming actively hostile toward AI?
- How firm is the S3X conclusion? Do people re-enter S3B Bargaining (making new deals with themselves about AI) after months in S3X, having found new niches?
- What fraction reach each of the three outcomes?
- How long does switching fields actually take?

These gaps matter because they determine whether S3X is a brief phase or a long-term condition. If most people in S3X transition within 6 months, it is a short passage. If they stay for two or more years, it warrants its own support structure.

The model itself acknowledges: the three-resolution structure (switch fields, exit knowledge work, fight AI) covers observed responses but has not been checked against a representative sample of displaced workers.

**Fix:** Recruit a group of 40–60 people who are clearly in S3X — their role has been eliminated, clients have stopped paying for their human work, or they have concluded they can no longer compete. Follow them for 18–24 months. Track which resolution they pursue, how long it takes, whether any return to earlier states, and what happens economically. Break down results by domain, age, and access to reskilling resources.

---

### 7. Regression triggers and rates lack temporal specificity — testable

V6 lists what can trigger a regression — capability changes, access changes, tooling shifts, workplace changes, personal events — but provides no rate data. For example:

- "A junior colleague outperforming with AI re-triggers S3E from later states."

Does a single observation trigger that? A sustained performance gap over weeks? Only when the person's manager also notices? And what fraction of people actually regress versus explain it away?

Similarly, "a model release that overruns prior rebuttals" is listed as a capability trigger, but V6 does not specify:

- Which types of capability jump trigger regression? A new modality in a domain the person thought was safe, or just incremental improvement in the same area?
- Are there threshold effects — regression only happens if the new capability exceeds what the person had in their head by some meaningful margin?
- What is the baseline regression rate for a typical capability jump — for example, "20% of S5 people regress on a major capability jump, 5% drop out, 75% stay"?

Without these numbers, practitioners cannot predict the impact of a model release or major feature launch on their user population.

**Fix:** Set up the longitudinal study to log all trigger events — capability jumps, team changes, performance reviews, peer comparisons — with enough detail to classify them. Use model version tracking and release notes to gauge how large each capability jump was. Report regression rates per trigger type with confidence intervals.

---

### 8. The "most people cycle through the model more than once" claim is still unquantified — testable

V6 carries forward from V5 the claim: "People cycle through the model more than once because the AI environment keeps changing, not because the person is unstable."

This is flagged as a **conjecture** (an educated guess, not a finding) in the model's own limits documentation: "V6 makes no numerical claim about cycle frequency."

But practitioners and researchers need actual numbers:

- What is the average number of cycles per person over a 24-month window?
- Do people in more volatile domains cycle more often?
- Are some people chronic cyclers — more than three cycles per year — and if so, what predicts that?
- Does cycling increase burnout risk, or is it unrelated?

The model assumes cycling is normal and expected, not a sign of instability. Measuring cycle frequency is how you test that assumption.

**Fix:** Compute cycle frequency for all study participants. Define a cycle boundary using state-transition events (entering a new major state, regressing, or exiting the model entirely). Report mean, median, and distribution of cycles per person per year, broken down by domain and Identity Stakes.

---

## Minimum Viable Study: Establishing V7 Dynamics

### Scope

Measure how long people stay in S3E, S5, S6E/S6R, and S3X, and how often they move between states, across an 18–24-month window spanning two major model releases.

### Design

**Who to follow:** 150 knowledge workers, starting either from their first AI exposure or from wherever they currently sit in the model.

Break the group into:

- **High-stakes domains:** 80 people — software engineering, medicine, law, creative writing, research, translation.
- **Low-stakes domains:** 70 people — business analysis, financial forecasting, customer support, administrative work.

Include a mix of seniority (individual contributor, manager, senior) and how long they have been meaningfully exposed to AI in their domain (0–3 years).

**What to track:**

- **Quarterly surveys:** which state they're in (self-reported plus behavioral markers from the observation guide), usage volume, whether their current pace feels sustainable, intention to keep using AI, and any major work changes.
- **Event logging:** capture all capability jumps (model releases, new features in their domain), workplace changes (team reorganization, new manager, new performance metrics), and personal events (performance feedback, peer comparisons, burnout signals).
- **Usage data (optional):** if participants consent and the tools allow it — such as ChatGPT, Copilot, or Claude — log monthly Delegation Level and frequency.

**Duration:** 18–24 months minimum. Must span at least two major model releases.

### Measurement Tools

- **State classification:** trained reviewers apply the observation guide markers each quarter. Target inter-rater agreement above 0.75 (Cohen's kappa — a standard score for how consistently two independent reviewers classify the same person the same way).
- **Dwell time:** for each state transition, measure time from entry to exit.
- **Regression tracking:** flag all transitions to earlier states and record the trigger event if identifiable.
- **Dropout scoring:** at exit, score on two axes (practical: 0–10; emotional: 0–10) following the dropout documentation.

### Primary Outcomes

- Median dwell times, with IQR (the spread from the 25th to 75th percentile), for S3E, S5, S6E, S6R, and S3X, broken down by Identity Stakes.
- Transition rates: S2T → S5, S2T → S2D, S2T → dropout; S5 regression rates on a capability jump; S6E/S6R → S7B Burnout; S3E → S3B Bargaining versus S3E → S5.
