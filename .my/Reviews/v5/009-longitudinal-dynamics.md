# Longitudinal Dynamics Review — Model V5

## TL;DR

- V5 deliberately omits transition probabilities and dwell times because fabricating numbers is worse than admitting they don't exist. That stance is correct.
- V6 should add numerical dynamics, but only after a longitudinal study yields real data. Without data, V6 should specify *which transitions* are candidates for quantification and *what kind of measurement* would justify numbers for each.
- Five dynamics questions stand out: (1) How long do people stay in defensive resistance or bargaining before moving forward? (2) What determines whether someone exits into Maturity (S7A) vs Identity Expansion (S7B)? (3) How often and under what conditions do people cycle through the model as AI capabilities grow? (4) What predicts burnout duration and recovery vs permanent dropout? (5) Does the model hold across professional domains, or are domain-specific substates required?
- A 200-person 18-month panel study across three professional domains (software engineering, creative writing, clinical work) would generate defensible transition data and cost roughly $180k–$280k all-in.
- The highest-ROI measurement is behavioral logging of AI usage frequency, scope changes, and tool-switching, combined with monthly structured interviews. Self-report questionnaires are secondary.

## Verdict

V5 is honest about what it doesn't know. That honesty is its strength. The model's state structure and mechanism anchors hold up under scrutiny—each state maps clearly to documented psychological processes, and the fork at S1 (low stakes → S2T, high stakes → S2D) is well-grounded in identity-threat literature. What V5 lacks is empirical timing: how fast do transitions happen, what variance exists, and which variables predict which exit from a state. A V6 that adds fabricated numbers will be worse than V5; a V6 that specifies a roadmap for real quantification will be much more useful. The study design below is achievable and would yield that roadmap.

## What V6 Dynamics Layer Should Specify

A V6 dynamics layer should not add numbers until data supports them. Instead, it should make these concrete commitments:

1. **Transitions to quantify immediately** — For S1→S2T, S1→S2D (the branch probabilities based on Identity Stakes), and S2T→S5 and S2D→S3 (the forward-motion transitions): once a 200-person longitudinal sample exists, estimate transition probabilities at 3-month intervals and report confidence intervals. These are the highest-stakes branches—quantifying them is worth the sample size.

2. **Dwell-time distributions to measure** — For S2D (defensive resistance), S3B (bargaining), and S6A–S6D (overuse states): measure median time in state, 25th/75th percentiles, and whether the distribution is log-normal or heavy-tailed. These states are psychologically volatile; their duration varies wildly, and knowing that variation is essential for modeling intervention timing.

3. **Hazard rates for end-state entry** — For S7A vs S7B vs S7C vs S7D: specify what makes someone more likely to land in each end state. This is not a pure transition probability (the denominator is people who reached S5, not all people); it is a competing-risk model where the risk factors include domain type, organizational context, prior identity work (passage through S3), and measured cognitive style.

4. **Regression triggers and re-entry rates** — Operationalize the claim that "model releases" and "capability jumps" re-trigger S3 from S5–S7 states. Measure: for each released model, what fraction of S5+ users regress to S3, and how long does the regression last? This requires tracking people who were already stable before a release event.

5. **Dropout severity axes and intervention thresholds** — For the "practical severity × emotional severity" plane: define measurable anchors for each axis (e.g., "practical severity > 7" = tool failed on >50% of tasks; "emotional severity > 7" = person reports anxiety or identity threat on exit interview) and report the contingency table (practical × emotional) for observed dropouts.

6. **Cultural and domain substates** — The model specifies that intensity varies by culture and domain, but doesn't name what varies. V6 should specify: if you measure a software engineer in S3 vs a clinical psychologist in S3, what is different? Are the mechanisms identical but the surface behavior different, or do substates exist? This requires 3+ professional domains with adequate sample size in each.

## The 3–5 Dynamics Questions That Matter Most

These are the questions whose answers would most change how you *use* the model for intervention design, team adoption strategy, or individual support.

1. **How long do people stay stuck in S2D (defensive resistance) or S3B (bargaining)?** — If median time in S2D is 2 weeks, you intervene one way; if it is 6 months, you intervene differently. Same for S3B: if most people move through it in 3 months, bargaining is a healthy coping mechanism; if they stay for 1–2 years, it's a stable defensive posture and requires different support. Answer changes: how to time organizational change, whether to force motion or wait, what maturity looks like for that domain.

2. **What determines whether a person reaches S7A (healthy maturity) vs S7B (identity expansion) vs S7D (burnout)?** — All three are outcomes of S5 (Understanding). If we can predict which path a person will take based on measured variables before S5 (prior domain expertise, regulatory environment, organizational incentives, cognitive openness), we can shape the conditions that lead to healthy stability instead of unsustainable expansion or burnout. Answer changes: how to design teams and workflows to favor S7A.

3. **How many times do people cycle through the model as AI capabilities grow?** — V5 notes that "most people cycle more than once" but is silent on frequency. If the typical person cycles 2–3 times per year as major models release, the model is a continuous pressure; if cycling happens once per 3–5 years, the model is more of an episodic shock. Answer changes: how frequently you expect regressions, what rhythm of organizational support is needed, how much fatigue to expect.

4. **What predicts whether a person exits S7D (burnout) by returning to S5/S7A vs exiting completely?** — Burnout is reachable from any S6 state. Some people return after a break; others leave permanently. What separates them? Is it organizational flexibility, prior identity work, cognitive style, or simple resource recovery time? Answer changes: whether burnout is a recoverable state (design for re-entry) or a terminal dropout (minimize the risk of entering).

5. **Does the state structure hold identically across professional domains, or do domain-specific substates exist?** — Software engineers, clinical psychologists, and visual artists may all go through S3 (ego shock), but the experience and duration might differ enough to require substates (e.g., S3-Technical vs S3-Relational). If substates are necessary, your interventions must be domain-tuned. If the structure is universal, you can use the same state-transition language across very different professions. Answer changes: whether to specialize the model or keep it universal.

## Minimum Viable Study Design

A three-arm, 18-month panel study with measurement at baseline, 3-month intervals, and event-triggered follow-ups after major AI model releases.

### Sample and Arms

- **Total N = 200** across three professional domains: 70 software engineers, 70 creative writers or content creators, 60 clinical or educational professionals (therapists, educators, medical residents). These domains span low-stakes (writing), high-stakes-technical (engineering), and high-stakes-relational (clinical work), covering the Identity Stakes × Task Delegation space.
- Inclusion: 18+ years old, 1+ years professional experience, English-fluent, 1+ month of AI tool exposure before enrollment.
- Recruitment: 60% through professional networks (GitHub, Medium/Substack, therapy associations), 40% through general platforms (Prolific, Upwork). Target roughly equal gender distribution and 20–40 years age range.

### Measurement Cadence

- **Baseline assessment** (pre-enrollment or week 1): demographic data, domain experience, prior AI exposure, cognitive style (10-item openness-to-experience scale), risk appetite.
- **Monthly check-in** (5-minute touchstone): binary state classification (self-reported: "Which description matches your current relationship with AI best?") + usage volume (hours/week, categories used, tools currently active).
- **Quarterly deep interview** (30–45 minutes, every 3 months at months 1, 4, 7, 10, 13, 16): structured interview with probes for state transitions, emotional experience (one-item affect scale), decision logic for scope boundaries, identity reflection.
- **Event-triggered follow-up** (within 2 weeks of any major model release or tool lifecycle event): additional monthly check-in to capture transition timing around capacity jumps.

### Instruments (Operationalization of State and Severity)

Rather than questionnaires, the study relies on behavioral logging and interview content analysis:

1. **Usage telemetry** (passive logging, with consent): frequency of AI tool launches per week, category distribution (e.g., "coding assistance," "content generation," "research/analysis"), tool-switching behavior (staying with one tool vs trying new tools in the same domain). High switching rate + high scope negotiation in monthly check-ins signals S3B; stable high volume + enthusiasm signals S6A; declining volume + explicit statements about needing a break signals S7D.

2. **Monthly scope statement** (self-reported): "What tasks do you currently use AI for, and what tasks do you explicitly don't use AI for?" Coded for scope boundary stability (S7A boundaries move on evidence; S3B boundaries move on capability pressure) and scope breadth. Scope contraction over time + emotional language signals S3B or S2D.

3. **Quarterly semi-structured interview** (audio-recorded, coded by two raters independently): open-ended questions about emotional experience ("How do you feel when you use AI for your main work tasks?"), identity work ("Do you think of AI as part of your professional skill set, or as a tool you use?"), boundary logic ("If a new AI model could do X, would you use it for X? Why or why not?"). Coded for:
   - **S3 vs S5 signal**: presence of identity-threat language (e.g., "I worry that my skills won't matter") vs reframing language (e.g., "I can focus on judgment while it handles routine work").
   - **S7A vs S7B signal**: identity expansion language (e.g., "I can do things I couldn't before") vs mature-stewardship language (e.g., "I know where it helps and where I'm still necessary").
   - **Emotional severity of any dropout reason**: coded 0–10 by raters (interrater reliability target ICC > 0.75).
   - **Domain-specific experience markers**: what's domain-specific vs universal in the state experience?

4. **Behavioral log of AI usage** (sampled or participant-reported): track a single "focal task" per domain (e.g., "code review" for engineers, "first-draft writing" for writers, "treatment-planning" for clinicians). For each focal task, quarterly: Did AI assistance volume increase, decrease, or stay the same? Did scope change? Did output quality (by participant's own assessment) change? These behavioral markers are much more reliable than self-report about state than asking "Are you in S6A or S7A?"

5. **Two-axis dropout severity** (if participant drops): exit interview with practical-severity and emotional-severity probes. For practical: "Did the tool fail on specific, reproducible tasks?" (evidence: yes → practical severity >5). For emotional: "Was there a sense of threat, identity worry, or exhaustion?" (evidence: yes → emotional severity >5). Reversibility test: 4 weeks post-dropout, if tool is replaced with a high-quality alternative, would they resume use? (yes → practical was primary; no → emotional was primary).

### Sampling and Cadence

- **Monthly 5-minute check-in**: ~95% retention expected; low friction.
- **Quarterly 30-min interview**: ~85% retention expected; incentivize with $15 per completed interview ($60/quarter per person).
- **Event-triggered follow-up**: triggered automatically when a major model release is announced (e.g., GPT-5, Claude-3-Opus-Pro); expect 3–4 releases during the study window.
- **Attrition management**: $10 bonus per person at month 9 (mid-study check-in) for participants who maintain compliance.

### Cost Estimate (Rough Order of Magnitude)

- **Recruitment and screening** (200 participants): $5k–$8k (depends on recruitment channel mix; internal networks are cheaper than Prolific).
- **Compensation** (200 participants × $60 quarterly interviews + $10 mid-study bonus + $200 completion bonus): $56k.
- **Interview transcription and coding** (quarterly interviews, N=200, 4 cycles, ~40 min each; 2 raters per transcript for subset): $12k–$18k (transcription + coding labor).
- **Behavioral logging infrastructure** (consent management, passive logging tools, data pipeline): $15k–$25k.
- **PI and co-investigator time** (study design, interview guide refinement, data oversight, analysis, 1.5 FTE for 18 months): $80k–$120k (academic rate; industry rate higher).
- **Statistics and data analysis** (transition-probability estimation, hazard-rate fitting, domain-comparison analysis, report writing, 0.5 FTE): $25k–$40k.
- **Contingency and misc** (IRB approval if needed, data security, miscellaneous costs): $5k–$10k.

**Total: $180k–$260k for a defensible 200-person, 18-month study.**

This is not a vanity project; it is the minimal sample and duration to generate transition probabilities and dwell-time distributions with confidence intervals narrow enough to be useful for V6.

### Key Risks and Mitigation

1. **Attrition in months 9–12** — Many longitudinal studies lose 20–30% of participants around the midpoint. Mitigation: mid-study bonus ($10/person at month 9), compelling quarterly reports to participants showing their own trajectory, simple pre-commitment at enrollment.

2. **Confounding by major AI releases** — If a transformative model releases in month 6, you will see a wave of regressions that drown out the normal transition baseline. Mitigation: this is not a confound; it is data. You want to measure regression rates around capacity jumps. Design analysis to separate "normal transitions" from "release-triggered regressions."

3. **Domain-specific attrition rates** — Clinical professionals may drop due to privacy concerns or time constraints; writers may lose interest if they've already formed a stable relationship with AI. Mitigation: recruit with clear privacy commitments, track domain-specific attrition rates separately, oversample initially (N=220) to target N=200 at month 18.

4. **Measurement reactivity** — Asking someone every month "What state are you in?" may cause them to think about state more deliberately than they otherwise would. This is mild; monthly check-ins are low-friction enough that the effect is small. Mitigation: frame check-ins as a log, not an assessment; use passive behavioral logging as the primary signal, self-report as secondary.

5. **Interview coder drift** — Two coders rating interview transcripts may disagree on whether a passage signals S3 vs S5 or S7A vs S7B. Mitigation: double-code a random 30% of interviews, calculate interrater reliability (ICC), retrain coders if ICC < 0.70, include disagreement resolution in the data (report both codings if ICC remains low for that item).

## Recommendations

1. **Launch a pilot study within the next 18 months.** A full 200-person study is a multi-year commitment and a six-figure budget. Start with 30 participants (10 per domain) over 9 months to validate measurement procedures, refine interview guides, and estimate attrition rates. Pilot data will show whether the state-classification scheme works in real time and whether behavioral logging is feasible.

2. **For a V6 timeline, front-load the highest-information measurement.** Don't wait for 18 months of full data. By month 9, you will have enough evidence to publish transition probabilities for the S1→S2T/S2D fork and early S2→S5/S3 transitions. That is the first V6 installment. Dwell-time distributions and end-state predictors come later as data accumulates.

3. **Operationalize the S3B vs S7A heuristic rigorously.** The current heuristic (S3B boundaries move under pressure; S7A boundaries move on evidence) is plausible but unverified. It is the most practically useful distinction in the model because it tells you whether someone is coping defensively or adapting sustainably. A behavioral signal that distinguishes them (e.g., pattern of scope changes in response to model releases) is more important than 200 survey questions.

4. **Plan domain-specific substates before the study.** If the software engineering cohort shows a distinct S3 experience—faster progress through S2D, different emotional flavor, different exit points—you will want to code that distinctly, not as noise. Brief domain primers (what a clinical psychologist's "AI for diagnosis support" dilemma looks like vs a writer's "AI for ideation" dilemma) will help interviewers and coders spot domain-specific patterns early.

5. **If you are a software engineer assessing this for your organization, interpret "numerical dynamics" pragmatically.** You do not need to wait for a longitudinal study to use V5. The state structure tells you how to think about adoption: expect people in high-stakes domains (your domain) to fork into defensive resistance; expect most of them to reach identity crisis (S3); expect some to stay in negotiated boundaries (S3B) indefinitely, and others to move to healthy integration (S7A) or even identity expansion (S7B). Knowing that much tells you to expect a 6–12 month cycle before stability, and to make space for identity work (not just training). Numbers would refine that calendar, but the qualitative structure is actionable now.
