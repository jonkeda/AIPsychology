This is a simpler rewrite of [007-internal-consistency.md](007-internal-consistency.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Internal Consistency Audit — Plain-Language Version

## What this review checks

The model V5 is a state graph: people move between named states (S1 Initial Encounter, S2T Trust Evaluation, S3 Ego Shock, S5 Understanding, S6A Enthusiastic Overuse, S7C Ethical Integration, and so on) along defined transitions. It also has rules about which states get a ⚡ marker (a tag meaning "an external event like a workplace mandate or new model release can push you in or out"). And it has axes — separate dials, like Identity Stakes and Task Delegation Level — that are supposed to be independent of each other.

This review walks the model and asks: do the rules it states match the rules it actually follows? When the model says "this state has no external trigger," does the text on that same page contradict it? Are claims tagged honestly as "guess" versus "established"? Are the dropout-scoring tools tight enough that two reviewers would land in the same place?

## TL;DR

- **S2T Trust Evaluation marker is wrong.** Workplace mandates compress S1 Initial Encounter, which directly changes how fast and how often people enter S2T Trust Evaluation. The model says S2T Trust Evaluation has no external trigger. Those two things contradict each other. Same problem at S5 Understanding — it can be exited by capability jumps (a new AI model that suddenly does something it couldn't yesterday), which is exactly what the ⚡ rule is supposed to flag.
- **S7C Ethical Integration contradicts itself on the same page.** The header says "no external trigger" and the very next line lists external triggers (public AI ethics scandals, personal moral dilemmas).
- **S6A Enthusiastic Overuse and S7A Maturity overlap is not addressed.** S6A Enthusiastic Overuse is "uncritical AI cheerleader." S7A Maturity is "calibrated, measured AI user." The model lets you go from S6A Enthusiastic Overuse to S7A Maturity but never says you can't be in both at once in the same area of your life. You probably can't, but the model should say so.
- **S3 Ego Shock's mechanism (terror management) isn't tagged honestly.** It's borrowed from a psychology theory about facing your own death, then loosely applied to facing AI replacing you at work. That's a real stretch and should be marked as a guess, not as established theory.
- **The dropout severity scale is too loose.** The 0–10 scales for "practical severity" and "emotional severity" only have 4–5 example points to anchor them. Two reviewers scoring the same person would land 2 or 3 points apart, not 1 point apart.
- **The S2T Trust Evaluation/S2D Defensive Resistance fork is not as symmetric as the model claims.** S2T Trust Evaluation (rational evaluation) has a direct path to S5 Understanding (stable integration). S2D Defensive Resistance (defensive evaluation) does not — it has to go through emotional processing first. The model says "neither comes before the other," but the graph clearly says one path is harder.
- **Multi-occupancy rules are missing.** The model says you can be in multiple S6 states or multiple S7 states at once. It doesn't say whether you can be in S6 and S7 at the same time, or whether S3B Bargaining and S7A Maturity can coexist in the same domain.
- The model holds together at the broad level. The state graph, axes, mechanism anchors, and dropout plane mostly fit. But the ⚡ marker rule is the single biggest source of inconsistency: stated cleanly, applied with quiet exceptions. None of these problems are fatal. All are fixable in V6.

## Findings

### 1. Mechanism-state alignment

1. **S6A Enthusiastic Overuse's exit mechanism doesn't match its anchor.** S6A Enthusiastic Overuse is anchored to **variable-reward reinforcement** — the same dynamic that makes slot machines and social media addictive. The whole point of variable-reward is that unpredictable outcomes keep you hooked. But the model says S6A Enthusiastic Overuse exits to S7A Maturity "as the enthusiasm settles as the person learns where the tool fails." Learning where a tool fails should *increase* unpredictability, not cool you off. What's actually being described is curiosity running out — you've explored and now you're bored. Either add a different exit reason ("rewards run out, you get tired of it"), or change the anchor from "variable-reward" to "novelty-driven exploration." The current pairing doesn't add up.

2. **S7F Evangelism prerequisite claim is hand-wavy.** S7F Evangelism is the "stable mentor of others through their AI transition" state. The model says it probably requires going through S3 Ego Shock (the panic state) first, and admits this is a guess. But it doesn't say *why*. Erikson, the psychologist whose work on generativity is cited here, never said you have to be shaken to be a mentor. Plenty of teachers got there without crisis. Either give a real reason ("having gone through S3 Ego Shock makes a mentor credible to people currently in S3 Ego Shock") or weaken the claim to "S3 Ego Shock experience may help" instead of "S3 Ego Shock is required."

### 2. Multi-occupancy boundaries

3. **Can you be in S6 and S7 at the same time?** The model lets a person be in multiple S6 states at once and multiple S7 states at once. It never says what happens between them. The transitions imply you exit S6 when you enter S7, but the model also allows regression — could a person regress from S7A Maturity back into S6A Enthusiastic Overuse and stay there long-term, while still in S7B Identity Expansion for a different domain? The model doesn't say. **Fix:** add one sentence after the S7 introduction: "S6 and S7 are not simultaneous occupancy pairs; entering S7 ends S6 occupancy, and you can only return to S6 via regression."

4. **Can S3B Bargaining and S7A Maturity coexist across different domains?** The model already says a person can have low identity stakes in one area of work and high stakes in another. So a graphic designer could be S7A Maturity (calmly evaluating AI for emails) and S3B Bargaining (negotiating uncomfortable boundaries about AI for design). That's reasonable but never stated. The model also doesn't say the inverse — that S3B Bargaining and S7A Maturity *cannot* coexist in the same domain, because they describe two different ways of moving the boundary, and you can't do both at once. Both rules should be written down.

### 3. The S2T Trust Evaluation/S2D Defensive Resistance fork

5. **The fork isn't symmetric, even though the model says it is.** The model says: "Both S2T Trust Evaluation and S2D Defensive Resistance are responses to S1 Initial Encounter; neither comes before the other." But look at the actual transitions:
   - S2T Trust Evaluation can go to S5 Understanding directly. It can also go to S2D Defensive Resistance or to Dropout.
   - S2D Defensive Resistance cannot go to S5 Understanding directly. It has to go through S3 Ego Shock, S3B Bargaining, or S1 Initial Encounter first. Or to Dropout.

   So S2T Trust Evaluation has an escape hatch straight to a stable end-state. S2D Defensive Resistance doesn't — it has to detour through emotional processing first. That's not a false claim per se; the model never said the paths were *equally easy*. But a reader looking at the graph will reasonably conclude S2D Defensive Resistance is the harder path, and the model should just acknowledge that. **Fix:** add a sentence like "S2T Trust Evaluation has a direct path to S5 Understanding; S2D Defensive Resistance does not. This reflects the difference between rational and ego-defensive evaluation, not a fixed ordering."

### 4. The two axes

6. **No problems found.** The two axes (Identity Stakes and Task Delegation Level) stay independent throughout the model. The S3 Ego Shock intensity table treats them as two dials, not one implying the other. Clean.

### 5. ⚡ marker consistency

7. **S2T Trust Evaluation should carry ⚡.** The rule is: a state gets ⚡ if at least one named external event materially changes the probability of entering or leaving it. S1 Initial Encounter is marked as compressed by workplace mandates, peer adoption events, and compelling demos. If S1 Initial Encounter gets compressed by a mandate, then S2T Trust Evaluation is entered sooner and more often. That's a direct probability change for S2T Trust Evaluation's entrance, which is exactly what the ⚡ rule is supposed to catch. Yet S2T Trust Evaluation says "no external-event marker." Either add ⚡ to S2T Trust Evaluation with a note about workplace mandates, or rewrite the rule to say it only counts direct triggers and not knock-on effects from upstream states.

8. **S5 Understanding should carry ⚡.** S5 Understanding's transitions explicitly include "→ S3 Ego Shock — regression via external trigger." Capability jumps (a new model release that suddenly does what people thought only humans could do) are named external events. They change the probability of exiting S5 Understanding. That's the ⚡ rule, exactly. Add ⚡ to S5 Understanding with a note: "Re-triggered backwards by capability jumps that invalidate the integrated way of working."

9. **S7C Ethical Integration contradicts itself.** S7C Ethical Integration says: "⚡ No external-event marker: S7C Ethical Integration is internally driven. Triggers exist (a public AI ethics incident, a personal moral dilemma) but they *amplify* rather than create the state." This is a contradiction. The ⚡ rule says "any material change in probability of entering or leaving." It doesn't carve out an exception for "amplification." If a public AI ethics scandal makes more people enter S7C Ethical Integration than otherwise would, that's a material change and ⚡ applies. Either add the marker, or rewrite the rule to explicitly distinguish "creating a state from scratch" from "amplifying an existing tendency." Right now the model is using a distinction it never defined.

10. **S6B Dependent Overuse is ambiguous.** S6B Dependent Overuse says "no external-event marker: internally driven." But S6B Dependent Overuse is reached from S3 Ego Shock, and S3 Ego Shock is itself triggered by capability jumps. So external events do affect entrance to S6B Dependent Overuse, just one hop removed. The model seems to be saying that what matters for ⚡ is whether *staying* in the state is driven by external events, not whether *getting* there was. That distinction may be defensible, but it's nowhere in the rule. Pick one: does ⚡ apply to entering, staying, or both? Then audit every state against that choice.

### 6. Conjecture tags

11. **S3 Ego Shock's terror management borrowing isn't tagged honestly.** Terror management theory in psychology is about people facing their own mortality — the existential discomfort of knowing you will die. The model uses this "in the loose sense" to describe what happens when an AI threatens to make your job obsolete. That is a real stretch. Calling AI replaceability "the same kind of existential discomfort" as facing death is a hypothesis, not a fact, and there's no published research the model cites to back it up. Compare with how generativity (used at S7F Evangelism) gets a citation to Erikson and an explicit "this extension is conjecture" tag. S3 Ego Shock deserves the same treatment. Either add a note: "Terror management's application to AI replaceability is untested," or move it to the Limits section under "Currently conjecture."

12. **The two-axis dropout model is dressed up as operational, but isn't.** The model talks about the two severity axes and the reversibility test as if they're a working instrument. They're not. The model has not run them on real dropouts. The reversibility test has known confounds (see finding 14). Mark this section "proposed operationalization, pending validation." Add a note in Limits: "The two-axis dropout model has been designed but not yet tested. The reversibility test is a candidate protocol, not a validated instrument."

13. **"Most people cycle more than once" is correctly tagged conjecture, but vague.** The model says "more than once" without saying what counts as a cycle. Does re-entering S2T Trust Evaluation count? Does shifting around inside S7 count? Without a definition, the claim is unfalsifiable — anything could be called a cycle later. **Fix:** define it: "A cycle is exiting S5 Understanding+ states, re-entering S1 Initial Encounter or S2, and reaching S5 Understanding+ again." Now the claim can be tested.

### 7. Dropout scoring

14. **The reversibility test has four traps.** The reversibility test is: give a dropout a tool that fixes their cited complaint. If they restart, the tool was the real problem (high practical severity). If they don't, something emotional was driving the exit. Four problems with this:
    - **A tool can rarely isolate practical failure.** When AI made errors on a high-stakes task, the practical failure and the identity threat were tangled together. A "fixed" tool only addresses the practical side; you don't get to see whether the emotional driver was independent.
    - **Refusal to restart doesn't prove practical severity was low.** A person might refuse the new tool because they've internalized the original failure (learned helplessness — the pattern of giving up after repeated failures), not because of identity issues per se. That's emotional residue from the practical failure.
    - **The two axes might not be independent in real cases.** Many dropouts say things like "the tool failed, *and* I felt terrible about it." Forcing reviewers to score practical and emotional separately may not match how the experience actually felt.
    - **Worked example.** A person quits because "AI made high-stakes errors and I lost confidence in my own judgment." You give them a better AI for low-stakes tasks. They restart for low stakes. The test concludes "high practical severity." But the original dropout was tangled — identity threat at high stakes plus practical failure. The restart at lower stakes doesn't prove the original practical severity; it just proves they can recover when the stakes are lower.

15. **The 0–10 scales are too loose for ±1 inter-rater agreement.** The model gives four region-prototypes:
    - high practical / low emotional ("Tool genuinely doesn't work")
    - low practical / high emotional ("Identity threat or exhaustion")
    - high practical / high emotional ("Mixed")
    - low / low ("Boredom, indifference, opportunity cost")

    Take a real case: "I tried using AI for my writing, but every time I used it I felt like I was cheating, and the outputs were mediocre too." Two reviewers might score:
    - **Reviewer A:** practical 6 (mediocre outputs), emotional 7 (cheating guilt). Mixed region.
    - **Reviewer B:** practical 3 (workable with editing), emotional 8 (cheating drove the exit). Low practical / high emotional region.

    Both are defensible. The 0–10 scale offers 11 levels of granularity but only 4–5 example anchors. Two reviewers will land 2–3 points apart, not 1. **Fix:** give three concrete anchors (0, 5, 10) per axis with specific examples.

    Practical severity: 0 = tool works perfectly; 5 = intermittent failures (about 1 in 3 outputs needs heavy editing), workable; 10 = systematic failure on the core task, unusable.

    Emotional severity: 0 = no identity concerns, dropped out due to opportunity cost; 5 = mild discomfort about role or authenticity, manageable; 10 = severe identity threat, person describes the tool as threatening their sense of self.

## Recommendations

1. **Fix S7C Ethical Integration marker contradiction (finding 9).** Add ⚡ or rewrite the rule to distinguish creation from amplification. Do this before the next version is shared. The contradiction undermines confidence in the entire ⚡ system.

2. **Clarify the ⚡ rule's scope (findings 7, 8).** Decide whether ⚡ applies to direct triggers only, or also to knock-on effects from upstream compression. Then audit every state against the clarified rule. Add ⚡ to S2T Trust Evaluation and S5 Understanding, or rewrite their text to fit a narrower rule.

3. **Acknowledge the S2T Trust Evaluation/S2D Defensive Resistance asymmetry (finding 5).** Add a sentence saying S2T Trust Evaluation has a direct path to S5 Understanding and S2D Defensive Resistance does not. This doesn't break the "no implied order" claim; it explains why the two paths feel structurally different.

4. **Tag S3 Ego Shock's terror management as conjecture (finding 11).** Add a note that applying terror management theory to AI replaceability is an untested extension, not established theory.

5. **Define multi-occupancy rules (findings 3, 4).** State plainly: "S6 and S7 are not simultaneous occupancy pairs," and "S3B Bargaining and S7A Maturity cannot coexist in the same domain but can coexist across different domains."

6. **Anchor the dropout scoring scales with concrete reference points (finding 15).** Provide 0, 5, and 10 examples for both axes. Test inter-rater agreement on 5–10 real dropout cases. If reviewers can't agree within ±1, adjust the descriptions further.

7. **Reframe S6A Enthusiastic Overuse's exit (finding 1).** Either add a satiation/plateau condition that explains why variable-reward engagement naturally winds down, or change the anchor from "variable-reward reinforcement" to "novelty-driven exploration."

8. **Demote the two-axis dropout model from "operational" to "proposed" (finding 12).** Frame the axes and the reversibility test as a tool to *explore* dropout cases, not to *measure* them. They haven't been tested.
