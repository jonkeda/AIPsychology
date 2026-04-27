# Longitudinal and Dynamics Review — Model V5

## TL;DR

- V5 deliberately leaves out transition probabilities and dwell times (how long people stay in each state) because guessing numbers is worse than admitting the data don't exist. That choice is correct.
- V6 should add numbers, but only after real data arrives. Until then, V6 should spell out which transitions are candidates for measurement and what evidence would justify numbers.
- Five dynamics questions stand out: how long people stay stuck in defensive resistance or negotiation; what determines whether someone lands in Maturity (S7A Maturity) versus Identity Expansion (S7B Identity Expansion); how often people cycle through the model as AI capabilities grow; what predicts burnout recovery versus permanent dropout; whether the model works the same across software engineering, creative work, and clinical work.
- A 200-person study over 18 months across three professional domains would generate solid transition data for roughly $180k–$280k.
- The most useful measurement is behavioral data: how often people use AI, what new scope they try, when they switch tools. Monthly interviews are secondary.
- V5 wins by admitting uncertainty. The state structure and core mechanisms hold up. What V5 lacks is timing: how fast transitions happen, what variation exists, and which variables push someone toward which exit. A V6 that adds fake numbers will be worse than V5. A V6 that maps out how to get real numbers will be much more useful.

## Findings

1. **The S1 Initial Encounter fork (defensive resistance or acceptance) is well-grounded.** The model claims people with high-stakes professional identities tend toward S2D Defensive Resistance (defensive resistance) when they encounter AI; people with low-stakes use tend toward S2T Trust Evaluation (transfer). This matches research on identity threat: the more your professional identity is tied to your skills, the more threatening an AI tool feels initially. This is the highest-stakes branch to quantify.

2. **The state structure itself holds.** Each state maps to documented psychological mechanisms. S2D Defensive Resistance matches defensive coping. S3 Ego Shock matches identity crisis (the disorientation when core beliefs about yourself are challenged). S5 Understanding matches the resolution phase. The structure is coherent, not arbitrary.

3. **State-entry timing is the missing piece.** V5 does not specify how long a person typically stays in S2D Defensive Resistance before moving to S3 Ego Shock, or whether some stay weeks while others stay months. Same for S3B Bargaining (negotiation): if most people move through it in three months, it is healthy coping. If they stay one or two years, it is a stable defensive position needing different support. A study would answer this.

4. **Dwell times vary widely within states, especially defensive states.** S2D Defensive Resistance and S6D Social Overuse (severe burnout) are emotionally volatile; one person exits quickly while another stalls. S7A Maturity may be stable for years. Without the distribution (median, spread, tail behavior), you cannot predict how long to support someone or when to escalate intervention. This variance is the core dynamics question for organizational teams.

5. **End-state predictors are actionable and testable.** The model claims four types emerge from S5 Understanding: mature integration (S7A Maturity), aggressive scope expansion (S7B Identity Expansion), retreat at lower scope (S7C Ethical Integration), or burnout (S7D Burnout). If you can predict which path based on domain, organizational context, prior experience, and how they handled S3 Ego Shock, you can design conditions favoring S7A Maturity over S7D Burnout. Directly useful for team design.

6. **Regression patterns after model releases are quantifiable but not yet measured.** V5 notes that when new AI models release, people in stable states (S5 Understanding or S7) tend to regress to S3 Ego Shock. This is **testable**: after GPT-5 or Claude 4 releases, measure what fraction of previously stable users shift back to identity questioning, and how long the regression lasts. This requires tracking people before and after a release, not just one survey.

7. **Domain variation is named but not operationalized.** V5 says intensity varies across software engineering, creative work, and clinical work, but does not define what varies. Does a clinical psychologist's S3 Ego Shock unfold faster than a writer's? If you measure 10 software engineers and 10 therapists, both in S3 Ego Shock, do you see the same mechanisms or different substates entirely (a therapy-specific S3 Ego Shock where patient-privacy concerns dominate, versus an engineering-specific S3 Ego Shock where algorithm-correctness concerns dominate)? The study should answer this with 60–70 people per domain.

8. **The practical × emotional severity plane for dropout is measurable but lacks anchors.** Without measurement anchors (such as "practical severity > 7" means the tool failed on more than half the person's tasks; "emotional severity > 7" means the person reports anxiety on exit interview), the plane remains descriptive. The study should operationalize both axes and report how many people fall into each quadrant.

9. **Cycling frequency is unknown but critical for adoption rhythm.** V5 mentions "most people cycle more than once" but does not measure frequency. If the typical person cycles every six months, AI adoption is continuous pressure requiring constant support. If once every three to five years, more episodic. This changes how you pace organizational change and training.

10. **Burnout recovery versus permanent exit is not distinguished.** V5 identifies S7D Burnout (burnout) as a possible outcome but does not quantify what fraction recover (return to S5 Understanding or S7A Maturity) versus drop out permanently. If 80% recover after rest, the model is about temporary overload. If 50% drop out permanently, burnout is terminal and requires prevention-focused design. Operationalizable: ask people who dropped out whether they would resume use if the tool improved or context changed (a reversibility test).

11. **A minimum-viable study is achievable and specific.** The design below (200 participants, three domains, 18 months, behavioral logging plus quarterly interviews) would yield transition probabilities and dwell-time distributions with confidence intervals narrow enough to be useful for V6. The cost is $180k–$280k: substantial but defensible for a model that affects team adoption and individual burnout.

12. **Key study design bets on behavior over self-report.** Track AI usage (how often they launch the tool, what categories, whether they switch tools), ask monthly about scope changes, conduct quarterly interviews about identity and emotional state. Behavioral data is more reliable than asking "What state are you in?" because people lie (to themselves and researchers) about emotional state, but they cannot lie about whether they launched a tool.

## Minimum-viable study design

Three-arm, 18-month panel (tracking the same people over time) with measurement at baseline, every three months, and triggered again after major AI releases.

### Participants

- **Total N = 200**: 70 software engineers, 70 creative writers or content creators, 60 clinical or educational professionals (therapists, educators, medical residents). Spans low-stakes professional use (writing), high-stakes technical work (code review, debugging), and high-stakes relational work (diagnosing, treating).
- **Inclusion**: 18 or older, one or more years of professional experience, English-fluent, at least one month of AI tool exposure before enrollment.
- **Recruitment**: 60% through professional networks, 40% through general labor platforms. Aim for roughly equal gender distribution and age range 20–60.

### Measurement schedule

- **Baseline (week 1)**: demographics, professional experience, prior AI exposure, openness-to-experience, risk appetite.
- **Monthly check-in (5 minutes)**: which state feels like the best fit; AI usage volume (hours per week, categories, tools currently in use).
- **Quarterly deep interview (30–45 minutes at months 1, 4, 7, 10, 13, 16)**: structured interview covering state transitions, emotional experience, scope boundaries, identity reflection. Audio-recorded and transcribed.
- **Event-triggered follow-up**: within two weeks of any major model release, add an extra check-in to capture transition timing.

### What gets measured

1. **Usage telemetry (passive logging)**: weekly tool launches, category mix, tool-switching frequency. High tool-switching plus high scope changes signal S3B Bargaining (negotiation). Stable high volume plus enthusiasm signal S6A Enthusiastic Overuse. Declining volume plus break-needed statements signal S7D Burnout.

2. **Monthly scope statement**: "What tasks do you currently use AI for, and what tasks do you explicitly not use it for?" Coded for whether boundaries are stable or volatile across months. S7A Maturity boundaries shift only on evidence; S3B Bargaining boundaries shift under pressure.

3. **Quarterly interview analysis**: open-ended questions about emotional experience, identity, boundary logic. Coded by two independent raters for: S3 Ego Shock-versus-S5 Understanding signal (identity-threat language versus reframing language); S7A Maturity-versus-S7B Identity Expansion signal (sustainable-stewardship language versus expansion language); emotional severity for dropouts (rated 0–10, aiming for inter-rater reliability above 0.75); domain-specific patterns.

4. **Behavioral log of one focal task per domain**: for example, code review for engineers, first-draft writing for writers, treatment planning for clinicians. Every three months: did AI assistance volume increase, decrease, or stay the same? Did scope change? Did the person's own quality assessment change? More reliable than asking "What state are you in?"

5. **Exit interview for dropout**: when someone stops using the tool, brief interview probing practical severity (did the tool actually fail on reproducible tasks?) and emotional severity (was there threat, identity worry, exhaustion?). Then follow up four weeks later: if you swapped in a high-quality alternative, would you use it? (Yes = practical was the main issue; No = emotional.)

### Retention and incentive

- **Monthly check-in**: expect 95% retention; low friction.
- **Quarterly interview**: expect 85% retention; offer $15 per completed interview ($60 per quarter per person).
- **Attrition management**: pay all participants $10 at month 9 (mid-study) to reduce mid-study dropout.

### Cost estimate

- **Recruitment and screening** (200 participants): $5k–$8k.
- **Participant compensation** (200 × $60 quarterly + $10 mid-study + $200 completion): $56k.
- **Interview transcription and analysis**: $12k–$18k.
- **Behavioral logging infrastructure**: $15k–$25k.
- **Researcher time** (1.5 FTE, 18 months): $80k–$120k (academic rate; industry higher).
- **Statistics and analysis** (0.5 FTE): $25k–$40k.
- **Miscellaneous** (IRB, data security, contingency): $5k–$10k.

**Total: $180k–$260k.** The minimum sample and duration to generate transition probabilities and dwell-time distributions with confidence intervals narrow enough to be useful for V6.

### Major risks

1. **Mid-study attrition (months 9–12).** Longitudinal studies typically lose 20–30% at the halfway point. Mitigation: mid-study bonus, compelling quarterly trajectory reports, explicit pre-commitment.

2. **Major AI releases causing confounding.** A transformative model release in month 6 will trigger regressions that may obscure baseline patterns. Mitigation: this is data, not confound. Analyze "normal transitions" and "release-triggered transitions" separately.

3. **Domain-specific dropout.** Clinical professionals may drop due to privacy concerns. Mitigation: clear privacy commitments at recruitment, oversample initially (N=220) to hit N=200 at month 18.

4. **Measurement reactivity.** Asking monthly "What state are you in?" may cause more deliberate reflection than otherwise. Mitigation: frame as a log, not assessment. Use passive behavioral logging as primary; self-report secondary.

5. **Coder disagreement.** Two raters may disagree on whether a passage signals S3 Ego Shock versus S5 Understanding. Mitigation: double-code 30%, calculate inter-rater reliability, retrain if reliability drops below 0.70.

## Recommendations

1. **Launch a pilot study within 18 months.** Start with 30 participants (10 per domain) over 9 months to validate the state-classification scheme in real time, refine interview guides, and estimate attrition.

2. **Front-load the highest-information measurement for V6.** Don't wait for full data. By month 9, you'll have enough evidence to publish transition probabilities for the S1 Initial Encounter → S2T Trust Evaluation/S2D Defensive Resistance fork and early S2 → S5 Understanding/S3 Ego Shock transitions. That is the first V6 release. Dwell-time distributions and end-state predictors come later.

3. **Operationalize the S3B Bargaining versus S7A Maturity distinction rigorously.** The current heuristic is plausible but unverified. It is the most practically useful distinction in the model — it tells you whether someone is coping defensively or adapting sustainably. Identify a behavioral signal (such as the pattern of scope changes in response to model releases) before the study begins.

4. **Specify domain primers before the study.** If software engineers show a distinct S3 Ego Shock experience, you want to code it distinctly, not as noise. Write 1–2 page primers for each domain describing what a therapist's "AI for diagnosis" dilemma looks like versus a writer's "AI for ideation" dilemma versus an engineer's "AI for code review" dilemma. Use these to train interviewers and raters.

5. **For software engineers evaluating V5 now, use the qualitative structure.** You don't need a longitudinal study to use V5 today. The state structure tells you how to think about adoption: expect people in high-stakes professional roles to fork into defensive resistance initially. Expect most to reach identity crisis (S3 Ego Shock). Expect some to stay in negotiated boundaries (S3B Bargaining), and others to move to healthy integration (S7A Maturity) or aggressive expansion (S7B Identity Expansion). Knowing that much tells you to expect a 6–12 month cycle before stability, and to make space for identity work, not just training.
