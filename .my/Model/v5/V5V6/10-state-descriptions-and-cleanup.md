# Slice 10 — State Descriptions and Cleanup

Covers source items **14c** (S6 observation guide), **14f** (remove grief language from S3E), and **17** (per-state description updates from 1-Answers-Model5.md sections K, F.6, and G).

---

## Item 14f — Strip grief language from S3E Ego Shock

### What the source asks for

Remove "grief," "grieving," and "loss" from S3E Ego Shock. Replace with "identity disruption," "self-efficacy confrontation," or "existential discomfort."

### Concrete change

In `states/S3E-ego-shock.md`, scan for and replace:

| Remove | Replace with |
| --- | --- |
| grief / grieving | existential discomfort |
| loss of identity | identity disruption |
| mourning | reckoning |
| stages of grief | phases of identity disruption |

The voice-of-person quote stays as-is (*"If AI can do this… what does that make me?"*) — it captures the existential register without using clinical grief language.

The mechanism reference to "terror management in the loose sense" is fine — that is a named theoretical construct, not a grief metaphor.

---

## Item 14c — S6 Observation Guide

### What the source asks for

A concrete observation guide for practitioners: what to look for in real life to distinguish the four S6 states.

### Where it lives

`observation-guide.md` (top-level, not inside states/).

### Content

```markdown
# Observation Guide

Practitioner-facing. What to look for when you are trying to identify which state someone is in. Not a diagnostic instrument — a set of heuristics for orienting a conversation or an observation.

---

## S6 States: distinguishing them in practice

All four S6 states share high AI usage volume. The driver differs.

### S6E — Enthusiastic Overuse

**What it looks like:**
- Usage spikes align with reward moments: a fresh model release, a team demo, a positive reaction to an AI-produced output.
- The person talks about AI with energy and little critical distance.
- They try AI on problems where it is the wrong tool and are surprised when it fails.
- Output volume is up; output quality is variable and the person doesn't track it.

**Key question to surface it:** "When was the last time AI surprised you in a bad way? What did you do with that?"
An S6E person will either not have an answer or will quickly pivot back to a positive memory.

**What to watch:** usage patterns against reward timing. If adoption spikes follow moments of social praise or impressive outputs, variable-reward reinforcement is running. Remove the leaderboard, remove the demo — see if usage drops or shifts to more deliberate patterns.

---

### S6S — Dependent Overuse

**What it looks like:**
- High AI use but anxious affect, not enthusiastic affect.
- The person checks AI output against other AI output rather than against their own judgment.
- Self-reported confidence in their own work has declined since adoption.
- They struggle to make decisions without AI involvement, even for tasks they handled comfortably before.

**Key question to surface it:** "If AI were unavailable for a week, what would you do differently?"
An S6S person will express more anxiety about this than the work difficulty actually warrants.

**What to watch:** changes in self-confidence over time relative to AI adoption. Also: does the person seek AI for low-stakes tasks they previously handled autonomously without noticing?

---

### S6R — Driven Overuse (Pressure)

**What it looks like:**
- The person uses AI for everything, but with an efficiency framing, not an excitement framing.
- They describe AI as something they "have to" use to stay competitive or meet targets.
- Their AI use tracks their productivity targets — more use when targets are high or tracked, less when not.
- They switch goals frequently: the AI efficiency goal is crowding out the original work goal.

**Key question to surface it:** "If performance metrics stopped tracking AI use tomorrow, how would your usage change?"
An S6R person will often admit it would drop significantly, or reveal that they find the current pace unsustainable.

**What to watch:** goal-switching frequency. Is the person's stated goal for their work shifting toward AI-efficiency rather than the original craft or output goal? Also: track usage against productivity reporting cycles — if usage spikes before reviews, S6R is likely.

---

### S6S — Social Overuse

**What it looks like:**
- Adoption closely tracks team or peer adoption. When the team goes heavy on AI, so do they; when a respected colleague backs off, so do they.
- They can't articulate a personal case for their level of AI use — they describe what their team is doing.
- They express discomfort or anxiety about being seen as "behind" rather than about the work itself.

**Key question to surface it:** "What would you do with AI if you were working on this entirely alone, with no one watching?"
An S6S person's hypothetical answer will often differ significantly from their observed behavior.

**What to watch:** whether individual adoption tracks team adoption or individual usage patterns. If a team change (new colleague, new manager) changes the person's AI use immediately, normative social influence is the driver.

---

## General S6 observation principles

1. **Volume alone does not distinguish.** All four S6 states can produce similar usage volume. The driver is what differs.
2. **Ask about affect, not behavior.** "How do you feel about your AI use right now?" surfaces the emotional register (energized, anxious, driven, compliant) faster than observing behavior.
3. **Look for what would change the behavior.** Remove the variable reward (S6E), remove the productivity tracking (S6R), change the social context (S6S), rebuild independent judgment (S6S). If removing that thing would change the behavior, you have identified the driver.
4. **S6S is the hardest to observe because the person is least likely to report it.** They will not say "I no longer trust my own judgment." They will say "AI is just faster." Watch for the anxiety underneath.

---

## Distinguishing S3B Bargaining from S7M Maturity in practice

Both look like "uses AI for some things, not others" in a single conversation.

**S3B signal:** ask about a domain they have walled off. Then describe a hypothetical model release that gets noticeably better at that domain. Watch the reaction. If the boundary moves quickly under the hypothetical without the person testing it first — S3B is likely.

**S7M signal:** the same person will say "I'd need to test that before changing how I use it." The boundary is held on evidence, not on identity.

The cleaner observation: ask which tasks they *won't* delegate to AI and why. If the reason maps to their professional identity domain ("that's my core craft"), the boundary is identity-drawn. If the reason maps to AI's reliability ("it hallucinates too much in this context"), the boundary is competence-drawn.

---

## Distinguishing S2T Trust Evaluation from S2D Defensive Resistance

Both look like careful AI evaluation.

**S2T signal:** the person updates their view based on both positive and negative AI outputs. They can tell you times AI impressed them *and* times it failed. Their stated view of AI has moved since they started testing.

**S2D signal:** the person focuses on failures. When you mention a capability, they know an exception to it. When AI succeeds, they attribute it to their prompting skill or to a low-stakes task. Their stated view of AI has not moved despite significant testing.

The cleanest probe: "Tell me about a time AI did something that made you reconsider your view." An S2T person will have an answer. An S2D person will either not have one or will describe something that confirmed their negative view.

---

## Observation limits

These heuristics are conversation starters, not diagnostic tools. Most real cases are mixed. Use the observation guide to orient a conversation, not to classify someone.

Self-report is contaminated once someone has read the model. If they know what state they are supposed to be in, they will report it. Behavioral observation over multiple weeks is more reliable than a single conversation.
```

---

## Item 17 — Per-state description additions from 1-Answers

The following additions come from 1-Answers-Model5.md sections K (state descriptions), F.6 (state validity), and G (predictability). These are not full rewrites — they are additions to existing state descriptions.

### S3B Bargaining

Add to the "healthiness" section of `states/S3B-bargaining.md`:

> S3B Bargaining is a sustainable state. Many people remain productively in S3B Bargaining for years. It is not a failure and should not be treated as a stage that must be exited. The appropriate framing for a practitioner is "this person has found a workable equilibrium" rather than "this person is stuck."

Add to the validity note (or limits-of-operationalization):

> S3B Bargaining and S7M Maturity are observationally similar in a single conversation but earn their distinction through different mechanism explanations (dissonance reduction by scope limitation versus metacognitive calibration), different behavioral predictions under capability jumps, and different upstream paths. The distinction is valid even though it requires longitudinal observation to confirm.

### S3E Ego Shock

Add to the observation markers section:

> S3E Ego Shock is present as a passage state in most high-stakes people. As a long-term residence it is harmful. Practitioners should look for whether the person is moving through it (transitioning toward S3B Bargaining or S5 Understanding within weeks to months) or staying (identity disruption unresolved after six or more months in the same domain). Sustained S3E Ego Shock warrants a referral consideration — it is within the range of clinical distress, not ordinary adaptation discomfort.

### S6S Dependent Overuse

Add to the healthiness section:

> S6S Dependent Overuse is corrosive when sustained. The mechanism is self-reinforcing: each AI output that succeeds silently confirms the person's own contribution was unnecessary, which further reduces self-trust. Early signals — the person stops attempting tasks without AI involvement, declines to review AI output against their own judgment — are worth responding to before the erosion is substantial.

### S7M Maturity

Add:

> S7M Maturity is the model's cleanest sustainable state. The person has a working internal map of where AI fails and routes work around those failures. Note the assumption built into this state: it requires viable AI-collaborative work to remain in the person's domain. S7M Maturity is not available to someone whose economic position has been eliminated by AI. See `states/S3X-structural-displacement.md`.

### S7V Evangelism

Add to the origins section (from slice 04):

> A note on sustainability: S7V Evangelism is sustainable-with-cost. The external orientation — helping others through what you yourself have navigated — draws on generativity (the drive to invest in others' growth) which is self-sustaining for many people. But sustained advocacy is high-effort. The path to S7B Burnout is real from S7V, especially when external demand exceeds personal capacity or when the audience is hostile. Watch for energy decline and rising cynicism.

---

## Item 14g addition to states — describe, don't prescribe marker

In the healthiness section of every S6 state, add one sentence:

> The model describes how people arrive in this state and how they tend to leave it. It does not prescribe that this state must be exited quickly. Whether and how quickly to support a transition is a practitioner judgment, not a model requirement.

---

## Verification checklist

- [ ] S3E Ego Shock file has no "grief," "grieving," or "loss" language.
- [ ] `observation-guide.md` exists with S6E, S6S, S6R, S6S guide sections.
- [ ] `observation-guide.md` includes the S3B vs S7M and S2T vs S2D sections.
- [ ] S3B Bargaining, S3E Ego Shock, S6S Dependent Overuse, S7M Maturity, S7V Evangelism have the additions above.
- [ ] Every S6 state has the "describes, does not prescribe" sentence in healthiness.
- [ ] S7M Maturity has the viable-domain assumption note.
