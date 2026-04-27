# Earn-Its-Keep Audit — Plain-Language Version

This is a simpler rewrite of [011-earn-its-keep.md](011-earn-its-keep.md). Same findings, plain language. If you've read the original and it landed, skip this one.

## What this audit asks

For every piece of model V5 — every state, axis, and claim — ask three questions:

- **Explanatory power:** does it tell you something useful about why people behave the way they do?
- **Operational use:** can a practitioner actually use it? Can you spot it in real life?
- **Falsifiability:** could you describe a result that would prove it wrong?

If a piece fails all three, it's dead weight. Cut it. If it passes most but not all, weaken the claim so it doesn't pretend to be more than it is.

## TL;DR

- **Cut S0 Baseline** (the "Baseline" state, before anyone has met AI). It has no explanatory power, no practical use, and no way to be wrong. The model starts cleaner at S1 Initial Encounter.
- **Weaken** the claim that S3B Bargaining and S7A Maturity are different (both look like "I use AI for some things but not others"). The model itself admits this is a guess that needs years of follow-up to test.
- **Cut** the Cultural Variability section. The model literally says no cross-cultural data has been gathered.
- **Weaken** three other claims that are flagged as guesses inside the model but not flagged clearly enough in the main text.
- **Keep** all 16 core states and all the structural pieces (the two axes, the dropout map, the reversibility test, and so on). They earn their keep.
- Net effect: delete 1 state, delete or weaken 4 claims, simplify 1 heuristic. V6 will be **leaner** and more honest about what it does and doesn't know.

## Audit table

| Construct | Explanatory Power | Operational Use | Falsifiability | Verdict |
|-----------|-------------------|-----------------|-----------------|---------|
| S0 Baseline (Baseline) | N | N | N | **DELETE** |
| S1 Initial Encounter (Initial Encounter) | Y | Y | Y | KEEP |
| S2T Trust Evaluation (Trust Evaluation) | Y | Y | Y | KEEP |
| S2D Defensive Resistance (Defensive Resistance) | Y | Y | Y | KEEP |
| S3 Ego Shock (Ego Shock) | Y | Y | Y | KEEP |
| S3B Bargaining (Bargaining) | Y | Y | Partial | KEEP / WEAKEN |
| S5 Understanding (Understanding) | Y | Y | Partial | KEEP / WEAKEN |
| S6A Enthusiastic Overuse–D (Overuse variants) | Y | Y | Y | KEEP |
| S7A Maturity (Maturity) | Y | Y | Y | KEEP |
| S7B Identity Expansion (Identity Expansion) | Y | Y | Y | KEEP |
| S7C Ethical Integration (Ethical Integration) | Y | Y | Partial | KEEP / WEAKEN |
| S7D Burnout (Burnout/Withdrawal) | Y | Y | Y | KEEP |
| S7F Evangelism (Influence/Evangelism) | Y | Y | Partial | KEEP / WEAKEN |
| Identity Stakes Axis | Y | Y | Y | KEEP |
| Task Delegation Level (D1–D4) | Y | Y | Partial | KEEP |
| Practical × Emotional Dropout Plane | Y | Y | Y | KEEP |
| Reversibility Test | Y | Y | Y | KEEP |
| ⚡ Marker Convention | Y | Y | Y | KEEP |
| Limits of Operationalization | Y | Y | Y | KEEP |
| Regression / Loop Property | Y | Y | Y | KEEP |
| External Trigger Layer | Y | Y | Y | KEEP |
| Social Context Layer | Y | Y | Y | KEEP |
| Cultural Variability Section | N | N | Y (principle only) | **DELETE** |
| S5 Understanding Dual-Component Claim | Partial | Partial | N | **WEAKEN** |
| S3B Bargaining/S7A Maturity Heuristic Distinction | Partial | Y | N | **WEAKEN** |
| S7F Evangelism S3 Ego Shock-Prerequisite Claim | Partial | Partial | N | **WEAKEN** |
| D1–D4 Categorical Boundaries | Y | Y | Partial | **WEAKEN** |
| "Most People Cycle Multiple Times" | Partial | Partial | N | **WEAKEN** |

## Findings

### Keep (16 core constructs)

1. **S1 Initial Encounter.** The first time someone meets AI seriously. How big the stakes feel for their identity decides which path they take from here. Falsifiable.

2. **S2T Trust Evaluation.** The person tests AI fairly to see how good it is. This is different from S2D Defensive Resistance (defensive evaluation) and the difference matters for how you'd help them.

3. **S2D Defensive Resistance.** The person evaluates AI through the lens of *this thing threatens who I am*, so they latch onto every flaw and ignore every strength. The fix is not to give them more evidence — it's to acknowledge the threat first.

4. **S3 Ego Shock.** The crash. Self-efficacy (the feeling that you're good at your job) collapses, and existential worry kicks in. The table that crosses identity stakes with task delegation level explains a lot.

5. **S6A Enthusiastic Overuse.** Compulsive AI use driven by the same mechanism as a slot machine: you don't know what you'll get, and that uncertainty is what hooks you. Different driver from the other S6 flavors.

6. **S6B Dependent Overuse.** Confidence in AI replaces confidence in self. The fix has to rebuild the person's own judgment alongside their AI use, not just curb the AI use.

7. **S6C Driven Overuse.** The person isn't excited about AI; they're under pressure (deadlines, quota, fear of being slow). The fix is structural — change the pressure — not feedback about the tool.

8. **S6D Social Overuse.** The person uses AI heavily because their peer group does. Classic group-conformity research (Asch's line experiments from the 1950s, where people gave wrong answers to match the group). Explains why the same person uses AI very differently in different teams.

9. **S7A Maturity.** Calm, calibrated AI use. The person knows when AI helps and when it doesn't, and adjusts.

10. **S7B Identity Expansion.** "I'm a carpenter who uses a hammer; I'm a photographer who uses a camera." The person folds AI into their sense of who they are and what they can do.

11. **S7C Ethical Integration.** The person uses AI but also keeps thinking about whether and how they should — without freezing up and refusing.

12. **S7D Burnout / Withdrawal.** The person is depleted, not opposed. Looks like dropout but the trajectory tells you which it is.

13. **S7F Evangelism Influence / Evangelism.** The person becomes a guide for others. Explained by Erikson's idea of *generativity* — the midlife drive to help the next group through what you went through.

14. **Both axes.** Identity stakes (how much of *you* is on the line) decides which path you take and how hard it hits. Task delegation level (D1 = "ask AI a question" through D4 = "let AI do the whole job") decides how intense it gets within a given path. Both are observable and testable.

15. **Dropout as a two-axis plane.** Two people can both quit AI and look identical from the outside, but for different reasons (the tool didn't work versus it made them feel bad). Treating dropout as one thing hides this. The reversibility test (offer a tool that fixes the practical complaint and see if they come back) sorts the two cases apart.

16. **The structural pieces.** Mechanism anchors, the Limits section, the trigger and context layers, the regression/loop property, and the ⚡ marker convention. All earn their place.

### Weaken (5 claims)

17. **S3B Bargaining versus S7A Maturity as different states.** Both look like "I use AI for some things but not others." The model claims they're different underneath (S3B Bargaining is anxious bargaining, S7A Maturity is calm calibration). But the model itself admits: "This is a heuristic, not a measured fact. Requires longitudinal observation across multiple model releases, and is contaminated by self-report once a subject has read this model." That's a long way of saying *we can't actually test this yet*. Move it out of the main text and into the Limits section.

18. **S5 Understanding needs both internal and social acceptance.** The model says S5 Understanding (the stable, integrated state) requires both an internal mental shift *and* the people around you treating AI use as normal. The model itself says this is "currently conjecture" with no measurement plan. Action: rewrite the main text to say "Stability appears to involve both internal model coherence and social normalization, but neither is operationalized and the claim is untested."

19. **Stable evangelists were once shaken.** The model says S7F Evangelism evangelists almost always passed through S3 Ego Shock (the panic state) first — that the lived experience is what makes them credible. The model itself flags this as conjecture. Move it from main text to the Limits section as a testable hypothesis: "S3 Ego Shock experience predicts stable S7F Evangelism."

20. **D1–D4 as four sharp categories.** The four delegation levels (ask a question, get a draft, get a finished thing with guidance, hand off entirely) are useful as buckets but the boundaries are intuition, not measurement. Where exactly does "summarize this article" end and "write a report with guidance" begin? Add a note: these are rough qualitative buckets, not precise categories.

21. **"Most people cycle through the model more than once."** The model says it deliberately avoids numerical claims about cycle frequency, but then drops in a frequency claim anyway. Pick a lane. Rewrite to: "People can cycle through the model as AI evolves; V5 makes no claims about how often or how many."

### Delete (2 constructs)

22. **S0 Baseline.** This is the state before the person has had any meaningful contact with AI. It fails all three tests:
    - **No explanatory power.** It's the absence of a state, not a state.
    - **No operational use.** No practitioner sits with a person and asks "are you in S0 Baseline?" — the question is whether they've been triggered into S1 Initial Encounter yet.
    - **No falsifiability.** It's true by definition.

    The model is stronger if it just starts at S1 Initial Encounter. Replace the entry point with: "Triggered by meaningful exposure to AI — a demonstration, a workplace mandate, a peer adopting it, a media story, or a personal experience with the tool."

23. **Cultural Variability section.** The model literally says: "This entire section is currently conjecture. No cross-cultural data has been gathered." That's an explicit admission that nothing in this section has been measured against reality. Move it to the Limits section as a research proposal, not as a load-bearing part of the model.

## Recommendations

1. **Delete S0 Baseline.** Redraw the state diagram so it begins at S1 Initial Encounter. Replace the entry point text with: "Entry: triggered by meaningful exposure to AI — a demonstration, a workplace mandate, peer adoption, a media narrative, or a personal experience."

2. **Reorganize the Limits section** to add a subsection — **Untested but Falsifiable Hypotheses** — and put these in it: the S3B Bargaining-versus-S7A Maturity distinction; the S5 Understanding dual-component claim; the S7F Evangelism-was-once-S3 Ego Shock claim; the cycling-frequency claim; and the cultural variability material (with a proposed five-culture comparison study).

3. **Rewrite the S3B Bargaining section.** Drop the S3B Bargaining-versus-S7A Maturity distinction from the main text. Add a pointer: "See Limits of Operationalization for testability status."

4. **Rewrite S5 Understanding.** Soften the dual-component claim: "Stability appears to involve both an internal mental-model shift and social normalization, but neither is operationalized and the claim is untested."

5. **Rewrite S7F Evangelism.** Drop the S3 Ego Shock-prerequisite claim from the main text: "Most observed S7F Evangelism users have passed through S3 Ego Shock — their lived experience makes them credible guides — but this is untested."

6. **Add a note to D1–D4:** "These are qualitatively distinct buckets, not sharply bounded categories. Treat them as a rough scale."

7. **Delete the Cultural Variability section** from the main model. Move it to Limits as: "**Future research: cross-cultural validation.** Working hypothesis: the basic state structure is the same across cultures; what changes is the intensity and emotional flavor. Proposed test: measure state sequence and time spent in each state across five cultural contexts — high craft-identity, techno-optimistic, collectivist, hierarchical, and economic-anxiety. A finding that would falsify the model: a culture where stable S7A Maturity users routinely jump straight from S0 Baseline to S7A Maturity without going through S1 Initial Encounter."
