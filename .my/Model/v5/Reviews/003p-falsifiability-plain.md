# Falsifiability and Predictive Power — Plain-Language Version

This is a simpler rewrite of [003-falsifiability.md](003-falsifiability.md). Same findings, shorter words, more examples. If you've read 003 and it landed, skip this one.

## What "falsifiable" means here

A claim is **falsifiable** if you can describe an experiment whose result would prove it wrong. "All swans are white" is falsifiable: find one black swan and you're done. "AI is changing society" is not falsifiable: nothing you observe could prove it wrong, because the claim is too vague.

The model V5 has lots of claims. The question this review asks: which ones could you actually test, and which ones are just stories?

## TL;DR

- V5 is honest about what it can prove. Where V4 said "this is testable" and wasn't, V5 says "this is a guess." That's progress.
- Four of those guesses can be turned into real studies. Each one needs roughly 30–80 people, followed for a year or two. Doable.
- The "reversibility test" for people who quit AI works, but only as a first sort. To get the full picture you need to interview them too.
- The S2T Trust Evaluation versus S2D Defensive Resistance test (people who evaluate AI fairly versus people who evaluate it defensively) needs a controlled experiment, not just observation. The recipe is in the findings below.
- The model is in good shape to start collecting real data. Some of the experiments need tightening up before you run them.

## Findings

### 1. "Mechanism anchors" don't tell you who is in which state

V5 attaches a **mechanism anchor** to each state. That's psychology-speak for "the reason someone behaves this way." For example, S3 Ego Shock (the panic state) is anchored to "self-efficacy collapse" — the feeling of *I'm not good at my job anymore*.

The problem: knowing the reason doesn't help you identify the state. If you see a coworker looking miserable about AI, you can guess it's self-efficacy collapse. But it could also be: they're worried about money, they're tired, they had a bad week, or their boss yelled at them. The mechanism anchor explains the state once you've identified it. It does not help you identify it in the first place.

**Fix:** Add a sentence saying mechanism anchors are explanations, not diagnostic tools.

### 2. The lightning bolt on S3B Bargaining is overstated

V5 uses a ⚡ symbol to mark states that get triggered by external events. S3B Bargaining (where someone makes a deal with themselves to use AI for some things but not others) has ⚡ pointing at "model releases" as the **primary** cause of the state.

That's wrong. People enter S3B Bargaining because they're uncomfortable with AI being good at their job (an internal struggle). A new model release can speed this up or shake the deal loose, but the model release isn't what creates S3B Bargaining. Someone could enter S3B Bargaining without any new release happening.

**Fix:** Drop the word "primary." Say model releases accelerate S3B Bargaining, not cause it.

### 3. "Most people cycle through more than once" — testable

V5 says people don't pass through this model just once. They reach a stable place (S5 Understanding or S7), then a new AI release knocks them back to an earlier state, and they go through again.

This claim sounds true but right now is just a hunch. You can test it. Here's how:

- Find 60 people who are currently in S5 Understanding or S7.
- Check on them every 3 months for 18 months.
- Count how many slide back to S2D Defensive Resistance or S3 Ego Shock and then climb out again.
- If fewer than 30% cycle, the claim is wrong.

Cost: about $80k. Not expensive for a study that turns a hunch into evidence.

### 4. "S5 Understanding needs both internal and social acceptance" — testable

V5 says S5 Understanding (the stable, integrated state where AI use feels normal) requires two things at once: **internally**, your mental model of work makes sense; **socially**, the people around you treat AI use as no big deal. If either piece breaks, you fall out of S5 Understanding.

Right now this is a guess. It's also easy to measure:

- **Internal piece:** interview the person. Ask them to explain when and how they use AI. Score whether their explanation hangs together.
- **Social piece:** ask how often AI comes up in their team without anyone making a big deal of it.

Find 50 people in S5 Understanding. Measure both pieces. Watch them for a year. If someone falls out of S5 Understanding only when one of the pieces breaks, the model is right. Cost: about $60k.

### 5. "Stable evangelists were once shaken" — testable

V5 says people who become long-term AI cheerleaders (S7F Evangelism) tend to have *previously* gone through the panic state (S3 Ego Shock). The idea: you can't credibly help others through the rough part if you never had a rough part yourself.

To test:

- Find 25 active AI evangelists.
- Ask each one whether they ever felt threatened or shaken by AI.
- Watch them for a year.
- If anyone who never felt shaken stays stable as an evangelist, the claim is wrong.
- If anyone who never felt shaken collapses under pressure (becomes the loudest voice in a room because that's what their team rewards), the claim is also testable but a different way.

Cost: about $20k.

### 6. "S3B Bargaining versus S7A Maturity look similar but behave differently" — testable

S3B Bargaining and S7A Maturity both look like "I use AI for some things but not others." The model says they're different underneath:

- **S3B Bargaining:** when a new model comes out, the person quickly moves their personal line about what AI is allowed to do, without checking whether the new model is actually better at it.
- **S7A Maturity:** when a new model comes out, the person tests it before deciding whether to expand AI's role.

You can watch this happen. Recruit 40 people (20 in each state), wait for two model releases (typically 6–12 months apart), and watch what they do. Did they test before changing their stance, or did the boundary just slide? Cost: about $50k.

### 7. The reversibility test has four traps

The reversibility test is for people who quit AI. The idea: offer them a tool that fixes their stated complaint. If they come back, the tool was the real problem. If they don't, something deeper was going on.

Four things can mess up this test:

- **Switching costs.** A better tool still means learning something new. They might decline because they don't want to relearn, not because of identity issues. Fix: offer training and walk them through it.
- **Saving face.** If they publicly quit AI, restarting looks like changing their mind in public. Fix: offer it privately as part of a study, not as "hey come back."
- **Shame.** When the tool failed them the first time, it might have made them feel stupid. Fixing the tool doesn't fix the leftover bad feeling. Fix: ask them after they restart whether anything still feels off.
- **They were just stressed.** Maybe the original quit happened during a bad month at work, and now things are calmer. The improved tool gets credit it doesn't deserve. Fix: test the tool when work pressure matches what it was the first time.

### 8. The reversibility test only sorts into two piles, not four

The model claims dropout has two dimensions: practical (the tool didn't work) and emotional (it made me feel bad). That gives four kinds of dropout: pure-practical, pure-emotional, both, and neither.

The reversibility test only tells you who restarts and who doesn't. That's two piles. To split them properly into the four kinds you need to also:

- Interview the restarters to see if there was emotional baggage as well.
- Interview the non-restarters to see if it was the tool or the feelings.
- Try offering the tool again 6 months later and see if anything changed.

**Fix:** rename it "Reversibility Test (Screening Instrument)" and add the follow-up steps.

### 9. The S2T Trust Evaluation versus S2D Defensive Resistance test is solid, with caveats below

S2T Trust Evaluation people evaluate AI fairly. S2D Defensive Resistance people evaluate it defensively — they latch onto any flaw and ignore any strength. This is well-grounded in existing psychology research on how people defend their identities against threatening information.

To test it:

- Take 40 people in S2T Trust Evaluation and 40 in S2D Defensive Resistance.
- Show them 8 strong AI outputs and 8 weak ones.
- Ask each person to estimate what fraction of all AI outputs would be this good or this bad.
- The S2D Defensive Resistance group should weight the bad examples way more heavily than the S2T Trust Evaluation group.

This is normal psychology methodology. Nothing exotic.

### 10. The S2T Trust Evaluation versus S2D Defensive Resistance test has a confound

Here's the trap: maybe S2T Trust Evaluation and S2D Defensive Resistance people just have different starting beliefs about AI. If an S2D Defensive Resistance person genuinely thinks AI is bad at their job, and an S2T Trust Evaluation person thinks AI is decent at it, they'll naturally focus on different evidence — even if neither is being defensive.

To prove it's identity-defense and not just different starting beliefs, you need an extra step: ask them up front what they expected, then show them evidence that contradicts what they expected, and watch how much each group updates. If S2D Defensive Resistance people refuse to update even when shown contradicting evidence, *that's* the identity defense kicking in.

### 11. The model doesn't say where defensiveness shows up

The model says S2D Defensive Resistance people defend against positive evidence about AI. But it doesn't say where this happens.

Example: a graphic designer is S2D Defensive Resistance about AI for design (it threatens her core skill) but might be totally relaxed about AI for writing emails (no skin in the game). Would she defend against positive evidence about AI's email writing? Probably not. The defensiveness should only kick in for things she cares about.

**Fix:** spell out that defensive evaluation only happens in domains where the person's identity is on the line.

## Recommendations

1. Add a note that mechanism anchors explain states, they don't diagnose them.

2. Drop "primary" from the S3B Bargaining lightning bolt. Say model releases speed it up, not cause it.

3. Rename the reversibility test to "Reversibility Test (Screening Instrument)" and add the interview and re-offer steps.

4. Run the S5 Understanding dual-component study. 50 people, 12 months, about $60k.

5. Run the cycling-and-regression study. 60 people, 18 months, about $80k.

6. Run the controlled S2T Trust Evaluation versus S2D Defensive Resistance experiment with priors measured up front. 80 people, about $40k.

7. Run the S7F Evangelism-without-prior-S3 Ego Shock study. 25 people, 12 months, about $20k.

8. Run the S3B Bargaining-versus-S7A Maturity boundary-tracking study. 40 people across two model releases, about $50k.
