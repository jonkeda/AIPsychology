This is a simpler rewrite of [002-related-literature.md](002-related-literature.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Related-Literature Audit — V6

## TL;DR

- V6 renames V5's "Mechanism anchors" to "Related literature" and drops the claim that they're causes. That's honest — V5 was overselling. But it also means V6 stopped trying to explain *why* states happen.
- Three of the four psychology references (self-efficacy, variable-reward, metacognitive calibration) are well-matched to their states. The fourth — "terror management" for S3E — borrows the wrong term.
- The references do useful work within a state family (comparing states that look similar). They do less useful work across families.
- S3E's two-part anchor (efficacy collapse + terror management) is defensible, but "terror management" is the wrong label for what it's actually describing.
- These references help you understand what a state *is*. They don't help you figure out which state someone is in.

---

## 1. The rename is honest, but it's also a step backward on explaining *why* things happen

V5 called these "Mechanism anchors" and used strong cause-and-effect language. For S3E Ego Shock, V5 said: "self-efficacy collapse **under domain-specific capability threat**" and "terror management in the loose sense — **confrontation with one's own replaceability triggers** the same kind of existential discomfort that confrontation with mortality does." The syntax commits to a cause: the threat *makes* the collapse happen.

V6 calls them "Related literature" and explicitly backs off: "Borrowed conceptually as vocabulary; self-efficacy collapse is offered as a frame for thinking about S3E, not as a tested cause." Model6.md goes further: knowing that S3E is related to self-efficacy collapse tells you what *kind* of phenomenon S3E is. It doesn't let you diagnose S3E in a person, and it doesn't commit the model to claiming self-efficacy collapse is the cause.

This is **honest**. V5 was presenting causal mechanisms without any evidence they were right, and V6 corrects that. But it's also **a retreat**: V6 downgrades from "here is why S3E happens" to "S3E is conceptually similar to self-efficacy collapse," without replacing the dropped causal story or saying anything about what was lost. A reader who came to V6 expecting an answer to "why does S3E happen?" gets: "S3E belongs to the same family of phenomena as self-efficacy collapse." That is useful, but it is not the same thing.

**Fix:** Add one paragraph in Model6.md after the "Related literature is conceptual, not diagnostic" section, explaining the tradeoff directly. Something like: "V5 proposed that self-efficacy collapse *caused* S3E. V6 treats self-efficacy collapse as a label for what kind of thing S3E is, without claiming to know the cause. That makes the model more honest but less explanatory." Readers need to know they are not getting a causal explanation in V6 — not because the model is being humble, but because the cause hasn't been tested.

---

## 2. "Terror management" is a poor label for S3E; the other three references are accurate

Here is the hit rate on the four psychology references:

**Self-efficacy (a person's belief that they can actually do a thing) for S3E (Ego Shock — where someone realizes that a skill they built their career around can now be done by a tool).** Accurate. Self-efficacy theory is exactly about believing "I can do this." When AI demonstrably does the task the person trained for, that belief no longer works the same way. Precise fit. ✓

**Variable-reward (the slot-machine effect: behavior that keeps going because the payoff is unpredictable) for S6E (Enthusiastic Overuse — routing everything through AI even when it's the wrong tool, driven by the thrill of unpredictable hits).** Accurate. This is exactly how slot machines, social media feeds, and mobile games create compulsive use. V6's description — "intermittent-reward dynamic that underlies compulsive engagement with any tool whose outputs are unpredictably good" — is textbook Skinner. ✓

**Metacognitive calibration (knowing accurately when your own judgment is reliable and when it isn't) for S7M (Maturity — using AI when it's better, skipping it when it isn't, and only updating that line when measured evidence says to).** Accurate. Research on calibration is exactly about whether people know the limits of their own judgment. Precise fit. ✓

**Terror management (a psychological theory about how people respond to reminders of their own death) for S3E (secondary mechanism).** Loose fit. Terror management theory (Greenberg and Solomon) is about the anxiety people feel when reminded they will die. The existential discomfort in S3E — when someone confronts that they might be professionally replaceable — is real, but it is not the same thing as death anxiety. Calling it terror management stretches the concept into a domain it wasn't built for. V6 hedges with "in the loose sense," but that doesn't fix the mismatch. Better terms exist.

**Fix:** Replace "terror management in the loose sense" with "confrontation with replaceability as an existential threat" or just "the existential discomfort that comes from confronting one's replaceability." If you want a canonical psychology term, consider "existential threat response" — it covers identity threat without dragging in the death-anxiety baggage. If you drop the term entirely, say: "the existential discomfort from confronting one's replaceability compounds with the efficacy loss." The self-efficacy collapse is doing the real work anyway.

---

## 3. How much weight each reference carries depends on which state you're looking at

The three references don't all do the same amount of work:

**S7M's metacognitive calibration is carrying real weight.** It's what separates S7M Maturity from S3B Bargaining. From the outside, both states look identical: "uses AI for some things, not others." V6 says the difference is that S7M people draw the line based on where AI is actually reliable (the competence line), while S3B people draw the line based on what feels too important to hand off (the identity line). Metacognitive calibration explains the competence-line logic and gives you a concrete observational test: the S7M person can name specific failure modes of the tools they use; the S3B person cannot. This reference is genuinely load-bearing.

**S6E's variable-reward is doing moderate work.** It explains *why* the S6E person stays uncritical (random good results sustain behavior despite failures), and it distinguishes S6E from S6D (Dependent Overuse — anxiety-driven), S6R (Driven Overuse — productivity-goal-driven), and S6S (Social Overuse — peer-pressure-driven). But the main discriminator between these states is the emotional register — what the person is feeling — not the variable-reward label alone. Variable-reward could show up in other contexts too. This reference names the mechanism for S6E but couldn't on its own tell you "this is S6E and not something else."

**S3E's two-part reference (self-efficacy + terror management) is doing work, but conditionally.** The self-efficacy piece is what separates S3E from S3B (S3B is about managing the discomfort of holding contradictory beliefs, not about losing confidence in a skill). But the two-part compound only works if both pieces are active. If confidence collapse happens without any existential element — say, someone loses confidence in a skill they never much cared about — is it still S3E? If someone has existential dread about AI's impact on their field without ever having built confidence around a specific skill, is that S3E? V6 doesn't answer either question. The compound is carrying weight for the S3E vs S3B distinction, but you're relying on it to do two things at once, and the two parts don't always line up.

**Fix:** In the S3E state file, separate the weight-bearing part from the typical-but-not-required part. "This state is characterized by loss of efficacy belief in the core skill" (the actual anchor) and "A secondary existential element may compound this" (the typical accompaniment). Make clear that efficacy collapse is necessary for S3E and the existential register is common in high-stakes situations but not required. This prevents the state from being defined as a compound when really only half the compound is the core.

---

## 4. These references help you understand a single state, not pick the right state from a lineup

If you already know someone is in S3E, knowing "S3E is related to self-efficacy collapse" is useful. It tells you what's going on under the hood. But if you're looking at someone and trying to figure out *which* state they're in, these references don't help much.

Here's why: each reference describes an internal psychological process (belief in your ability, reward-driven behavior, accuracy of self-assessment). But each state is that process *plus* a specific combination of identity stakes and AI delegation level. The same underlying process can show up in multiple states. Variable-reward-driven behavior could appear in S5 Understanding (someone who has learned to use AI well and enjoys unpredictable wins) or in S6E (Enthusiastic Overuse) depending on everything else. Metacognitive calibration exists in S5 Understanding and S7M Maturity and even S3B Bargaining — most S3B users do calibrate their scope, they just calibrate on identity grounds rather than competence grounds.

The references anchor individual states to existing psychology. They do not form a diagnostic system on their own.

**Fix:** In the observation guide, add a note saying explicitly that the related-literature references are not diagnostic tools. Something like: "These constructs explain what each state involves cognitively, not how to identify which state a person is in. Use behavioral markers and the state-graph logic for identification. Use the related-literature names to understand what you are looking at once you have already identified the state."

---

## 5. The two-part anchor for S3E works, but the second part is named badly

The question: is "self-efficacy collapse + terror management" a genuine compound or two loosely-related ideas stapled together?

It is **a genuine compound**. The two parts reinforce each other when the skill is central to the person's professional identity:

1. Efficacy collapse says: "I can no longer claim exclusive expertise in this skill."
2. Existential threat says: "This skill defined my role. If I can't claim it, what's left?"

These are not independent. The second amplifies the first when the person's identity is at stake. Someone who loses confidence in a low-stakes skill — say, doing mental arithmetic when a calculator exists — does not feel existential threat. Someone who loses confidence in a high-stakes skill — writing, if they are a novelist — feels both. The compound is real.

But it is **named badly**. Two problems:

1. "Terror management" is the wrong label. Terror management is about anxiety triggered by reminders of death and dying. Using it for replaceability anxiety imports death-anxiety meaning into a domain where it doesn't belong. "In the loose sense" doesn't fix this.
2. The compound assumes both parts activate together. If someone experiences confidence collapse without existential threat (because the skill was never identity-central), are they in S3E? The model doesn't say. If someone has existential dread about being replaced without ever having built confidence in the specific skill, is that S3E? It doesn't sound like it, but the model leaves room for it.

**Fix:** Rename the existential component to "confrontation with one's replaceability" or "existential threat through skill displacement" and drop the terror-management reference. Then add a note in the S3E file: "The two-part pattern is most visible when identity stakes are high. At low identity stakes, efficacy collapse can occur without the existential element. S3E is primarily defined by efficacy collapse; the existential register is typical in high-stakes situations but is not required."

---

## Recommendations

1. **Replace "terror management" with a more precise label.** Use "confrontation with replaceability as an existential threat" or drop it and say "existential discomfort from replaceability." Terror management specifically refers to death-anxiety responses and should not be used for identity-threat responses. This is a correctness fix, not optional. (Priority: high)

2. **Add one paragraph in Model6.md explaining what was traded away by moving from mechanisms to vocabulary.** Say that V5 claimed specific causal mechanisms without evidence, V6 dropped those claims to be more honest, and this makes the model more careful but less explanatory. Readers need to know they are not getting "why S3E happens" — they are getting "what S3E is conceptually similar to." (Priority: high)

3. **In S3E, separate the core anchor (efficacy collapse) from the typical-but-not-required part (existential element).** Make clear that efficacy collapse is what defines the state, the existential element is common in high-stakes situations, and the two reinforce each other — but the first is the actual anchor. (Priority: medium)

4. **In the observation guide, add a note that related-literature references are not diagnostic tools.** Say: "These anchors explain what is happening cognitively in each state, not how to identify which state a person is in. Use behavioral markers and the state-graph logic for identification." (Priority: medium)

5. **Audit the other states for similar loose-fit references.** Check S6R (Driven Overuse, anchored to "goal-substitution"), S6D (Dependent Overuse, anchored to "self-efficacy displacement"), and S7F (Evangelism, anchored to "generativity") for the same precision applied to S3E. If "generativity" is just an Erikson name-drop without precision, rename it. (Priority: low)
