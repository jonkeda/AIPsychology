# Comparative Review — Plain-Language Version

This is a simpler rewrite of [008-comparative.md](008-comparative.md). Same findings, plain language. If you've read the original and it landed, skip this one.

## What this review is doing

V5 is the model in this repo. There are older models in psychology and tech adoption that try to explain similar things — how people react to a new technology, how they change behavior, when they get stuck. This review walks through each older model and asks: did V5 borrow it, improve it, or invent something new?

## TL;DR

- V5 adds something the older tech-adoption models miss: what happens when the new tech threatens your sense of who you are. That's a real addition.
- V4 used to compare AI adoption to grief (denial, anger, bargaining, and so on). V5 dropped that. Good. Grief is about permanent loss; AI threat isn't permanent and isn't loss.
- V5's two-axis idea — how much your identity is on the line, crossed with how much you're handing over to AI — is genuinely new. No older model does this.
- V5 splits "people who use AI too much" into four different kinds with four different causes. Also new. They need different fixes.
- V5's test for *why* someone quit AI (offer them a fix, see if they come back) is original and you can actually run it.
- V5 admits that 40% of its claims are still guesses, but hides this admission at the end. Move it to the front.

## Findings

### 1. Grief stages (Kübler-Ross: denial, anger, bargaining, depression, acceptance)

V5 dropped the grief framing. Right call.

Grief is about accepting that something is gone forever. AI threatening your job isn't that. It can be reframed, reversed, or worked around. V5's S3 Ego Shock (the panic state) is a single sharp identity-disruption moment with multiple ways out, not a fixed sequence of emotions you march through.

Also worth knowing: the grief-stages idea has been **out of favor in actual bereavement research** for years. Researchers like Bonanno and Prigerson have shown most people don't go through fixed stages even for real grief. So V5 isn't just dropping a bad fit, it's dropping a model that's already been weakened in its own field. Keep the rejection.

### 2. Technology Acceptance Model — TAM (Davis, 1989: people adopt tech based on how useful and how easy they think it is)

V5's S2T Trust Evaluation state (where someone calmly evaluates whether AI is useful) is basically TAM with different labels.

But V5 adds something TAM doesn't have. In S2T Trust Evaluation, the person weighs the evidence fairly. In S2D Defensive Resistance (defensive evaluation), the same person discounts anything good about AI and zeroes in on anything bad. That's a **different mental process** — it's identity-defense, not utility-evaluation. TAM has no story for why the same person evaluates the same evidence differently depending on whether their identity is on the line.

For low-stakes tools (picking an email client), TAM works fine and V5 is overkill. For high-stakes tools (AI doing your core job), V5's addition is necessary.

### 3. Diffusion of Innovations (Rogers: people adopt new tech based on how well it fits their existing way of doing things)

V5's S5 Understanding (the integrated, settled state) borrows Rogers' idea about fit. V5 splits "stable" into two pieces: *internal* (your mental model is coherent) and *social* (the people around you treat AI use as normal). That split is useful.

But Rogers' original framework has five factors — relative advantage, compatibility, complexity, observability, trialability — that are more detailed and easier to test than V5's "did they reach S5 Understanding or not." V5 should **say out loud that S5 Understanding is a coarser version of Rogers**, not an improvement on him. Right now Rogers gets one parenthetical mention and that's not honest.

### 4. Transtheoretical Model — TTM (Prochaska and DiClemente: behavior change moves through stages — not yet thinking about it, thinking about it, preparing, acting, maintaining — with relapses)

V5 doesn't cite TTM, but the shape is there: not-yet-encountered (S0 Baseline) → first encounter (S1 Initial Encounter) → evaluating (S2T Trust Evaluation or S2D Defensive Resistance) → using (S5 Understanding or S6) → settled (S7) with the ability to fall back.

TTM has something V5 doesn't: a list of 10–21 specific techniques for **moving** someone from one stage to the next. V5 only describes states. It says nothing about how to push someone from S2D Defensive Resistance (defensive) toward S5 Understanding (integrated).

In software-engineer terms: V5 is a state diagram. TTM is a state diagram **plus** the control logic for moving between states.

### 5. Gartner Hype Cycle (the famous curve: trigger → peak of hype → trough of disappointment → plateau of real productivity)

You can map V5 to the curve: S1 Initial Encounter (trigger) → S6A Enthusiastic Overuse (enthusiastic overuse / peak hype) → S7D Burnout (burnout or dropout / trough) → S7A Maturity (mature use / plateau).

But V5 rightly says this curve isn't universal. Some people skip the hype peak entirely. Some go straight from S1 Initial Encounter to S5 Understanding with no trough. S6 actually has four parallel attractors, not one peak. V5 treats Gartner as **one possible path**, not the path everyone takes.

### 6. Identity Stakes × Task Delegation modulation

This is **genuinely new**.

V5 says: every state feels different depending on two dials.
- **Identity Stakes** — how much of your sense of self is on the line (low = AI is doing my expense report; high = AI is doing the work I'm proud of being good at).
- **Task Delegation (D1 to D4)** — how much authority you've handed over (D1 = AI looks things up for me; D4 = AI makes decisions on my behalf).

No older model does this cross-cut. Grief stages vary by how big the loss is, but not by what kind of threat it is. TAM varies by perceived usefulness, but not by identity threat. Rogers varies by innovation features, but not by which capability is threatened. TTM varies by readiness, but not by stakes.

V5's claim: the same state (such as S3 Ego Shock) feels mildly surprising at low stakes / D1 and existential at high stakes / D4. That's a useful insight.

Catch: V5 doesn't say how the two dials combine. V4 had a formula for it. V5 dropped the formula because "the multipliers have no defined units" — that's honest, but it's also a dodge. A real model would specify how to combine them in a way you could measure.

### 7. Four-way split of S6 (overuse) with different causes

This is **genuinely new**.

V5 splits "person uses AI a lot" into four different states with four different drivers:
- **S6A Enthusiastic Overuse** — driven by hits of dopamine from unpredictable rewards (the slot-machine effect).
- **S6B Dependent Overuse** — driven by losing confidence in your own ability and leaning on AI to compensate.
- **S6C Driven Overuse** — driven by mistaking efficiency itself for the goal (you start optimizing speed for its own sake instead of caring about the work).
- **S6D Social Overuse** — driven by everyone else doing it (peer pressure, social conformity).

No older model says "the same surface behavior — heavy AI use — can come from four different mechanisms." Two people using AI heavily are not in the same state and don't need the same intervention. One needs hedonic rebalancing (dialing down the dopamine loop). Another needs to rebuild confidence. Another needs to remember what the work was actually for. Another needs to feel safe disagreeing with their team.

Catch: V5 doesn't say how to **tell them apart in real life**. How would you spot variable-reward overuse versus goal-substitution overuse just by looking at someone's usage logs?

### 8. The dropout plane (practical severity × emotional severity) with a reversibility test

This is **genuinely new and the most testable thing in V5**.

Older research treats dropout as one thing. V5 says it has two dimensions:
- **Practical severity** (0–10): the tool didn't actually do the job.
- **Emotional severity** (0–10): using the tool made the person feel bad.

The reversibility test: give the dropout a tool that fixes their stated complaint. If they come back, practical severity was the real driver. If they don't, the issue was emotional.

No older model decomposes dropout this way.

Catch: the test assumes the person told the truth about *why* they quit. If practical severity was actually high but the person quit while saving face ("I just don't like AI"), the test points the wrong direction.

### 9. The "Limits of Operationalization" section (the part where V5 admits what's still a guess)

V5 is **honest, but undermines its own authority** by admitting that 40% of its claims are conjecture.

Older models hid this. Kübler-Ross never said her stages were anecdotal. TAM doesn't flag that "perceived usefulness" is hard to measure. V5 says it out loud. That's rare and right.

But the placement is wrong. The admission is buried at the end, and the individual states never repeat the warning. If S7F Evangelism's claim about needing prior S3 Ego Shock is a guess, the S7F Evangelism write-up itself should say so. By the time the reader reaches the Limits section at the end, they've forgotten which claims were marked solid and which were marked speculative.

## Recommendations

1. **Cite TAM, Rogers, TTM, and Gartner by name in the mechanism anchors.** Stop hiding the borrowings in parentheticals. Say "borrows from X" or "extends X by Y."

2. **Lead with the Identity Stakes × Task Delegation modulation as the headline new contribution.** Put it before the state descriptions so readers know upfront what's actually new.

3. **Spell out how to detect each kind of S6 in real life.** Add an "Observation guide" under S6 with concrete behavioral markers. For S6A Enthusiastic Overuse, look at whether usage spikes line up with reward timing. For S6B Dependent Overuse, watch self-reported confidence drop over time. For S6C Driven Overuse, count goal-switching frequency. For S6D Social Overuse, check whether someone's adoption tracks their team's adoption.

4. **Run the reversibility test as an actual study.** Recruit dropouts, offer them a tool-fix, see who returns, correlate with their stated emotional distress.

5. **Move the "Limits of operationalization" warning to the front.** Add inline footnotes or callouts under each unproven claim saying "conjecture: awaiting longitudinal data." Replace the end section with a one-line summary.

6. **Frame V5 as an extension of the older models, not a replacement.** Add a one-paragraph "Relationship to Prior Frameworks" section before the state map.

7. **Strip out remaining grief language entirely.** No more "grief," "grieving," or "loss" anywhere in S3 Ego Shock. Use "identity disruption," "self-efficacy confrontation," or "existential discomfort."

8. **Say out loud that V5 describes paths, it doesn't prescribe them.** One sentence: "This model describes observed paths, not recommended paths. Don't use it to push people through transitions; use it to figure out where someone is."

9. **Keep the state-machine structure.** The directed graph with regression arrows is V5's strongest contribution. Moving from fixed stages to states with flexible transitions was the right move.

10. **Drop the comparison table; fold it into the narrative.** The table breaks the flow. The findings above already cover the comparisons. Keep the table only as a lookup reference if readers ask for one.
