# Method 4: Manager Observation Framework — Detailed Plan

## Objective

Test whether managers can reliably identify the AI Psychological Adaptation Cycle stages in their direct reports, and in a second phase, test whether stage-aware management interventions improve adoption outcomes compared to generic approaches.

---

## Phase 1: Can Managers See the Stages?

### Preparation

**Manager cohort selection**

Recruit 10–15 managers who:
- Have at least 4 direct reports each
- Span different departments (technical, creative, operational)
- Are willing to participate for 3 months
- Have their own varying levels of AI adoption (mix of enthusiasts and sceptics — don't select only pro-AI managers)

Total observed population: 40–75 individuals across all managers.

---

### Manager Training

A single 90-minute session covering:

**Part 1 (30 min): The model**

Walk through the stages using the short descriptions. For each stage, provide:
- What it sounds like (quotes)
- What it looks like (observable behaviours)
- What it does NOT look like (common misidentifications)

**Observable behaviour guide:**

**Stage 0: Pre-Exposure**
- Sounds like: No mentions of AI. Doesn't attend AI-related meetings or training.
- Looks like: Genuine unawareness, not active avoidance.
- Not: Someone who knows about AI but hasn't tried it (that's Stage 1).

**Stage 1: Dismissal**
- Sounds like: "It's a fad." "We tried chatbots five years ago." "It's not relevant to what we do."
- Looks like: Eye-rolling in meetings. Declining to try tools. Changing the subject.
- Not: Someone who tried AI and found it lacking (that might be practical dropout or Stage 2).

**Stage 2: Defensive Resistance**
- Sounds like: "I tried it. It got this wrong." "It's not creative." "It's just autocomplete."
- Looks like: Sharing AI failures with colleagues. Testing AI on deliberately hard problems to prove it fails. Spending more energy criticising than exploring.
- Not: Legitimate quality feedback (Stage 4 — Trust Evaluation). The difference is emotional tone: Stage 2 is triumphant when AI fails; Stage 4 is neutral.

**Stage 3: Ego Shock**
- Sounds like: Quiet withdrawal. "I don't know." Uncharacteristic self-doubt. Reduced confidence in meetings.
- Looks like: Mood change after an impressive AI demo. Avoiding discussions about AI capabilities. Asking questions about job security or future relevance — or conspicuously not asking.
- Not: General low mood unrelated to AI. Managers should not diagnose personal mental health.
- **Important:** This stage is the hardest to observe and the most sensitive. Managers should never label someone as being in "ego shock" to their face.

**Stage 3B: Bargaining**
- Sounds like: "I use it for X but I always do Y myself." "It's fine for rough drafts." "The real thinking is still mine."
- Looks like: Consistent AI use with rigid, self-imposed boundaries. Clear rules about which tasks get AI and which don't. Defending those boundaries if challenged.
- Not: Thoughtful, evidence-based task allocation (that's Stage 5 or 7A). The difference is rigidity — bargaining boundaries are identity-protective, not pragmatic.

**Stage 4: Trust Evaluation**
- Sounds like: "I've been testing it on problems where I know the answer." "It's reliable for X but not for Y."
- Looks like: Systematic experimentation. Comparing AI output to own output. Documenting strengths and weaknesses. Calm, analytical tone.
- Not: Stage 2 (which looks similar but has an adversarial emotional tone).

**Stage 5: Understanding**
- Sounds like: "It's a good tool for this kind of thing." "I know when to use it."
- Looks like: Natural, unselfconscious AI use. Not evangelical, not defensive. AI is part of the workflow without fanfare.
- Not: Overcompensation (Stage 6), which looks similar but with higher intensity and broader scope.

**Stage 6: Overcompensation**
- Sounds like: "Have you tried using AI for this?" (about everything). "I automated my whole morning." "Why would anyone do this manually?"
- Looks like: AI use expanding rapidly into new domains. Declining to do tasks manually. Evangelising unprompted. Staying late to experiment.
- Not: Healthy enthusiasm (Stage 5 with energy). The difference is scope creep and potential quality decline from over-delegation.

**Stage 7 (various):**
- **7A Maturity:** Calm, balanced, selective use. Not exciting to observe — looks like "normal."
- **7B Identity Expansion:** Person describes their work differently. New capabilities they didn't have before. AI is part of their professional identity.
- **7D Burnout:** Reduced AI use after a period of heavy use. Fatigue. "I need a break from this."
- **7F Evangelism:** Actively teaching others. Running informal sessions. Writing guides. Mentoring.

**Part 2 (30 min): How to log observations**

Introduce the observation log (below). Practice coding 3–4 written scenarios as a group to calibrate. Discuss edge cases.

**Part 3 (30 min): Boundaries and ethics**

- Never label someone to their face ("You're in ego shock")
- Never use stage identification in performance reviews
- Never pressure someone to move stages faster
- Report patterns, not individuals, in the final analysis
- If someone appears to be in genuine distress (Stage 3), refer to appropriate support — don't try to manage it as a "stage"
- All logs are confidential and used only for research purposes

---

### Observation Log

Each manager keeps a log with one entry per direct report per fortnight (every 2 weeks). Total: 6 entries per person over 3 months.

**Log format:**

```
Date: _______________
Person ID: ___________ (anonymised — use consistent codes, not names)
Role type: Technical / Creative / Operational / Leadership

Observed stage: [select one: 0 / 1 / 2 / 3 / 3B / 4 / 5 / 6 / 7A / 7B / 7C / 7D / 7F / Unsure]

Confidence: Low / Medium / High

Evidence (1–3 bullet points — what did you see or hear?):
- 
- 
- 

Change since last entry: No change / Moved forward / Moved backward / Unsure

If changed — what triggered it? (optional):

Notes (optional):
```

**Log delivery:** Managers submit logs fortnightly via a shared form or spreadsheet. Keep it lightweight — 5 minutes per person per fortnight.

---

### Cross-Validation

At the end of the 3-month observation period:

**1. Manager vs. self-report comparison**

Run the Method 1 survey (Internal Survey) with the observed population. Compare each person's self-identified stage with their manager's most recent stage assessment.

Measure: **Agreement rate.** What percentage of manager assessments match self-reports?

Expected outcomes:
- High agreement (>60%) = stages are observable and recognisable from both sides
- Moderate agreement (40–60%) = stages are partially observable; some are harder to see from outside
- Low agreement (<40%) = the model may describe internal states that aren't externally visible, limiting management utility

**2. Inter-rater reliability (if possible)**

If any individuals are observed by two managers (e.g., matrix reporting, project leads), compare their stage assessments for the same person.

Measure: **Cohen's kappa.** Values above 0.4 indicate fair agreement; above 0.6 indicates good agreement.

**3. Manager vs. usage data (if Method 3 is running)**

Compare manager-observed stages with behavioural patterns from AI tool usage data. Do managers identify overcompensation in people whose usage data shows a spike? Do they identify bargaining in people whose usage is consistent but task-restricted?

---

### Phase 1 Analysis

**Stage observability ranking**

Which stages can managers reliably identify? Rank stages by agreement rate with self-reports. Expected: Stages 1, 2, 6, 7F are most observable (they involve visible behaviour). Stages 3 and 3B are least observable (internal, identity-level experiences).

**Confusion matrix**

Where do managers mis-identify stages? Common expected confusions:
- Stage 2 (Defensive Resistance) confused with Stage 4 (Trust Evaluation) — both involve critical assessment, but the emotional tone differs
- Stage 5 (Understanding) confused with Stage 7A (Maturity) — both look "normal"
- Stage 3B (Bargaining) confused with Stage 5 (Understanding) — both involve selective use, but for different reasons

**Manager self-awareness**

Ask managers to identify their *own* stage at the start and end of the observation period. Did participating in the study change their own position?

---

## Phase 2: Do Stage-Aware Interventions Help?

Run only if Phase 1 shows managers can reliably identify stages (agreement rate >50%).

### Design

Split the manager cohort into two groups:

**Group A — Stage-aware interventions (treatment)**

Managers receive guidance on stage-matched responses:

**For Stage 0 (Pre-Exposure):**
- Low-pressure exposure. Share examples, not mandates.
- Invite to observe, not participate.

**For Stage 1 (Dismissal):**
- Don't argue. Don't mandate.
- Provide a compelling, relevant demo — ideally from a peer, not a vendor.
- Let curiosity develop naturally.

**For Stage 2 (Defensive Resistance):**
- Acknowledge the flaws they've found — they're often real.
- Don't dismiss their concerns as irrational.
- Avoid framing AI as inevitable or unstoppable — that amplifies the threat.
- Ask: "What would it need to do well for you to find it useful?"

**For Stage 3 (Ego Shock):**
- Do not pressure. Do not performance-manage.
- Normalise the feeling: "A lot of people feel this way."
- Reinforce the person's unique value — judgement, relationships, context, creativity.
- If distress is significant, refer to appropriate support.
- Give time. This stage passes, but not on demand.

**For Stage 3B (Bargaining):**
- Respect the boundaries. Don't push people to use AI for tasks they've reserved for themselves.
- Acknowledge that partial adoption is productive.
- Let the boundaries shift naturally as confidence grows.

**For Stage 4 (Trust Evaluation):**
- Support the testing. Provide good use cases and realistic expectations.
- Share known limitations honestly — don't oversell.
- Let them reach their own conclusions.

**For Stage 5 (Understanding):**
- Minimal intervention needed.
- Support social normalisation — make AI use visible and unremarkable within the team.

**For Stage 6 (Overcompensation):**
- Gently check quality. Are they over-delegating?
- Ask: "Is AI the right tool for this specific task?"
- Don't shame the enthusiasm — redirect it.

**For Stage 7D (Burnout):**
- Reduce pressure to use AI.
- Acknowledge the exhaustion.
- Let them set their own pace for re-engagement.

**For Stage 7F (Evangelism):**
- Channel it. Give them a role — peer mentor, training support, community of practice lead.
- Their credibility with resisters is higher than any formal programme.

**Group B — Standard approach (control)**

Managers continue with whatever AI adoption approach the organisation is already using (training, mandates, encouragement — whatever is status quo). No stage-awareness training beyond Phase 1 participation.

---

### Measurement

Compare Groups A and B after 3–4 months on:

**1. Adoption progress**

For each observed individual, measure stage movement:
- How many stages did they advance? (Using fortnightly logs)
- Did they reach Stage 5+ (Understanding or beyond)?
- Did they regress?

Compare average stage advancement between Group A and Group B.

**2. Dropout rate**

How many people stopped using AI during the period? Split by emotional vs. practical dropout.

Compare dropout rates between groups.

**3. Team sentiment**

Brief pulse survey at end of Phase 2:
- "I feel supported in how I'm learning to use AI" (1–5)
- "I feel pressured to use AI more than I'm comfortable with" (1–5)
- "My manager understands how I feel about AI tools" (1–5)

Compare scores between groups.

**4. Quality of AI-assisted work (if measurable)**

If work outputs can be evaluated (e.g., code quality, document quality, decision quality), compare quality trends between groups. This is the hardest metric but the most valuable.

---

### Phase 2 Analysis

**Primary question:** Do people with stage-aware managers advance through the cycle faster, with less dropout and higher satisfaction, than people with standard management?

**Secondary questions:**
- Which stages benefit most from stage-aware intervention?
- Does stage-aware management reduce emotional dropout specifically?
- Does it reduce regression after external triggers?

---

## Timeline

| Period | Activity |
|--------|----------|
| Week 1–2 | Recruit manager cohort; schedule training |
| Week 3 | Deliver training session |
| Week 4–15 | Phase 1: Fortnightly observation logs (3 months) |
| Week 13–14 | Run Method 1 survey with observed population for cross-validation |
| Week 15–17 | Phase 1 analysis; decide whether to proceed to Phase 2 |
| Week 18 | Split cohort into treatment and control; brief Group A on interventions |
| Week 18–33 | Phase 2: Stage-aware interventions vs. control (3–4 months) |
| Week 33–36 | Phase 2 analysis; final report |

**Total: ~9 months** for both phases. Phase 1 alone: ~4 months.

---

## Risks and Mitigations

| Risk | Mitigation |
|------|-----------|
| Managers label people and it leaks into performance management | Explicit ground rules in training. Anonymised logs. Separate from performance processes. |
| Hawthorne effect — people behave differently because they know they're observed | Don't tell the observed population about the study during Phase 1. Inform them retrospectively and offer opt-out from data inclusion. Ethics review required for this approach. |
| Managers project their own biases onto observations | Inter-rater reliability check. Calibration exercises in training. Cross-validation with self-reports and usage data. |
| Stage 3 (Ego Shock) observation could cause harm if handled insensitively | Clear boundaries in training: observe, don't intervene beyond normal management. Refer distress to appropriate support. Never use "ego shock" language with the person. |
| Small sample limits statistical power | Focus on effect sizes and patterns rather than p-values. This is exploratory, not confirmatory. |
| Control group may feel disadvantaged | Offer the stage-awareness training to Group B after Phase 2 completes. Frame it as phased rollout, not exclusion. |
| Managers in Group A may over-intervene | Emphasise that the best intervention for most stages is restraint, not action. "The most useful thing you can do at Stage 3B is nothing." |

---

## Ethical Considerations

- Observing people's psychological states without their knowledge raises consent questions. Consult legal/ethics before proceeding. Options: inform participants generally ("we're studying AI adoption patterns"), or get retrospective consent.
- Stage identification must never be used in hiring, firing, promotion, or performance evaluation decisions.
- Ego shock (Stage 3) may involve genuine distress. Managers are observers, not therapists. Escalation paths to employee support services must be clear.
- All individual-level data should be anonymised in reports. Only aggregate patterns should be shared with leadership.
