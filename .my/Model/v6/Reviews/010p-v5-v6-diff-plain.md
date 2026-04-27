This is a simpler rewrite of [010-v5-v6-diff.md](010-v5-v6-diff.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# V5 → V6 Diff Review — Plain Language

## TL;DR

- **Renaming "mechanism anchors" to "related literature"** is honest — V5 was implying more causal grounding than it had. V6 stops pretending. But the same concepts stay, unchanged. Only the label changed, not the content.
- **"Descriptive-first" declaration** is accurate but doesn't change much. V6 still makes causal-sounding claims in the same breath. The actual text needs to change, not just the disclaimer at the top.
- **Inline Conjecture / Testable markers** work better than a single bottom section. Saying a claim is uncertain right next to the claim beats burying it at the end.
- **State ID renames** (S3 → S3E, S6A/B/C/D → S6E/D/R/S, S7A/B/C/D/F → S7M/I/E/B/V) were needed. V5's naming was a mess. V6 is clean and easier to remember.
- **New S2T → S2D edge** is correct and small — if you discover something threatening while evaluating openly, you can shift to defensive mode.
- **Direct S3E → S5 edge** is probably real but cannot be observed in practice. You cannot tell it apart from someone who went through S3B very quickly. Either remove it or move it to the open questions list.
- **S3X Structural Displacement** earns its place. It separates "my identity is threatened" from "my job is being eliminated." Those are different problems that need different responses.
- **PEN Pre-emptive Non-Adoption** is useful vocabulary but hard to diagnose. You cannot reliably tell it apart from S2D Defensive Resistance in a single conversation. Most real cases are mixed.
- **Per-domain identity scoping** is clearer now but applied inconsistently. Some state files still write as if a person has one state globally, not one state per domain.
- **Multi-occupancy rules** (which S6 states can coexist) are well-reasoned and fill a real gap from V5.
- **S0's permanent-non-user reading** is real coverage. It separates "hasn't encountered AI yet" from "never will." That matters for not misclassifying someone as S2D when they are simply outside the system.
- **Grief language removed from S3E** is correct. S3E is about identity reorganization, not mourning. V5's "loss" framing pointed practitioners in the wrong direction.
- **File split** (one state per file) makes navigation easier at the cost of losing the whole-model-at-a-glance view. Net positive.
- **New top-level guides** (healthiness, usage, observation) were missing from V5 and needed. Not noise.
- V6 is a solid working improvement. It is honest about what is tested and what is not. The two main loose ends — the unobservable S3E → S5 edge and the fuzzy PEN vs S2D boundary — should be tightened before V7.

---

## Findings

### 1. Renaming "mechanism anchor" to "related literature" is honest but does not change the content — improvement at the cost of less boldness

V5 said each state was "anchored" to concepts from cognitive science — self-efficacy, cognitive dissonance, terror management, and so on. The word "anchored" implied these were proven causes. They were not. They were vocabulary chosen because it fit the observed pattern.

V6 reframes these as "related literature" and adds a disclaimer: *"related literature anchors a state in existing thinking and points the reader at further reading, but does not predict behaviour, identify states, or claim causal mechanisms."*

That is honest. V5 was overselling.

But nothing else changed. The exact same concepts appear with the exact same descriptions. S3E still mentions self-efficacy collapse and terror management. S6E still mentions variable-reward reinforcement. S7M still mentions metacognitive calibration (awareness of your own thinking). The content is identical. Only the label on the tin changed.

This fix creates a new problem: V6 now gives the model permission to keep any concept as long as someone, somewhere, has written something vaguely related — without testing whether it actually explains the state. The disclaimer is honest but makes the model easier to bloat over time.

**Fix:** Keep the reframing. Add a second rule: *"Related literature must name a specific, established concept from prior work, and the connection must be the most direct one available. If a simpler concept exists, use it. Do not use related literature as a holding bin for vague resemblances."*

---

### 2. "Descriptive-first" declaration is honest about attitude but doesn't change the text — real but narrow

V6 opens with: *"This model is descriptive. It provides names for recognisable psychological patterns… It does not provide causal mechanisms. Empirical predictions. Diagnostic instruments. Treatment protocols."*

This is accurate and needed. V5 implied in places that it had empirical grounding it didn't have.

But the declaration does not clean up the actual text. V6 still writes things like *"Self-efficacy collapse is offered as a frame for thinking about S3E"* and *"Cognitive dissonance reduction via scope limitation (Festinger)"* as the anchor for S3B. Those are claims about what causes what, dressed in softer language. The model still says self-efficacy collapse explains why S3E feels the way it does.

A genuinely descriptive model would say: "S3E reliably shows these symptoms and these transition patterns. Whether self-efficacy is the cause is an open question." V6 takes a position on the cause while calling itself descriptive.

**Fix:** The declaration is fine. Add this precision to Model6.md: *"'Descriptive' means we observe the state and its transitions. 'Related literature' names concepts from prior work that may explain why the state behaves as it does. We have not tested these explanations. Treat them as working hypotheses, not proven causes."*

---

### 3. Inline Conjecture and Testable markers are better than a single bottom section — improvement

V5 collected all uncertainty notes into one section at the end. V6 marks each claim where it appears: *"**Testable —** distinguishing the direct path requires following the same person over time"* or *"**Conjecture —** the four coexistence claims are based on observation of two cultural archetypes."*

This is better. You now know immediately whether a claim is tested, testable, or a guess — without hunting through a bottom section.

The downside: it is now easier to miss how much of the model is still untested. You can see that S2T vs S2D is unresolved right there on that page. But you cannot easily see that most transitions have no probability estimates at all.

The gain outweighs the cost.

**Fix:** None needed. Extend it: search for hedging language throughout the model files — words like "typically," "usually," "often." Any sentence using that kind of language should either carry a Testable or Conjecture marker, or have the hedge removed.

---

### 4. State ID rename (S3 → S3E, S6 family, S7 family) was overdue — improvement, worth the disruption

V5 used:
- Bare **S3** for what V6 calls **S3E** (Ego Shock) — inconsistent, since S3B and S3X were also under S3.
- **S6A/B/C/D** — letters with no connection to the state names.
- **S7A/B/C/D/F** — letters with no connection, and skipping E for no clear reason.

V6 renames to:
- **S3E** (Ego Shock), **S3B** (Bargaining), **S3X** (Structural Displacement) — consistent.
- **S6E/D/R/S** — first letter matches the state name (Enthusiastic, Dependent, pressure-dRiven, Social).
- **S7M/I/E/B/V** — first letter matches the state name (Maturity, Identity expansion, Ethical integration, Burnout, eVangelism).

V5's naming was chaotic. V6 is clean. Anyone who learned the V5 labels will need to re-learn them, but these are working documents, not published papers. Fix it once and move on.

One brittle point: S6D stands for Dependent and S6R stands for pressure-Driven. Both D and R look similar on a quick scan, and a reader who knows the word "Driven" might expect D for that, not R. The files back up the naming, but the diagram could confuse someone skimming it.

**Fix:** Accept the rename. For S6D vs S6R, add a note in the state graph or each state file: *"S6D = Dependent (personal ability eroding). S6R = pressure-Driven (external goals crowding out personal ones)."* Make the distinction visible.

---

### 5. New S2T → S2D edge: correct and small — improvement

V5 had S2T (open evaluation) and S2D (defensive resistance) as two separate responses to S1, with no path between them once you picked one. V6 adds a **S2T → S2D** edge: if someone starts evaluating openly but discovers something that threatens their sense of self, they can shift to defensive mode.

This is correct. Open evaluation and defensive evaluation are not fixed personality traits. What you discover can change your stance. V5 treated the fork as permanent; V6 treats it as driven by evidence.

The edge is narrow and does not destabilize the model. The two states remain separate responses to S1. The new edge just allows a mid-course shift when the evidence gets uncomfortable.

**Fix:** None. This is solid.

---

### 6. Direct S3E → S5 edge: removes strategic pressure and cannot be observed — lateral move, possibly a regression

V5 had S3E Ego Shock splitting into **S3B Bargaining** (negotiate scope of AI use) or **S5 Understanding** (direct integration), with the direct path being rare for high-stakes cases. V6 adds an explicit **direct S3E → S5 edge** and marks it "rare," with this note: *"Most people who appear to take this path are actually doing an accelerated S3B."*

Here is the problem: if the direct edge exists and is "rare," how do you tell whether someone took it versus a very fast S3B? V6 says: *"**Testable —** distinguishing the direct path from a fast S3B requires following the same person over time; on a single observation the two look identical."*

That is honest. It also means this edge is useless in practice. When you see someone move from S3E to S5 quickly, you cannot tell which path fired. You cannot plan an intervention based on a transition you cannot observe in real time.

V5 had this same problem but was quieter about it. V6 makes the problem explicit and then adds the edge anyway. That feels backwards: "We know this is unobservable, but we're including it because it matches our intuition."

The edge is probably real. But leaving it out of V6 would have been more defensible than including it with a caveat that it is indistinguishable from its neighbor.

**Fix:** Remove the direct S3E → S5 edge, or move it to the open questions section and say: *"Conjecture: some people can integrate S3E without bargaining. Testable: distinguishing this from fast S3B requires following people monthly or weekly over an extended period. Until that data exists, treat S3E → S5 as a theoretical possibility, not a modelled transition."*

---

### 7. S3X Structural Displacement earns its place — improvement

V5 had no concept for the case where someone concludes that their role is being economically eliminated, not just disrupted. The model could describe S3E Ego Shock, but if the real question was "there may be no position left to adapt to," the model had nothing to say.

V6 introduces **S3X Structural Displacement**: the problem is no longer psychological (can I adapt?) but structural (is there a job to adapt into?).

This separates identity-crisis work from labor-market crisis. A person can face both at once, but they need different responses. The model now says: structural displacement is outside the integration cycle.

The state file is honest about the three outcomes: move to a different domain (and start the model again there), leave knowledge work on principle, or fight back through advocacy (also outside the integration cycle). This is clean and accurate.

**Fix:** None. The only open question — whether the three outcomes are complete — is honestly marked as a guess. Keep the state.

---

### 8. PEN Pre-emptive Non-Adoption is useful vocabulary with a weak diagnostic — qualified improvement

V6 adds **PEN Pre-emptive Non-Adoption**: a stable decision not to use AI, made at or shortly after first encounter, based on values rather than on testing or identity threat.

This concept is needed. Someone can decide not to use AI because it conflicts with what they believe — without it threatening their sense of self and without ever testing it. V5 had no term for this.

But V6 admits the signs you would look for to identify the state are unreliable. Distinguishing PEN from S2D (Defensive Resistance) requires three signals — and then notes: *"Most real cases are mixed."*

This is honest, but it means PEN is easier to name in hindsight than to identify during an actual conversation. A practitioner might think they are seeing PEN (a values-grounded refusal) and later find it was S2D with ethical language on top.

The concept is useful for understanding non-adoption. The diagnostic is weak. You can use it to understand someone after extended dialogue, but you cannot use it to route an intervention after a single encounter.

**Fix:** Keep PEN. Upgrade the diagnostic: *"PEN is most reliably distinguished from S2D Defensive Resistance by asking: Does the person's position hold if their concern is addressed? In S2D, a better AI actually tightens the defensive stance. In PEN, a better AI reveals that the core concern — labour displacement, data exploitation, and so on — is not solved by capability. It is solved by values, policy, or economics."* Mark this as testable and point toward a future study design.

---

### 9. Per-domain identity scoping is clearer in principle but applied inconsistently — improvement that is incomplete

V5 said identity stakes are relative to a domain, but the model often wrote as if a person's state were a single global thing: *"they entered S3E"* rather than *"they entered S3E in domain X."*

V6 makes per-domain scoping explicit. The scope statement says identity stakes are *"a property of the person relative to a capability domain."*

The improvement is real. But V6 still breaks its own rule in places:

- S7M Maturity: *"In high-stakes domains S7M typically follows S3E."* Per-domain. Correct.
- S5 Understanding: *"Most adapted users settle into a combination (S7A + S7C is common…)"* — uses V5 labels, does not clarify which domain. Incorrect.
- Limits of Operationalization: *"'Most people cycle through the model more than once'"* — once per domain, or globally? Not clear.

A person who is S2D in writing, S5 in marketing, and S7M in graphic design should be able to track all three separately. The files mostly support this. Some don't.

**Fix:** Check every state file for phrases like "the person" or "the state" used as if the state is global. Where that appears, clarify: is this per-domain, global, or does it depend on the example? Add a standard note to each state file: *"[State name] applies within a domain. The same person can be [State A] in one domain and [State B] in another."*

---

### 10. Multi-occupancy rules clarify a gap in V5 — improvement, not over-engineering

V5 said S6 states sit downstream of S5 but said nothing about whether someone could occupy two S6 states at the same time.

V6 spells this out:
- **S6E and S6D are mutually exclusive** — opposite feelings; you can move from one to the other, but you cannot stably hold both.
- **S6R and S6S can coexist** — external pressure and going-along-with-the-crowd reinforce each other.
- **S6E and S6R can coexist** — typical in startup contexts (enthusiastic and under efficiency pressure simultaneously).
- **S6D and S6S can coexist** — typical in compliance-heavy workplaces (self-doubt plus feeling watched).
- **All S7 states can coexist** — multiple stable identities are possible at the same time.

The rules are honest about their basis: based on observation of two workplace archetypes (startup and compliance-heavy), not directly tested. That is the right flag to put on them.

This is useful in practice. If you see someone apparently in S6E + S6D simultaneously, something is off. If you see S6E + S6R, that is expected.

**Fix:** None. This is solid.

---

### 11. S0 expanded to cover permanent non-users — real improvement, not a token gesture

V5 treated S0 as transitional: someone who has not encountered AI yet, nothing more.

V6 distinguishes two readings:
1. **Pre-encounter** — not yet exposed, probably will be. Transitional.
2. **Permanent non-user** — will not engage, ever. Terminal.

This matters. Someone who has never used AI and never will is not in S2D Defensive Resistance — which requires having considered AI and rejected it on identity-threat grounds. They are not in PEN — which requires a values-grounded decision. They simply have not formed a stance. They are outside the system.

V5 risked classifying "my elderly relative does not use AI" as S2D. V6 says: no, some people are simply outside the model because they have never encountered it and never will.

A practical probe: ask "What do you know about AI from direct personal experience? Can you describe a specific product you tried?" No meaningful answer means probably a permanent non-user, not a defensive resister.

**Fix:** None. This is good.

---

### 12. Grief language stripped from S3E — correct diagnosis, not evasion — improvement

V5 described S3E with language that implied loss and mourning: "existential discomfort," "confrontation with one's own replaceability." The framing suggested the person was working through bereavement.

V6 reframes S3E as **reckoning**: *"The person is confronting the fact that the skill they built their self-concept around is now also something a tool can do. The work of S3E is reorganising self-concept around that fact, not mourning a lost capability."*

This is more accurate. The person has not lost their skill. They still have it. What changed is that it is no longer unique. The right emotional frame is anxiety and destabilization, not sadness or loss.

V6 adds: *"Affect is anxious or destabilised; not sad in the bereavement sense."* This helps practitioners distinguish S3E from actual grief, which has a different timeline and needs different support.

The change is not evasive. It is corrective. V5's grief language was imprecise and pointed to wrong interventions.

**Fix:** None. This is a good correction. Extend it: in the healthiness file, note that treating S3E as grief can lead to prolonged support when the person actually needs reframing, not grieving space.

---

### 13. File split (one state per file) gains navigation, loses coherence — pragmatic improvement

V5 had a single 250+ line document with all states inline. V6 puts each state in its own file: `S3E-ego-shock.md`, `S6E-enthusiastic-overuse.md`, and so on.

**Gain:** If you want to read about S3E, you read one focused file. Easier to link to. Easier to update one state without touching the rest.

**Loss:** You can no longer see the full model on one screen. The detailed architecture is distributed across files. V6 has a Mermaid diagram (`02-state-graph.md`) that provides the overview, but the connections between states are no longer visible in a single document.

**Net:** The gain outweighs the loss. Most use cases are "I need to understand one state better," not "I need the whole model at once." The diagram covers the overview.

**Fix:** In Model6.md, add a link to the state graph immediately below the first paragraph: *"For the full state graph and transitions, see [State Graph](02-state-graph.md)."* Make it impossible to miss.

---

### 14. New top-level guides are essential, not padding — improvement

V6 added three new files:
- **`healthiness.md`** — which states are sustainable, which are corrosive, which are transitional. Explicitly marked as interpretation, not a model claim.
- **`usage.md`** — what the model can and cannot be used for. Concrete use cases and hard limits.
- **`observation-guide.md`** — behavioral markers for identifying states in practice. What to watch and what to ask.

V5 had none of these. The model was silent on how to use it.

These three files fill a real gap. A practitioner reading V6 now knows whether a state is healthy to stay in, whether the model supports diagnosis or prediction, and how to identify a state in a real person.

**Fix:** None. These are well-written and needed. Extend them: in each state file, link to the relevant section of observation-guide.md. In healthiness.md, link each claim to the state file that supports it.

---

## Recommendations

### Priority 1 — needed for V7

1. **Audit per-domain scoping for consistency.** Every state file should clarify whether claims apply per-domain or globally. Add a standard note to each state file per Finding 9.

2. **Remove or move the direct S3E → S5 edge.** It cannot be distinguished from fast S3B in a single observation. Move it to the open questions section and mark it as a guess pending data from a study that follows people over time. See Finding 6.

3. **Upgrade the PEN vs S2D diagnostic.** Add a testable distinction: *"Does the position hold if the concern is addressed?"* Point toward a future study design. See Finding 8.

4. **Add a tighter rule to Related Literature.** A concept must be the most direct explanation available — not just vocabulary from somewhere adjacent in the literature. See Finding 1.

---

### Priority 2 — usability

5. **Add per-state observation links.** In each state file, link to the corresponding section of observation-guide.md.

6. **Clarify S6D vs S6R in the state graph.** "Dependent" → D and "pressure-Driven" → R is correct, but a reader skimming the graph could misread S6D as "Driven." Add a footnote or legend entry.

7. **Link to the state graph from Model6.md.** Make the Mermaid diagram unavoidable on first read, not buried in file 2.

---

### Priority 3 — forward work

8. **Design the study to test S2T vs S2D and S3B vs S7M.** These are the two key transitions that cannot currently be distinguished without following people over time. The S3E → S3X threshold is the other priority. Budget: roughly $80–150k for 200 people over 18 months, with monthly check-ins.

9. **Validate PEN with cross-domain data.** A person whose refusal is genuinely values-grounded should decline AI use even in low-stakes domains where their identity is not on the line. A mixed S2D+values case will show inconsistency across domains. Testable in a 3-month study, roughly $20k.

10. **Stress-test the healthiness interpretation with practitioners.** Which healthiness claims match what people in the field actually see, and which don't? Iterate from there.

---

## What V5 should have fixed but didn't

1. **Time estimates for how long S3E lasts.** V5 said "six or more months unresolved is a sign of clinical distress." V6 keeps this number but admits it was never measured. The direction is probably right. The number is a guess. A future study should test this threshold.

2. **Whether S5 Understanding actually needs two things at once.** Both V5 and V6 claim S5 requires internal reframing plus social normalization happening together. Both call it a guess. A study should test whether both are actually required or whether one dominates.

3. **The "most people cycle through more than once" claim.** V5 called it qualitative; V6 still quotes it without new data. A study where you follow the same people over time would confirm or disprove this quickly.

---

## What V6 changed that should probably be reversed in V7

1. **The descriptive-first declaration, if the text doesn't change to match.** As written, it is an attitude statement without substance-level follow-through. Either revert it as redundant, or actually remove the causal vocabulary from the state files — which would require rewriting most of them.

2. **The direct S3E → S5 edge.** It is unobservable in a single session, it removes pressure to model S3B properly, and it adds an escape hatch the model doesn't need. Move it to open questions.

3. **Related literature as currently framed.** The disclaimer does not prevent vague resemblances from accumulating in the model over time. Tighten the rule, or revert to V5's "mechanism anchor" language and explicitly defend the causal claims.
