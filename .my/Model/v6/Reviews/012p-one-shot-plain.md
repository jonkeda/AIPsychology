This is a simpler rewrite of [012-one-shot.md](012-one-shot.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Review L — One-Shot "Make It Better" Review

## TL;DR

- **Proposed change:** Collapse the four S6 Overuse states (Enthusiastic, Dependent, Driven, Social) into a single **S6 Overuse state** with four separate "why are you doing this" attributes. Separately, collapse S7M, S7I, and S7E into a single **S7 Integration state** that can carry multiple styles at once. Keep S7B Burnout and S7V Evangelism as their own states.
- **Why:** Eight states in the model right now can't be told apart from observable behavior. The model's own observation guide admits this. Reorganizing them as attributes removes the false complexity without losing any of the psychological content.
- **Outcome:** State count drops from 18 to 14. Practitioner guidance becomes workable. The distinction between "state" (what someone is doing) and "driver" (why they are doing it) becomes clear.

---

## 1. Collapse S6 and S7 — the most impactful fix

The model's biggest source of fake complexity is in S6 and S7. These aren't properly defined states. They are different causes of the same behavior, or dimensions that coexist, labeled as if they were separate places a person could be.

### The S6 problem

S6E (Enthusiastic), S6D (Dependent), S6R (Driven), and S6S (Social) all describe exactly the same observable behavior: high AI usage across many tasks. The only difference is *why* the person is doing it:

- **S6E Enthusiastic:** the outputs are unpredictably good, which is rewarding the same way slot machines are. You keep pulling the handle because sometimes it pays off.
- **S6D Dependent:** the person's belief in their own ability has slowly transferred to the AI. They now trust the AI more than they trust themselves.
- **S6R Driven:** chasing productivity metrics overrides the original purpose of the work. Efficiency pressure took over.
- **S6S Social:** peers adopted AI, so this person did too. Conformity, not conviction.

The model's own observation guide says it plainly: *"Volume alone does not distinguish. All four S6 states can produce similar usage volume. The driver is what differs."* If you can't tell the states apart by watching someone, they are not states in any useful sense. They are causes.

The practical consequence: if you're trying to figure out which S6 state someone is in from a conversation or brief observation, you can't. The guide says each one requires weeks of observation and specific contextual knowledge (Is there a leaderboard? Did their team adopt AI? Did they see a demo?). Meanwhile, every intervention the model suggests depends on knowing which cause is active — and you cannot know that from a single observation.

**Fix:** Replace S6E, S6D, S6R, and S6S with a single **S6 Overuse** state that carries one or more **driver attributes**: Reward-Driven, Anxiety-Driven, Efficiency-Driven, Social-Driven. Observation guidance stays the same — you still look for the driver signal. The state is now one box, not four.

### The S7 problem

S7M (Mastery), S7I (Identity Expansion), and S7E (Ethical Integration) are listed as separate states, but the state-graph rules say they can coexist indefinitely without any transition:

- S7M + S7E together: the reflective practitioner
- S7I + S7V Evangelism (the promoter state) together: the creative leader
- S7M + S7V together: the steady mentor
- S7I + S7E together: the creator wrestling with what they are building

If three states can coexist without any of them transitioning to or from the others, they are not states. They are **dimensions** — independent things that can be true about a person at the same time. You don't transition from "reflective" to "ethically-integrated"; you can be both at once, all week, without anything changing state.

The model is forced to claim S7M, S7I, and S7E are separate, then immediately admit they coexist, then list transition rules that don't actually apply when they coexist. It contradicts itself.

What these three really are:

- **Mastery-Focused (S7M):** "I know when to use AI and when not to." Accurate self-knowledge about the tool's limits and your own.
- **Identity-Expanding (S7I):** "AI extends what I can be." The person's sense of their own capabilities now includes what they can do with AI as a partner.
- **Ethically-Integrated (S7E):** values, consent, and output attribution are part of how this person thinks about their work, not afterthoughts bolted on later.

A person can be all three at once. These are styles of integration, not stops on a road.

S7B Burnout and S7V Evangelism are genuinely different — they are transitions with distinct causes and observable behaviors. Keep them as separate states.

**Fix:** Restructure as:

1. **S6 Overuse** (one state, four driver attributes). Transitions: → S7 Integration when the driver runs dry or fails, → S7B Burnout when sustained cost exceeds value.
2. **S7 Integration** (one state, three coexisting calibration attributes: Mastery-Focused, Identity-Expanding, Ethically-Integrated). A person may carry any combination. Transitions: → S3E Ego Shock (regression when a capability jump destabilizes them), → S7B Burnout, → Dropout.
3. **S7B Burnout** and **S7V Evangelism:** unchanged as distinct end states.

All the psychological content, observation guidance, and transition rules survive this reorganization. What is removed is the false claim that there are eight separate states when there is really one state with four causes and one state with three styles.

### Why this fix beats the alternatives

- Removing PEN (discussed in Runners-up below) eliminates 1 state. This fix eliminates 8.
- Fixing the S2T/S2D fork contradiction (also below) fixes 2 states. This fixes 8.
- Adding numerical dwell-time guidance (also below) is future infrastructure. This fix addresses a structural flaw breaking the current model today.

---

## Runners-up

1. **Remove or demote PEN** — PEN is a state meant to capture people who resist AI on values-based grounds, as distinct from S2D Defensive Resistance (where someone resists AI because it threatens their sense of competence). The observation guide admits "most real cases are mixed" and lists three signals for telling PEN from S2D apart — all of which only show up across multiple observations over time, not from a single conversation. If you cannot reliably distinguish PEN from S2D in practice, PEN does not earn its place as a separate state.

   **Fix:** Remove PEN as a standalone state. Keep the values-grounded distinction as a sub-type or a note inside the S2D file.

2. **Fix the S2T / S2D fork framing contradiction** — The state graph says S2T (Trust Evaluation, where someone evaluates AI fairly) and S2D (Defensive Resistance, where someone evaluates AI defensively) are "responses to S1, with no implied order." But there is now a new edge in the graph: S2T → S2D, triggered when the person discovers higher stakes during testing. That edge *does* imply an order. The model needs to commit: either these are genuinely parallel with no path between them (remove the edge, and say S2T people can regress to S2D if stakes get high enough), or S2T is the default low-stakes entry and S2D is what happens when someone realizes the stakes are higher than they thought (drop the "no implied order" language and be explicit about it).

   **Fix:** Pick one framing and make it consistent throughout the state graph and observation guide.

3. **Clarify how the Delegation Ceiling relates to states** — The Delegation Ceiling is a cap on how much of your work you're willing to hand off to AI. It is described as "independent of state." But the healthiness file says the ceiling "changes through sustained skill-building" and "readiness work" — both of which are state-dependent processes. That's a contradiction. Spell out: does the ceiling change when someone reaches S7M (Mastery)? Does it reset if they regress to S3E (Ego Shock, the destabilized panic state)? Can coaching during S3B Bargaining lower the ceiling by making high-delegation work feel safer, or can coaching only raise the ceiling?

   **Fix:** Add a paragraph to the Delegation Ceiling definition that explains exactly how ceiling changes relate to state transitions and regressions.

4. **Add dwell-time numbers** — The model is silent on how long someone typically stays in S3E (Ego Shock), S6 (Overuse), or S7B (Burnout). "This state can persist" is not useful for a practitioner. They need to know: is three weeks in S3E normal, or is that a sign something is stuck? Should someone still in S7B after three months trigger an intervention? Add rough ranges based on whatever evidence is available, even if that evidence is thin. A rough estimate flagged as low-confidence is more useful than nothing.

   **Fix:** Add dwell-time estimates (even rough ones, with a low-confidence note) to the S3E, S6, and S7B state files.
