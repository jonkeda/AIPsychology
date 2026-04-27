This is a simpler rewrite of [010-v4-v5-diff.md](010-v4-v5-diff.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# What Changed From V4 to V5 — Plain-Language Version

This review walks through every meaningful change between V4 and V5 of the model, and judges whether each change made the model better, worse, or just different.

## TL;DR

- **Mechanism anchors added.** Each state in the model is now tied to a known idea from psychology (such as "novelty appraisal" or "self-efficacy collapse"). This helps explain *why* a state behaves the way it does. Some of the anchors are still guesses, not proven facts.
- **States renamed.** S1 Initial Encounter.5 became S2T Trust Evaluation and S2 became S2D Defensive Resistance. Cleaner labels. The downside: anything written about V4 now uses outdated names.
- **The fake formula is gone.** V4 had "intensity = baseline × Stakes × Delegation," which looked like math but had no units and could not be measured. V5 deleted it. Honest move. It does not fix the underlying problem of how to measure intensity.
- **The S3B Bargaining versus S7A Maturity test got weaker.** V4 called this distinction "falsifiable" (you could prove it wrong). V5 backed down and called it a "heuristic" (a rule of thumb). Honest, but a step backward in testability.
- **Dropout is now two sliders instead of two buckets.** Practical severity 0–10 and emotional severity 0–10. Better. V5 also adds a "reversibility test": fix their cited problem and see if they come back.
- **New "limits of operationalization" section.** V5 sorts every claim into: things you can see right now, things you can only see over time, things you only know from interviews, and pure guesses. Honesty win. Also exposes how little of the model is actually testable today.
- **Conjecture tags everywhere.** Several big claims are now stamped "we are guessing": S5 Understanding needs both internal and social acceptance; stable evangelists must have suffered first; most people cycle through the model more than once; the whole Cultural Variability section.
- **Adoption Ceiling deleted.** Was an optional feature in V4, never used. Gone in V5. No loss.
- V5 is mostly a defensiveness pass. It strips off V4's pseudo-scientific veneer and is more honest. The mechanism anchors add real explanatory power *if they hold up*. V5 does not solve the empirical problems — it admits them.

## Findings

### 1. Each state is now tied to a known psychology idea

**What changed:** V5 attaches an established psychological mechanism to each state. For example:

- S1 Initial Encounter → novelty appraisal (how the brain decides whether something new is a threat or an opportunity).
- S2T Trust Evaluation → calibration under uncertainty plus the Technology Acceptance Model (the standard framework for predicting whether someone will adopt a tool).
- S3 Ego Shock → self-efficacy collapse (the feeling of *I'm not good at my job anymore*) plus terror-management threat response (how people react when reminded their identity might not last).
- S3B Bargaining → cognitive-dissonance reduction (the brain papering over a contradiction in what you believe).
- S5 Understanding → schema integration plus diffusion theory (how new ideas spread and settle into people's mental models).
- S6A Enthusiastic Overuse → variable-reward reinforcement (the slot-machine effect).
- S6B Dependent Overuse → self-efficacy displacement (losing trust in your own judgment because you keep deferring to the tool).
- S6C Driven Overuse → goal-substitution (chasing the tool's goal instead of your own).
- S6D Social Overuse → normative social influence (the Asch conformity studies — going along with the group).
- S7A Maturity → metacognitive calibration (knowing what you know and what you don't).
- S7B Identity Expansion → extended-self incorporation (you start to think of the tool as part of you).
- S7C Ethical Integration → meaning-making.
- S7D Burnout → resource depletion.
- S7F Evangelism → generativity (Erikson's stage about helping the next generation, broadened to mentoring others through the AI shift).

**Why:** V5 says outright that the V4 model was just description, no explanation. Adding mechanisms changes that. Now you can say not just "this person is in S3 Ego Shock" but "they're in S3 Ego Shock because their sense of competence collapsed."

**Did it work:** Partly. The mechanisms are real — they all come from real research. The problem is they explain too much. S3 Ego Shock is anchored to self-efficacy collapse and terror-management. But the model never says why one person's self-efficacy collapse leads to S3 Ego Shock (panic) and another's leads to S3B Bargaining (a bargain). The mechanisms raise the bar on what the model is claiming without saying how the mechanisms interact. Some are educated guesses dressed as anchors (see finding 7).

**Fix:** Keep the mechanisms but attach a testable prediction to each one. "If S3 Ego Shock is mainly self-efficacy collapse, then we should see [specific observable thing]." Without that, the mechanism is decoration.

### 2. S1 Initial Encounter.5 became S2T Trust Evaluation, and S2 became S2D Defensive Resistance

**What changed:** V4 called these states S1 Initial Encounter.5 (Trust Evaluation) and S2 (Defensive Resistance). The `.5` made it sound like S1 Initial Encounter.5 sat between S1 Initial Encounter and S2 in time. It doesn't. Both are reactions to S1 Initial Encounter, just different ones. V5 renamed them S2T Trust Evaluation and S2D Defensive Resistance — same leading number, with a letter telling you which response.

**Why:** Get rid of the false impression of ordering.

**Did it work:** Yes, but at a cost. S2T Trust Evaluation and S2D Defensive Resistance are clearer than S1 Initial Encounter.5 and S2. Anything written about V4 now points at names that don't exist. And out loud, "S2 versus S2T Trust Evaluation" can sound the same. Net positive but real cost.

**Fix:** The introduction should say plainly: "If you used V4, S2T Trust Evaluation is the old S1 Initial Encounter.5, S2D Defensive Resistance is the old S2, and there is no plain S2 anymore."

### 3. The fake formula is deleted

**What changed:** V4 had: "Emotional intensity in any state = baseline × Identity Stakes × Task Delegation Level." V5 removed it and replaced it with a simple table under S3 Ego Shock.

**Why:** The formula had no units. What is "baseline"? Multiplied by what scale? V5 correctly calls this pseudo-math.

**Did it work:** Yes. The qualitative table ("Low identity stakes × D1 delegation = mild surprise; High × D4 = existential dread") is more honest. The cost is that the model can no longer claim to predict intensity precisely. That's the right concession.

**Fix:** Keep deleted. The model should now state plainly whether intensity is thought to add up, multiply, neither, or unknown.

### 4. The S3B Bargaining versus S7A Maturity test got demoted

**What changed:** V4 said S3B Bargaining and S7A Maturity look the same from the outside but offered a "falsifiable" way to tell them apart. V5 keeps the same idea but downgrades it to "heuristic" — a rule of thumb. V5 also notes the test is contaminated once a subject has read this model (because then they know what answer is "good").

**Why:** V4 oversold it. The test (watch what someone does after a new AI release comes out) is not really falsifiable. Whatever the person does, you can rationalize it as either "they bowed to pressure" or "they updated based on evidence."

**Did it work:** Honest, but a step back. Calling it a heuristic is more accurate. A better fix would have been to propose a different, actually-testable version: look at the *timing*. If someone's boundary shifted within a few weeks of a model release with no real testing, S3B Bargaining is more likely. If it only shifted after they ran the new model through their own work, S7A Maturity.

**Fix:** Replace the heuristic with a specific interview question, such as: "Walk me through the last time you decided to expand what you use AI for. Was it because the tool became capable of something new, or because you couldn't keep the boundary in place anymore?"

### 5. Dropout is now two sliders, plus a reversibility test

**What changed:** V4 split dropout into two buckets: emotional versus practical. V5 replaced the buckets with two sliders, each 0–10. A real dropout has a score on both. V5 also adds the reversibility check: give the dropout a tool that genuinely solves the problem they cited. If they restart, practical was the main driver. If they don't, emotional was.

**Why:** Real dropouts often have both. Buckets force you to pick one and lose information. The reversibility test shifts the question from "ask them" (unreliable) to "do something and see what happens" (more reliable).

**Did it work:** Yes for the two sliders. Partly for the reversibility test. The sliders handle common cases (high practical and high emotional at the same time). The test has limits: someone who quit emotionally might refuse the new tool because the same identity threat is still there — the test reads "emotional" but didn't really measure practical severity. The test also assumes the "fix" is what the person actually needed.

**Fix:** Keep both. Describe the reversibility test as "tends to work" rather than "always works."

### 6. New "limits of operationalization" section

**What changed:** V5 sorts every claim into one of four categories: things you can see in a snapshot, things you can only see over months, things you can only get from interviews, and pure guesses.

**Why:** V5 wants to head off readers who think the model is more proven than it is.

**Did it work:** Yes. The section is honest and useful. It draws a clear line between "we have evidence" and "we are guessing."

**Fix:** Keep and expand. For each long-term-only or interview-only claim, write down a specific protocol that would actually test it.

### 7. "Conjecture" tags on the big unproven claims

**What changed:** V5 marks four major claims as guesses: S5 Understanding stability needs both internal acceptance and social acceptance; S7F Evangelism (stable evangelist) is unstable without prior S3 Ego Shock (panic); most people cycle through the model more than once; the whole Cultural Variability section.

**Why:** These claims are useful as scaffolding but no one has actually checked them. V5 separates "we have evidence" from "we suspect."

**Did it work:** Partly. Marking something as a guess is honest, but it's not the same as fixing it. Half the model's biggest claims are now stamped "unverified." A reader doesn't know whether to design around these claims or treat them as placeholders.

**Fix:** Keep the tags but add guidance: "A conjecture is a working hypothesis, not a fact. If you build something on top of one, explicitly test whether the predicted thing actually happens. Write down any cases where the conjecture failed."

### 8. Adoption Ceiling is gone

**What changed:** V4 had Adoption Ceiling as an optional add-on — the idea that someone could be mature about AI at low stakes (like using it to write emails) but in panic at high stakes (using it for their core creative work). V5 cut it.

**Why:** It was never formalized in V4 and never used. Removing it cleans up the model.

**Did it work:** Yes for clarity, but the underlying problem is still there. People really do behave this way: calm with low-stakes AI, defensive with high-stakes AI. V5 removed the feature without proposing a replacement. Cleaner model, less precision on a common real-world case.

**Fix:** Keep removed; address the gap in the recommendations below.

### 9. The lightning-bolt rule is applied unevenly

V5 says: "A state gets a ⚡ if and only if at least one named external event materially changes the chance of entering or leaving that state." Then V5 applies the rule inconsistently. S2T Trust Evaluation has no ⚡ (called "internally driven"), but the model also says S2T Trust Evaluation can be re-triggered from S5 Understanding when a new model comes out — which is exactly an external event. Meanwhile S1 Initial Encounter has ⚡, and S5 Understanding doesn't, even though S5 Understanding is the very state people try to stay in and external events are usually what knocks them out.

### 10. Cultural Variability has no mechanism anchors

V5 admits Cultural Variability is a guess but still makes specific claims, such as "high craft-identity cultures amplify S2D Defensive Resistance, S3 Ego Shock, and S3B Bargaining." It doesn't say *why* a craft identity amplifies S2D Defensive Resistance. Are these people more likely to enter S2D Defensive Resistance in the first place, do they experience S2D Defensive Resistance more intensely, or do they stay there longer? Without a mechanism, the claim isn't testable.

### 11. No way out of S6B Dependent Overuse is described

S6B Dependent Overuse is the state where someone has lost confidence in their own judgment because they've been outsourcing decisions to AI. They start checking AI's answers against other AI's answers. The model only lists two exits: regression to S3 Ego Shock (panic) or onward to S7D Burnout (burnout). Both are painful. There is a third plausible exit — rebuild self-efficacy by deliberately doing low-stakes work without AI for a while — but the model doesn't describe it.

## Recommendations

1. **Turn the unfalsifiable guesses into real experiments, or drop them.** The model's credibility depends on being clear about what it knows versus what it suspects. Three claims are particularly hopeless as written:
   - **S5 Understanding needs both internal reframing and social normalization.** As written, "any discomfort can be blamed on a mismatch between the two" makes the claim impossible to disprove. Either propose a way to measure the two pieces separately, or drop the dual-component framing.
   - **Stable S7F Evangelism requires prior S3 Ego Shock.** If no one has actually observed someone in stable S7F Evangelism who didn't go through S3 Ego Shock first, what's the evidence? Right now it's pure speculation.
   - **Most people cycle more than once.** As a vibe, this is unfalsifiable. Either propose a measurement (such as "the median person re-enters S3 Ego Shock at least twice over five years") or remove the claim.

   For each of these, add a paragraph: "To test this, we would [specific protocol]. It would cost [time and money]. Status: not yet done."

2. **Operationalize the S3B Bargaining versus S7A Maturity distinction, or merge them.** Either propose a real test (a structured interview, timeline analysis, or a behavioral prediction), or collapse S3B Bargaining and S7A Maturity into one "Bounded Adoption" state with sub-conditions.

3. **Add a measurement-protocol appendix in V6.** For each claim that needs long-term observation or interviews, write out the actual protocol. For example:
   - **S2T Trust Evaluation versus S2D Defensive Resistance:** "Ask: Tell me about the last time you tested an AI tool. Did you update your estimate of its capability based on what you saw, or did you find yourself dismissing the good results and focusing on the limitations?"
   - **S3B Bargaining versus S7A Maturity:** "Track boundary-movement across three model releases. Code: moved within one week of release with no testing data published = S3B Bargaining; moved only after announced benchmarks or real trials = S7A Maturity."

4. **Address the Adoption Ceiling gap.** Three options:
   - Add sub-types under S7A Maturity (S7A Maturity-D2 for people calibrated only at low delegation; S7A Maturity-D3+ for people calibrated at high delegation).
   - Add a fourth axis called "Delegation Ceiling" tracking the highest delegation level a person will use.
   - Make it explicit that one person can be in multiple states at once (S7A Maturity for low-stakes work, S3 Ego Shock for high-stakes work) and document that pattern.

5. **Expand the External Trigger layer.** Distinguish triggers that *start* a transition from triggers that *speed it up* from triggers that *reverse* it. Build a small matrix.

6. **Add rules for how mechanisms interact.** S3 Ego Shock is anchored to both self-efficacy collapse and terror-management. Which one dominates? Propose something like: "Self-efficacy collapse dominates for skilled professionals; terror-management dominates for younger or early-career users."

7. **Restate each conjecture as a hypothesis with an experimental design.** For example: "S5 Understanding stability requires both internal reframing and social normalization. Test: measure internal reframing through a pre/post interview about how their mental model holds together; measure social normalization through a peer adoption survey. Compare S5 Understanding users with both versus only one. Predict: the both group has lower dropout. Cost: a six-month study, 50 users, three rounds of interviews."
