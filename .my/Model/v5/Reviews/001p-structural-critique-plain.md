# Structural Critique — Plain-Language Version

This is a simpler rewrite of [001-structural-critique.md](001-structural-critique.md). Same findings, plain language. If you've read the original and it landed, skip this one.

## What this review is about

Model V5 is a state machine. People move between states (S1 Initial Encounter, S2T Trust Evaluation, S2D Defensive Resistance, S3 Ego Shock, S3B Bargaining, S5 Understanding, S6A Enthusiastic Overuse–D, S7A Maturity–F, and so on) as they adopt AI tools. Each state has a description, a list of transitions out, and now in V5 a **mechanism anchor** — a one-line explanation of the internal process driving the state.

This review ignores the prose and looks at the graph. Are the states well-defined? Do the transitions match what the descriptions say? Can two reviewers, looking at the same person, agree on which state that person is in?

Often, no.

## TL;DR

- The S1 Initial Encounter → S2T Trust Evaluation / S2D Defensive Resistance split is **described as a parallel fork**, but the transition rules say it's actually a **sequence with branches**. Pick one.
- S3B Bargaining and S7A Maturity are supposed to be different states, but you **can't tell them apart** by watching someone. The rule for separating them admits it's just a guess.
- The S6 states are claimed to be independent, but the model only lists two specific combinations as common. That means they're **not actually independent**.
- The state diagram is **missing an edge** the text says exists (S3 Ego Shock → S5 Understanding).
- The model says some states can overlap, but never says **which combinations are allowed** and which aren't.
- Three of the S7 states (A, B, F) describe **internal experience**, not behavior. Two reviewers watching the same person could not agree on the label.
- The model says S3 Ego Shock (panic) leads to S6B Dependent Overuse (dependent overuse) but **doesn't explain why** panic would push someone toward more AI use rather than away from it.

## Findings

1. **The S2T Trust Evaluation/S2D Defensive Resistance fork claims to be a parallel fork but describes a sequence.** The model says: how much your identity is wrapped up in your job (Identity Stakes) decides whether step S1 Initial Encounter leads to S2T Trust Evaluation (open evaluation) or S2D Defensive Resistance (defensive evaluation). But then S2T Trust Evaluation's own transition list says: "→ S2D Defensive Resistance — testing surfaces a threatening capability." So a person can start in S2T Trust Evaluation because the stakes seemed low, then run into a scary capability during testing and flip into S2D Defensive Resistance. That's a **sequence with a conditional branch**, not two independent paths. The model's prose says one thing and its transition rules say another.

2. **S3B Bargaining and S7A Maturity look the same from the outside.** Both states describe the same behavior: the person uses AI for some things but not others. The model tries to separate them like this: in S3B Bargaining, the person redraws their personal limits when a stronger model comes out; in S7A Maturity, they only redraw the limits after testing the new model. The model openly admits this rule is "a heuristic, not a measured fact" and adds that anyone who reads the model will start describing themselves as S7A Maturity regardless of what they actually do. There's no way to measure "capability pressure" versus "measured evidence" without asking the person. So the two states **cannot be told apart in practice**.

3. **The S6 states claim to be independent but only line up in specific pairs.** The model says people can be in more than one S6 state at once and lists the common pairs: S6A Enthusiastic Overuse + S6C Driven Overuse in startups, S6B Dependent Overuse + S6D Social Overuse in compliance-heavy companies. If only certain pairs occur, the states aren't independent — they have rules about which combinations work. The model doesn't say why those pairs are common while S6A Enthusiastic Overuse + S6B Dependent Overuse and S6C Driven Overuse + S6D Social Overuse are rare. And there's a real question hiding here: S6A Enthusiastic Overuse is enthusiastic and high-energy, S6B Dependent Overuse is anxious and confidence-eroded. **Can both of those be high in the same person at the same time?** The model doesn't say.

4. **The state diagram is missing an edge.** The ASCII diagram shows S3 Ego Shock going to S3B Bargaining and S3B Bargaining going to S5 Understanding. But the S3 Ego Shock description in the text says: "Transitions: → S5 Understanding — direct integration when the person can hold the full confrontation." So the text says S3 Ego Shock can go straight to S5 Understanding. The diagram doesn't show it. Text and graph disagree.

5. **Nobody specified which states can coexist.** The model says S7 states are "long-term patterns ... not mutually exclusive" and S6 states "can occupy more than one simultaneously." But it never lists the rules. Can someone be in S6A Enthusiastic Overuse (enthusiastic, reward-seeking) and S6B Dependent Overuse (dependent, low-confidence) at the same time? Can they be in S6A Enthusiastic Overuse and S7A Maturity at the same time? Without rules, anyone can theoretically be in any combination, and the model **predicts nothing**.

6. **S7A Maturity, S7B Identity Expansion, and S7F Evangelism can't be told apart from outside the person's head.** S7A Maturity is metacognitive calibration (knowing what AI is good for and what it isn't). S7B Identity Expansion is extended-self (the AI tool feels like part of how you work). S7F Evangelism is generativity (you actively help others adopt AI well). All three are about how the person experiences AI, not what they do. Two reviewers given only behavior to look at could not reliably pick the same label. How do you tell whether someone's identity *includes* the AI tool (S7B Identity Expansion) versus uses it competently as a separate thing (S7A Maturity)? You can't. **The states are defined by inner experience**, so the only way to assign them is by asking — which is exactly what the mechanism anchors were supposed to fix.

7. **The S3 Ego Shock → S6B Dependent Overuse transition has no explanation.** S6B Dependent Overuse is anchored to "self-efficacy displacement" — the person hands over their judgment to AI. The model also says S6B Dependent Overuse "inherits its trigger from the upstream S3 Ego Shock episode rather than from any current event." So someone has an identity panic (S3 Ego Shock) and then ends up over-relying on AI (S6B Dependent Overuse). But why? A panicked person could just as easily back away from AI entirely. The model **doesn't predict which way they go**, but it claims S3 Ego Shock is the cause of S6B Dependent Overuse. That's a missing causal link.

8. **S3B Bargaining is called stable, but its own transitions say it isn't.** The model claims S3B Bargaining is "not a failure state — many people remain productive here for years." But S3B Bargaining's transition list includes "→ S3 Ego Shock — capability jump shatters the bargain." If new model releases regularly knock people out of S3B Bargaining and back into panic, then S3B Bargaining is **a holding pattern, not a stable state**. Pick one: redefine S3B Bargaining as temporary coping, or explain why some people's arrangement survives across model jumps.

9. **The two axes don't compose.** The model has two axes: Identity Stakes (how much of your self is on the line) and Task Delegation (how much of the task you hand over). It says they're independent, then provides a table under S3 Ego Shock showing how they combine — Low × D1 produces mild surprise, High × D4 produces existential crisis. V4 used to have a multiplier formula. V5 removed it because "multipliers have no units." Fine, but **nothing replaced it**. So the axes look like they should combine, the table shows they do combine, and yet there's no rule for how. They're decorative.

10. **The S2T Trust Evaluation mechanism anchor is too generic.** S2T Trust Evaluation is anchored to the Technology Acceptance Model — the idea that people adopt tech based on whether they think it's useful and easy to use. But that applies to *any* tech adoption, not specifically to people evaluating AI without identity threat. What actually makes S2T Trust Evaluation distinctive is that the person tests AI without ego defense kicking in. The anchor doesn't explain the *why*. Compare with S2D Defensive Resistance, anchored to "identity-protection cognition" — that one is specific to identity threat. **S2T Trust Evaluation's anchor is doing no work.**

11. **The S7F Evangelism prerequisite is presented as a guess but used as a rule.** The model says: people who become stable AI evangelists (S7F Evangelism) are "most stable when the person has previously passed through S3 Ego Shock ... without that experience, the advocacy tends to be naive (S6A Enthusiastic Overuse flavor) or compelled (S6D Social Overuse flavor) and collapses under the first hostile question." It calls this a heuristic ("not a tested claim"). But then it uses the heuristic to **decide whether S7F Evangelism is stable or not**. Pick one: if prior S3 Ego Shock is required for S7F Evangelism, write that into the state definition. If it's just a guess, stop using it to constrain transitions.

12. **Removing Adoption Ceiling left a hole.** V5 dropped the Adoption Ceiling concept and says: "If a use case requires it, that use case justifies V6." But there's no record of what Adoption Ceiling actually was or what its removal broke. **Concrete example:** a senior engineer who has thought about AI carefully and decided to use it only for low-stakes tasks. Where does that person fit? Are they in S7A Maturity, or is there a missing state for "I have adopted AI but deliberately chosen a low ceiling on delegation"? The model doesn't say.

## Recommendations

1. **Rewrite the S2T Trust Evaluation/S2D Defensive Resistance fork as a sequence.** Update the state diagram so S1 Initial Encounter → S2T Trust Evaluation (low stakes, typical) and S1 Initial Encounter → S2D Defensive Resistance (high stakes, typical), and add the edge S2T Trust Evaluation → S2D Defensive Resistance (threat appears during testing). Rewrite S2T Trust Evaluation's description to: "Non-defensive evaluation, which can convert to defensive evaluation if testing reveals threat." Rewrite the fork description to match: low-stakes people usually enter S2T Trust Evaluation, high-stakes people usually enter S2D Defensive Resistance, and S2T Trust Evaluation can move to S2D Defensive Resistance if testing turns up something threatening.

2. **Merge S3B Bargaining and S7A Maturity, or anchor them differently.** Two options:
   - **Option A (Merge):** Combine S3B Bargaining and S7A Maturity into one "Bounded Adoption" state. Tell them apart by *how the person got there*, not by what they say their motivation is. S7A Maturity is reached from S5 Understanding, S2T Trust Evaluation, or later S6/S7 states, with limits set after testing. S3B Bargaining is reached from S3 Ego Shock, under emotional pressure, with limits redrawn downward when stronger models appear. **Transition history is observable**; motivation isn't.
   - **Option B (Re-anchor):** Keep them separate but redefine S3B Bargaining as dissonance reduction under *active emotional pressure* (the person came from S3 Ego Shock and is still managing anxiety). S7A Maturity is not under that pressure.
   - Pick Option A. The heuristic approach can't be made to work; transition history can be checked.

3. **Write down which S6 states can coexist and which can't.** Add a section after the S6 overview saying: S6A Enthusiastic Overuse (enthusiastic, high positive feeling) and S6B Dependent Overuse (dependent, high anxiety) feel incompatible to most people and rarely happen together. S6C Driven Overuse and S6D Social Overuse can coexist in high-pressure cultures where being productive *is* the conformity. So S6A Enthusiastic Overuse + S6C Driven Overuse and S6B Dependent Overuse + S6D Social Overuse are stable; S6A Enthusiastic Overuse + S6B Dependent Overuse and S6C Driven Overuse + S6D Social Overuse aren't. Add similar rules for combinations with S7 states.

4. **Add the S3 Ego Shock → S5 Understanding edge to the diagram.** Update the ASCII diagram with a direct line from S3 Ego Shock to S5 Understanding (not only via S3B Bargaining). Add the condition: "S3 Ego Shock → S5 Understanding (rare; requires the person to face the identity threat directly without defense or compromise and rebuild self-concept on the spot)."

5. **Add a "State Occupancy" section** with explicit rules:

```
**S6 states (parallel, with constraints):**
- S6A Enthusiastic Overuse and S6B Dependent Overuse are mutually exclusive (opposite affect/motivation patterns).
- S6C Driven Overuse and S6D Social Overuse can coexist (productivity and conformity reinforce each other in cultures that value both).

**S7 states (parallel, intentionally overlapping):**
- Any S7 state can coexist with any other S7 state.

**S6 and S7 coexistence:**
- S6A Enthusiastic Overuse (enthusiastic overuse) can transition to S7A Maturity or S7B Identity Expansion but not coexist with either.
- S6B Dependent Overuse, S6C Driven Overuse, S6D Social Overuse all lead to S7D Burnout (burnout) as primary exit.

**Dropout reachable from every state.**
```
