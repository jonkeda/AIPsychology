This is a simpler rewrite of [012-one-shot-improvement.md](012-one-shot-improvement.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# One-Shot Improvement — Model V5 — Plain-Language Version

## Quick orientation

A few state names show up over and over. Once you know them, the rest is straightforward:

- **S6** — *Unsustainable engagement.* The person is using AI all day, leaning on it harder and harder, and running themselves down. V5 splits this into four flavors: S6A Enthusiastic Overuse, S6B Dependent Overuse, S6C Driven Overuse, S6D Social Overuse.
- **S7A Maturity** — *Stable integration.* AI use settles into a normal part of the job. The person is fine.
- **S7D Burnout** — *Burnout.* The person crashes out. They quit AI, change jobs, or stop functioning.
- **S3B Bargaining** — A negotiated state where someone uses AI for some tasks but refuses it for others, often as a self-protective deal.
- **S5 Understanding** — A stable, settled state where AI use feels normal both to the person and to the people around them.

The big claim of this review: the most useful thing the model could do is help a practitioner spot someone in S6 and tell them what to look for to know whether that person is heading for S7A Maturity or S7D Burnout. Right now V5 doesn't do that.

## TL;DR

- Collapse S6A Enthusiastic Overuse, S6B Dependent Overuse, S6C Driven Overuse, and S6D Social Overuse into one S6 state. The four flavors all come down to the same thing: the person is burning through more energy than they're putting back. The split adds detail without adding usefulness.
- Add explicit signs for when someone in S6 is heading toward S7A Maturity (settling down) versus S7D Burnout (crashing out).
- Right now, V5 leaves the practitioner blind at the worst moment. They can see someone burning out. The model gives them no idea what to do about it.
- The biggest payoff in the whole model is the moment someone leaves S6 — either toward stability or toward burnout. V5 fragments S6 into four sub-states but says nothing about what marks the exit. Fix that and the model becomes useful at exactly the point where intervention is still possible.

## Findings

1. The four S6 flavors all reduce to one underlying mechanism: **resource depletion** — the person is spending mental and emotional energy faster than they can refill it. Splitting that into four labels creates fake **precision**. It looks specific but doesn't help anyone identify which flavor someone is actually in.

2. V5 is **silent** on what tells you whether an S6 person is going to land in S7A Maturity (stable) or S7D Burnout (burnout). That transition is the highest-leverage moment in the entire model and the model has nothing to say about it.

3. Forcing practitioners to choose between four S6 states that all mean the same thing creates **cognitive load** with no payoff. Four labels for one phenomenon is worse than one label.

4. The Social Context layer (how peer behavior, workplace norms, and the surrounding culture shape AI adoption) is **undersized** relative to how much it actually drives transitions and stability. Right now it's a short bullet list. It should be a real sub-model.

5. The model lacks a **dropout feedback loop**. When several people drop out for similar reasons, what should the organization change so the next group doesn't drop out the same way? V5 doesn't address this.

6. S3B Bargaining's exit criteria are not **operationalized** — meaning, there are no concrete behaviors a practitioner can watch for to know that someone has exited S3B Bargaining. It's described in the abstract.

7. The "Limits of operationalization" section honestly admits which claims aren't directly testable, but stops there. It offers **no alternative**. A practitioner still needs to decide whether someone is in S3B Bargaining or S7A Maturity. The model should give them specific things to look for or ask, even if those aren't perfect.

## Recommendations

1. **Consolidate S6 and add exit markers.** Merge the four S6 variants into a single state called "S6 — Unsustainable Engagement," with resource depletion as the one underlying cause. Then add a subsection called "S6 Exit Markers — When S6 Becomes S7A Maturity vs. S7D Burnout" that lists three concrete behaviors a practitioner can watch for. For example: "rejects new use cases without testing them," "rebuilds independent judgment on familiar tasks," "reports that pausing AI use no longer feels threatening." This single change fixes findings 1, 2, and 3 in one pass.

2. **Develop the Social Context layer.** Expand the three-bullet list into a real sub-model with explicit cause-and-effect chains showing how workplace and peer-group context drive entry into states and stability of S5 Understanding.

3. **Add a dropout feedback loop.** When several people drop out for similar reasons, specify what the organization should change so the next group doesn't repeat the pattern. Dropout tends to cluster by reason. The model should explain how to read those clusters and adjust the conditions that caused them.

4. **Operationalize S3B Bargaining exit criteria.** Replace the current abstract description with concrete behaviors. For example: "person runs the same benchmark test twice" or "person explicitly writes down the boundary they've drawn." Spell out what to watch for or ask about when distinguishing S3B Bargaining from S7A Maturity.

5. **Replace "Limits of operationalization"** with a practical measurement guide. For each claim the model says you can observe at a single point in time, and each claim that takes longer-term tracking, give a specific thing to measure or a specific question to ask.
