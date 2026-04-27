# Longitudinal and Dynamics — Plain-Language Version

This is a simpler rewrite of [009-longitudinal-dynamics.md](009-longitudinal-dynamics.md). Same findings, plain language. If you've read the original and it landed, skip this one.

## What this review is about

The model V5 lays out a sequence of states people pass through when adopting AI: initial reaction, identity wobble, negotiation, integration, and so on. What V5 does **not** say is the **timing**. How long do people sit in each state? How likely is a transition from one state to the next? Which path are they on?

This review checks whether V5 is right to leave those numbers out, and what it would take to fill them in later.

## TL;DR

- V5 leaves out transition probabilities (chance of moving from one state to another) and dwell times (how long people stay in each state). That is the right call. Made-up numbers are worse than no numbers.
- V6 should add numbers, but only after a real study. Until then, V6 should at least list which transitions are worth measuring and what evidence would justify the numbers.
- Five timing questions matter most: how long people stay stuck in defensive resistance or in negotiation; what makes someone end up in healthy integration (S7A Maturity) versus aggressive expansion (S7B Identity Expansion); how often people loop through the model again as new AI comes out; who recovers from burnout versus quits for good; whether the model behaves the same in software, creative work, and clinical work.
- A 200-person, 18-month study across three professions would produce solid numbers for roughly $180k–$280k.
- The most useful data is **behavioral**: how often people open the tool, what they use it for, when they switch tools. Asking them how they feel is secondary, because people lie about their feelings (to themselves and to researchers). They can't lie about whether they opened the tool.
- The state structure and the core mechanisms hold up. What's missing is timing. A V6 with fake numbers would be worse than V5. A V6 that maps out how to get real numbers would be much better.

## Findings

1. **The first fork is well-grounded.** When someone first meets AI in their work, V5 says they split into two groups: those whose professional identity is heavily tied to their skills tend to react defensively (S2D Defensive Resistance), and those without that identity stake tend to just try the tool (S2T Trust Evaluation). This matches existing research on identity threat. The bigger your identity stake, the more threatening a competing tool feels at first. This is the most important branch to put real numbers on.

2. **The state structure itself holds.** Each state lines up with a real psychological mechanism that has been studied. S2D Defensive Resistance matches defensive coping. S3 Ego Shock matches identity crisis (the disorientation when something you believed about yourself is suddenly in question). S5 Understanding matches the resolution phase. The structure isn't arbitrary; it tracks real research.

3. **The missing piece is state-entry timing.** V5 doesn't say how long someone typically sits in S2D Defensive Resistance before moving to S3 Ego Shock. It doesn't say whether some people stay weeks while others stay months. Same for S3B Bargaining (the negotiation state, where someone draws lines about what AI can and can't touch). If most people pass through S3B Bargaining in three months, that's healthy adaptation. If they stay there one or two years, it's a stable defensive position that needs different help. A study would tell you which.

4. **Time-in-state varies a lot, especially in the rough states.** S2D Defensive Resistance and S6D Social Overuse (severe burnout) are emotionally chaotic. One person snaps out of it quickly; another stalls. S7A Maturity (the healthy stable end-state) can last for years. Without knowing the spread (typical case, range, what the worst cases look like), you can't tell whether someone is still on a normal trajectory or has gotten stuck. For organizational teams, this is the central practical question.

5. **End-state predictors are actionable and testable.** V5 says four end-states fan out from S5 Understanding: healthy integration (S7A Maturity), aggressive scope expansion (S7B Identity Expansion), retreat to lower scope (S7C Ethical Integration), or burnout (S7D Burnout). If you can predict which one someone will land in based on their domain, their workplace, their prior experience, and how they handled S3 Ego Shock, you can design conditions that push people toward S7A Maturity and away from S7D Burnout. Directly useful for team design.

6. **Regression after model releases is testable but not yet measured.** V5 says when a new AI model launches, people who were in stable states (S5 Understanding or S7) often slide back toward S3 Ego Shock (identity questioning). This is **testable**. After the next major release (such as a new GPT or Claude version), measure what fraction of previously stable users slide back, and how long it takes them to climb out. This requires tracking the same people before and after the release, not a one-time survey.

7. **Domain variation is named but not pinned down.** V5 says the experience varies across software engineering, creative work, and clinical work, but doesn't say what varies. Does a clinical psychologist's identity crisis unfold faster than a writer's? If you watch 10 software engineers and 10 therapists, both in S3 Ego Shock, are you seeing the same thing or two different things wearing the same label (a therapist's S3 Ego Shock dominated by patient-privacy worry versus an engineer's S3 Ego Shock dominated by code-correctness worry)? The study should answer this with 60–70 people per domain.

8. **The dropout picture is measurable but lacks anchors.** V5 splits dropout along two axes — how badly the tool failed practically, and how bad the experience felt emotionally. Right now both axes are described in words, with no anchors. To make the picture useful, you need rules such as: "practical severity above 7 means the tool failed on more than half the person's tasks" and "emotional severity above 7 means the person reports anxiety in their exit interview." The study should set those anchors and then count how many people fall in each quadrant.

9. **Cycling frequency is unknown but matters for adoption rhythm.** V5 says "most people cycle through more than once," but doesn't say how often. If a typical person re-enters the cycle every six months, AI adoption is constant pressure on the team and needs ongoing support. If it's once every three to five years, it's more of an occasional event. This changes how you pace training and organizational change.

10. **Burnout recovery versus permanent dropout isn't separated.** V5 lists S7D Burnout (burnout) as a possible outcome but doesn't say what fraction of burned-out people eventually return (back to S5 Understanding or S7A Maturity) versus drop out for good. If 80% recover after rest, the model is about temporary overload. If 50% are permanent dropouts, burnout is terminal and prevention has to come first. This is testable: ask people who dropped out whether they would resume use if the tool got better or their context changed (a reversibility test).

11. **A minimum-viable study is achievable and specific.** The design below — 200 participants, three professional domains, 18 months, behavioral logging plus quarterly interviews — would produce transition probabilities and time-in-state distributions with confidence intervals tight enough to be useful for V6. The cost is $180k–$280k. Substantial, but defensible for a model that affects how teams adopt AI and whether individuals burn out.

12. **The study bets on behavior over self-report.** Track AI usage (how often the tool is launched, what for, whether they switch tools), ask once a month about scope changes, then do a 30–45 minute interview every three months about identity and emotional state. Behavioral data is more reliable because, as noted in the TL;DR, people lie about their feelings but can't lie about whether they opened the tool.

## Minimum-viable study design

A three-arm, 18-month panel study (the same people tracked over time) with measurement at the start, every three months, and an extra check-in after major AI releases.

### Participants

- **Total: 200 people.** 70 software engineers, 70 creative writers or content creators, 60 clinical or educational professionals (therapists, educators, medical residents). Spans low-stakes professional use (writing), high-stakes technical work (code review, debugging), and high-stakes relational work (diagnosis, treatment).
- **Inclusion criteria:** age 18 or older, at least one year of professional experience, fluent in English, and at least one month of AI tool use before joining.
- **Recruitment:** 60% through professional networks, 40% through general labor platforms. Aim for a roughly even gender mix and an age range of 20–60.

### Measurement schedule

- **Baseline (week 1):** demographics, professional background, prior AI use, openness to new experiences, risk tolerance.
- **Monthly check-in (5 minutes):** which state best fits how they feel right now, plus AI usage volume (hours per week, what they used it for, which tools).
- **Quarterly deep interview (30–45 minutes, at months 1, 4, 7, 10, 13, 16):** structured interview covering state transitions, emotional experience, scope boundaries, identity reflection. Audio recorded and transcribed.
- **Event-triggered follow-up:** within two weeks of any major model release, an extra check-in to capture the timing of any regression.

### What gets measured

1. **Usage telemetry (passive logging):** weekly tool launches, what categories of work, how often they switch tools. Lots of tool-switching plus shifting scope signals S3B Bargaining (negotiation). Steady high volume plus enthusiasm signals S6A Enthusiastic Overuse. Declining volume plus statements like "I need a break" signals S7D Burnout.

2. **Monthly scope statement:** "What do you currently use AI for, and what do you explicitly refuse to use it for?" Coded month over month for whether the lines are stable or shifting under pressure. In S7A Maturity, lines move only when new evidence arrives. In S3B Bargaining, lines move when the person feels pushed.

3. **Quarterly interview analysis:** open-ended questions about emotional experience, identity, and how they decide what AI should and shouldn't do. Coded by two independent raters for: S3 Ego Shock versus S5 Understanding signals (identity-threat language versus reframing language); S7A Maturity versus S7B Identity Expansion signals (sustainable-stewardship language versus expansion language); emotional severity for dropouts (rated 0–10, aiming for inter-rater agreement above 0.75); and domain-specific patterns.

4. **Behavioral log of one focal task per domain:** for example, code review for engineers, first-draft writing for writers, treatment planning for clinicians. Every three months: did AI assistance go up, down, or stay flat? Did scope change? Did the person's own quality assessment change? More reliable than asking "What state are you in?"

5. **Exit interview for dropouts:** when someone stops using the tool, a brief interview asking about practical severity (did the tool actually fail on real tasks?) and emotional severity (was there threat, identity worry, exhaustion?). Then four weeks later, a follow-up: if you swapped in a high-quality alternative, would you use it? A "yes" means the tool was the issue. A "no" means the feelings were the issue.

### Retention and incentive

- **Monthly check-in:** expect 95% to stay engaged; low effort.
- **Quarterly interview:** expect 85% to stay engaged; pay $15 per completed interview ($60 per quarter per person).
- **Attrition management:** pay everyone $10 at month 9 (mid-study) to reduce mid-study dropout.

### Cost estimate

- **Recruitment and screening** (200 people): $5k–$8k.
- **Participant compensation** (200 × $60 quarterly + $10 mid-study + $200 completion): $56k.
- **Interview transcription and analysis:** $12k–$18k.
- **Behavioral logging infrastructure:** $15k–$25k.
- **Researcher time** (1.5 full-time equivalents, 18 months): $80k–$120k at academic rates; industry rates would be higher.
- **Statistics and analysis** (0.5 full-time equivalent): $25k–$40k.
- **Miscellaneous** (ethics review, data security, contingency): $5k–$10k.

**Total: $180k–$260k.** This is the minimum sample and duration to get transition probabilities and time-in-state distributions tight enough to be useful for V6.

### Major risks

1. **Mid-study dropout (months 9–12).** Long studies typically lose 20–30% of people at the halfway point. Mitigation: the mid-study bonus, sending compelling progress reports, and asking participants to commit up front.

2. **A major AI release messing up the data.** A transformative model release in month 6 will trigger regressions that obscure baseline patterns. Mitigation: treat this as data, not a problem. Analyze "normal transitions" and "release-triggered transitions" separately.

3. **Domain-specific dropout.** Clinical professionals may quit the study over privacy concerns. Mitigation: clear privacy commitments at recruitment, and over-recruit at the start (220 people) to land at 200 by month 18.

4. **The act of measuring changing the thing measured.** Asking someone every month "what state are you in?" may make them reflect more deliberately than they otherwise would. Mitigation: frame the monthly check-in as a log, not an assessment. Lean on passive behavioral logging as the primary signal; treat self-report as secondary.

5. **Coders disagreeing.** Two raters may disagree on whether a passage signals S3 Ego Shock or S5 Understanding. Mitigation: double-code 30% of the material, calculate inter-rater reliability, and retrain if it drops below 0.70.

## Recommendations

1. **Run a pilot study first.** Start with 30 people (10 per domain) over 9 months to make sure the state classification works in real time, refine the interview guides, and estimate dropout.

2. **Front-load the highest-information measurement for V6.** Don't wait for the full data set. By month 9 you'll have enough evidence to publish transition probabilities for the first fork (S1 Initial Encounter → S2T Trust Evaluation or S2D Defensive Resistance) and the early S2 → S5 Understanding or S3 Ego Shock transitions. Release that as the first V6 update. Time-in-state distributions and end-state predictors come later.

3. **Pin down the S3B Bargaining versus S7A Maturity distinction rigorously.** The current rule for telling them apart is plausible but unverified. It is also the most practically useful distinction in the model — it tells you whether someone is coping defensively or adapting in a sustainable way. Identify a behavioral signal (such as the pattern of how scope changes after a model release) before the study starts.

4. **Write domain primers before the study.** If software engineers go through a distinctly different S3 Ego Shock than writers do, you want to code those differences as real, not as noise. Write a 1–2 page primer for each domain describing what each profession's identity dilemma actually looks like: a therapist's "AI for diagnosis" worry, a writer's "AI for ideation" worry, an engineer's "AI for code review" worry. Use these to train interviewers and raters.

5. **For software engineers using V5 today, lean on the qualitative structure.** You don't need a longitudinal study to use V5 right now. The state structure tells you how to think about adoption: expect people in high-stakes professional roles to fork into defensive resistance at first; expect most to reach identity crisis (S3 Ego Shock); expect some to settle into negotiated boundaries (S3B Bargaining), others to move into healthy integration (S7A Maturity), others into aggressive expansion (S7B Identity Expansion). Just knowing that pattern tells you to expect a 6–12 month cycle before things stabilize, and to make space for identity work, not just training.
