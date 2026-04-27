This is a simpler rewrite of [006-practitioner-utility.md](006-practitioner-utility.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Practitioner Utility — Plain-Language Version

This review asks one question: if you're a manager or coach, can you actually *use* model V5 on Monday morning? Or is it just a nice picture?

## TL;DR

- From a single conversation, you can reliably spot only three states: S0 Baseline (doesn't use AI), S6A Enthusiastic Overuse (uses AI for everything), and the "D-level" (how much you're delegating). Everything else needs more time or direct self-report.
- You have real influence over a few specific transitions: how someone first reacts to AI (S1 Initial Encounter → S2T Trust Evaluation or S2D Defensive Resistance), whether they settle into a healthy "I'll use it for some things, not others" deal (S2D Defensive Resistance → S3B Bargaining), and the four flavors of overuse (S6A Enthusiastic Overuse/B/C/D).
- The "mechanism anchor" idea (a one-line explanation of *why* each state exists) is only useful for S3 Ego Shock and S6. For earlier states it describes brain wiring you can't change. For end states it doesn't tell you what to do.
- The new two-axis dropout score (rate practical pain 0–10, rate emotional pain 0–10) is less work than it sounds. The "reversibility test" — offering a fixed tool and watching what they say — is the only piece of the model with concrete steps. It cuts decision time roughly in half compared to V4.
- The reversibility test works as a five-minute diagnostic question in a 1:1. It is not a controlled experiment.
- Biggest gap: there's no intake script, no decision tree for figuring out which state someone is in, no scripts for what to actually say in S3B Bargaining or S6 interventions, and no quick way to gauge how much of someone's identity is tied to the work AI is touching.
- V5 is a working theory but not yet a working tool. Use it Monday morning as a frame for thinking about who is stuck where, and as a checklist for what questions to ask. Don't hand it to a manager and expect them to diagnose someone with it. The intake questions and decision trees are still missing.

## Findings

### 1. Which states can you reliably identify from one conversation?

Three, maybe four: S0 Baseline, S6A Enthusiastic Overuse, S6B Dependent Overuse, and D-level.

- **S0 Baseline versus everyone else:** five seconds. "Do you use AI?"
- **S6A Enthusiastic Overuse versus S7D Burnout:** two minutes of usage questions. Pulling AI into everything with energy = S6A Enthusiastic Overuse. Stopped almost completely = S7D Burnout. The volume gap is huge.
- **D-level (how deep is the delegation):** observable in real time. "Summarize this" = D1. "Help me decide between two strategies" = D3–D4.

Everything else is opaque or needs longer:

- **S2T Trust Evaluation (testing fairly) versus S2D Defensive Resistance (testing defensively):** Both look like testing. The tell is **asymmetric updating** — they latch onto bad evidence and ignore good evidence. You can spot this across three or four tries over a few weeks. Not in one conversation. Someone saying "It made a typo, so it's unreliable" while ignoring four hours saved smells like S2D Defensive Resistance, but you can't confirm in one shot.
- **S1 Initial Encounter (first encounter) versus S2T Trust Evaluation versus S2D Defensive Resistance:** You can sometimes separate S1 Initial Encounter by timing (they literally just started). Beyond that you're guessing in a one-shot.
- **S3 Ego Shock (panic and recalibrating) versus S5 Understanding (integrated):** Both will say "I get it now." One is rattled, one isn't. You can poke at it with "How does this change your role?" but the actual internal state is self-report only.
- **S7A Maturity (bounded, healthy use) versus S7B Identity Expansion (expanded, healthy use):** S7A Maturity says "I use it for X, not Y." S7B Identity Expansion says "I use it for X and now I can do things I couldn't before, and that's part of who I am now." You have to ask: "Has using AI changed what you think you're capable of?"
- **S7C Ethical Integration (worried about ethics):** They have to volunteer it. "I keep thinking about what AI means for creativity" or "I'm worried about junior people." Without that cue, no signal.

The model is honest about this. It says only three things are observable in a snapshot. Plan for two or three check-in conversations before you're confident about the harder pairs. You're triangulating, not diagnosing.

### 2. Which transitions can you actually influence?

Five buckets:

**S1 Initial Encounter → S2T Trust Evaluation or S2D Defensive Resistance.** You can't change how much someone's identity is wrapped up in the work (call this **Identity Stakes**). You *can* control how AI gets framed before they form a first impression. Frame it as "a tool for stuff you don't want to do anyway" and low-stakes people lean S2T Trust Evaluation. Frame it as "capability in your craft" and high-stakes people flip to S2D Defensive Resistance faster. Slow the S2D Defensive Resistance flip by separating the tool demo from the role-threat conversation, giving them quick wins where they feel in control, and naming the discomfort early ("This might feel identity-threatening; that's normal").

**S2D Defensive Resistance → S3B Bargaining.** You can help someone draw a line they can live with. Ask "What would you be willing to try it for?" and help them define a specific, measurable scope. The mechanism is **cognitive dissonance reduction** (the brain dealing with two contradictory beliefs by walling one off) — they get to hold "AI is powerful but I control how much of my work it touches." Works best when the scope is somewhere AI is genuinely useful but not central to their identity, when you don't push to expand the scope without their agreement, and when you check in after each major model release because the deal can shake loose if AI suddenly does the protected thing well.

**S2D Defensive Resistance or S3B Bargaining → S5 Understanding.** You can't force this. You can set the conditions. S5 Understanding needs both a coherent personal story about how AI fits *and* social acceptance (AI use is no big deal in their team). Speed up the personal story by teaching them how and when the tool fails, giving them calibration feedback, and walking through a failure together. Speed up the social side by making AI use visible among respected peers (by example, not pressure), treating it as "how we work now" without fanfare, and shielding them from public failure while learning.

**S5 Understanding → S6A Enthusiastic Overuse.** Hard to prevent. Damp it down by making the reward predictable (templates, known limits), removing leaderboards or AI-usage metrics, and asking "What problem were you solving when you started leaning on AI this hard?" If the answer is "none, I was just experimenting," redirect them to a defined project with a bounded role for AI.

**S5 Understanding or S6 → S3 Ego Shock (regression).** You can't stop capability jumps from happening. You can name the regression as normal: "Your mental model broke because the tool changed. This happens." Help them re-evaluate boundaries and notice what skills are still theirs.

**S3 Ego Shock, S6B Dependent Overuse, S6C Driven Overuse, S6D Social Overuse → S7A Maturity or S7C Ethical Integration.** The interventions differ by which driver is in play. That's *why* S6 is split into four states:

- S3 Ego Shock: "What's the core of what you do that AI can't replicate or shouldn't touch?"
- S6A Enthusiastic Overuse (compulsive use): "Where did you lose your judgment? Let's rebuild it."
- S6B Dependent Overuse (lost trust in own judgment): "What made you doubt yourself? How do we rebuild that?"
- S6C Driven Overuse (efficiency for its own sake): "What were you trying to achieve before efficiency became the goal?"
- S6D Social Overuse (peer pressure): "What does this tool actually help *you* do?"

**S6A Enthusiastic Overuse → S7B Identity Expansion.** Notice what the person can newly do, ask them to teach others (so the new skill is externalized and named), and write the new capability into their role.

Most of your leverage is on the S1 Initial Encounter → S2D Defensive Resistance → S3B Bargaining → S5 Understanding path, plus managing S6. Almost no leverage in S7, because S7 is stable. Your job there is support and mentorship, not intervention.

### 3. Do the mechanism anchors help you intervene differently?

Yes for S3 Ego Shock and S6. No for the rest.

Below S3 Ego Shock, the mechanisms describe early-stage cognition: how the brain decides whether something is new, threatening, or worth a closer look. Knowing that S2D Defensive Resistance is "identity-protective cognition" (defending the self by rejecting threatening evidence) tells you positive evidence won't win the argument — change the frame, not the evidence — but the actual intervention is just "reframe," not anything mechanism-specific.

**S3 Ego Shock is where mechanism anchors matter.** S3 Ego Shock is anchored to **self-efficacy collapse** (feeling you can no longer do your job) and **terror management** (the dread that comes with confronting your own replaceability). The right move is not "here's evidence AI isn't as good as you think." It's "I see you confronting your own replaceability. That's real, and it doesn't go away by argument." Then: "What's the core of who you are that isn't threatened?" The mechanism changes the *tone* from "talk them out of it" to "help them rebuild a self-concept that survives the threat."

**S3B Bargaining is partly mechanism-dependent.** Anchored to dissonance reduction by limiting scope. Help them do it cleanly: pick a scope where AI is useful and safe, write the scope down explicitly, don't pressure them to expand it.

**S6 mechanisms are highly actionable.** The four flavors of S6 each need a different move:

- **S6A Enthusiastic Overuse** (variable-reward reinforcement — the slot-machine effect): kill the unpredictability. Standardize templates. Remove metrics that reward AI use.
- **S6B Dependent Overuse** (self-efficacy displacement — "AI thinks better than I do"): rebuild their judgment. Have them grade AI outputs against *their own* thinking, not against AI's thinking.
- **S6C Driven Overuse** (goal substitution — efficiency replaces the original goal): revisit the original goal. "You wanted more time for thoughtful work, not maximum output. Did you actually get the thoughtful time?"
- **S6D Social Overuse** (peer pressure): change the context or the peer group.

Without those anchors, you'd guess.

**S7 mechanisms are explanatory, not prescriptive.** People in S7 are self-regulating. Your job is support, not intervention.

### 4. Does the two-axis dropout score change what you do?

Yes, a lot. And the reversibility test is what makes it usable.

| Scenario | V4 guess | V5 graded reading | What you do |
| --- | --- | --- | --- |
| High practical (8), low emotional (2) | "Practical, give them better tools" | "Yes, tool problem. Urgent." | Treat as a blocker. Find or build a better tool. Weeks. |
| Low practical (2), high emotional (8) | "Emotional, psychological support" | "Identity threat. Real but slower." | Treat as identity work. No tool will fix this. Months. |
| High both | "Unclear" | "Mixed. Tool failed in an identity-loaded spot." | Fix the tool first. Once it works, the emotional severity often drops because the rationalization clears. Then identity work if needed. |
| Low both | "Just not interested" | "Confirmed: not interested." | Don't intervene. |

The reversibility test makes it concrete. "You said it kept losing context. If I could give you a version that remembered context, would you try again?" Listen to both the answer and the tone:

- "Yes, absolutely" — practical-driven.
- "Maybe, but honestly I'm just tired of all this" — emotional-driven.
- "I could try but I don't know if it matters" — mixed, leaning emotional.

The 0–10 scale forces you to be honest about the split. It blocks the lazy choice of "I can't fix the tool, so it must be emotional." Maybe it's 50/50 and you can fix half of it.

### 5. Is the reversibility test executable in a real workplace?

As a diagnostic question, yes. As a controlled experiment, no.

Five minutes in a 1:1:

1. "I heard you stopped using ChatGPT because [their stated reason]. What would the tool need to do to make that reason go away?"
2. Listen for "It would need to [specific technical thing]" versus "I don't know, I'm just over it" versus "Maybe, but I'm burned out."
3. Note the tone. Practical (engineering problem), emotional (motivational problem), or mixed (tired and stuck).
4. Optional: if you have a workaround handy, offer it — but only if practical pain was driving the exit.

Real obstacles: people often have no clear stated reason ("It just didn't work for me"), time has passed, and they may not want to re-engage. The test is a triage question, not an experiment. Use it.

### 6. What's missing to turn V5 into a working tool?

In order of urgency:

**1. Intake protocol (CRITICAL).** A short structured conversation to narrow down which state someone is in. The model gives you state definitions but no questions to ask. A five-minute decision tree could look like this:

- "How long have you been using AI for work?" (places them past S0 Baseline)
- "How much of your core work could AI do?" (signals Identity Stakes without making it a therapy session)
- "When you tried it, what was your first reaction?" (S1 Initial Encounter flavor)
- "Are you testing it carefully, or nitpicking it?" (S2T Trust Evaluation versus S2D Defensive Resistance)
- "If you use it now, what stops you from using it more?" (S3B Bargaining boundary versus S5 Understanding maturity versus dropout)

**2. Mechanism-specific intervention scripts (HIGH).** For each of S3 Ego Shock, S3B Bargaining, S6A Enthusiastic Overuse, S6B Dependent Overuse, S6C Driven Overuse, S6D Social Overuse: "if the person is here, ask this." Just a list of good questions. Example for S3 Ego Shock:

- "Help me understand what this threatens about your role."
- "If AI can do X, what can you do that AI can't?"
- "What's the core of your identity that's separate from this skill?"

Example for S6B Dependent Overuse:

- "When you use AI, do you check its output against your own thinking, or against AI's thinking?"
- "What made you stop trusting your own judgment?"

**3. Identity Stakes shortcut (HIGH).** Three questions, ninety seconds:

- "How many years did you train to get good at this?"
- "When you do this skill, how much of your self-image is tied to doing it well?"
- "If someone else did this task faster with AI, what would that say about you?"

The third question is the real one. A defensive answer = high stakes. "Nothing, it's just a tool" = low stakes.

**4. D-level calibration guide (MEDIUM).**

- D1: "I'm using AI to summarize, extract, or organize information I already had."
- D2: "I'm handing off a skill task but I'm reviewing and editing the output."
- D3: "I'm asking AI to brainstorm, strategize, or draft something new that I then refine."
- D4: "I'm asking AI to make decisions, or I'm using autonomous AI."

Practitioner question: "For the work you stopped using AI for, were you mostly handing off specific tasks (D2), or asking it to think with you (D3–D4)?"

**5. S3B Bargaining boundary-setting template (MEDIUM).**

- "What domain or task type would you be willing to try AI for?"
- "Why does this feel safe?"
- "Let's be explicit: you're using AI for [X], not for [Y]. Agreed?"
- "When a new AI release comes out, we check whether it changes what's safe in [X]. Agreed?"
- "Check-in: does this boundary still feel right?"

**6. Longitudinal tracking for the hard pairs (MEDIUM).**

For S2T Trust Evaluation versus S2D Defensive Resistance: ask the same question twice. First time, listen for openness versus defensiveness. Second time, two weeks later after they've tried it: did they update based on evidence (S2T Trust Evaluation), or did they find new reasons to dismiss (S2D Defensive Resistance)?

For S3B Bargaining versus S7A Maturity: when a new AI capability crosses their boundary, do they re-evaluate based on evidence ("Let me test this carefully") or just slide the boundary without testing (S3B Bargaining)?

**7. End-state stabilization guide (LOW).**

- S7A Maturity: feedback on calibration. Don't second-guess their boundaries.
- S7B Identity Expansion: celebrate the expansion. Ask them to teach others.
- S7C Ethical Integration: take their ethical questions seriously. Don't dismiss them.
- S7F Evangelism: clear the path for them to mentor.

V5 is 80% of a working tool. The missing 20% is the operational part: the questions, the trees, the templates.

## Recommendations

1. **Build the intake protocol first.** Five-minute conversation that narrows states. Prerequisite for everything else.

2. **Add mechanism-specific intervention scripts.** For S3 Ego Shock, S3B Bargaining, S6A Enthusiastic Overuse, S6B Dependent Overuse, S6C Driven Overuse, S6D Social Overuse: the questions to ask and what each one is supposed to unlock.

3. **Add the Identity Stakes shortcut.** Three questions, ninety seconds.

4. **Clarify D-level definitions with examples.** Add the real-world signal: "What does delegating a design vision look like versus delegating a design task?" (D3 versus D2.)

5. **Add the S3B Bargaining boundary-setting template.** Explicit agreement, check-in protocol, trigger to renegotiate. Makes S3B Bargaining usable as a stable place to live.

6. **Document what to track over time.** For practitioners who can't diagnose S2T Trust Evaluation versus S2D Defensive Resistance or S3B Bargaining versus S7A Maturity in a snapshot, what should they notice over weeks and months? When should they re-assess?

7. **Drop or measure the S7F Evangelism prerequisite.** Either gather longitudinal data to test the claim that S7F Evangelism evangelists were once in S3 Ego Shock, or reframe it as "typically more stable if they've been through S3 Ego Shock; we don't yet know if it's required."

8. **Test the reversibility test.** Use it with 50 actual dropouts and see if the tone-based diagnosis matches what happens. Report back.
