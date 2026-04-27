# Slice 07 — Structural Displacement Branch (S3X)

Covers source item **19**: add Option 3 from [3-Answers-Model5.md](../../Questions/3-Answers-Model5.md) section A.3.1 — a Structural Displacement state between S3E Ego Shock and dropout for people whose economic position is non-viable.

## What the source asks for

Add one new state — **S3X Structural Displacement** — and connect it properly to the state graph. This is Option 3 from the economic-dependence analysis, chosen over the companion-model and the viability-modulator approaches.

## Why S3X and not a modulator

The modulator approach (add "economic viability" as a third axis) was Option 2. Option 3 (a new state) was chosen because:

- A person in S3X has qualitatively different psychological needs from a person in S3E Ego Shock. The interventions are different. A distinct state makes that explicit.
- The modulator approach would make the model's behavior conditional on an external economic fact that may not be known to the person or the practitioner. A state that the person *enters* when they conclude their position is non-viable is psychologically cleaner.
- States are cheap to add at a transition point; they are expensive to add inside the main body of the graph. S3X sits at the edge (between S3E and exit) without disrupting the core arc.

## State definition

### S3X — Structural Displacement

> "My job is not being disrupted. My job is being replaced."

A state reached when a person in S3E Ego Shock concludes — or is confronted with the reality — that viable AI-collaborative work no longer exists in their domain. The problem is no longer psychological (can I adapt?) but structural (is there a position to adapt *to*?).

**What distinguishes S3X from S3E Ego Shock:**

S3E Ego Shock asks *if AI can do this, what does that make me?* — an identity question. S3X has moved past that question to a different one: *the answer to that question is that my economic position is gone, and now what?*

The identity crisis is not resolved in S3X. It is joined by an economic crisis. The two reinforce each other, which is what makes S3X distinct from a dropout event.

**Entry condition:**

Not a transition that all S3E people reach. It requires one of:

- External confirmation of economic non-viability (role is being eliminated, clients are no longer paying for human work in this domain).
- Internal conclusion reached by the person after sustained S3B Bargaining has failed to produce a stable position.
- A capability jump that makes the person's remaining domain too small to constitute a viable livelihood.

**Related literature:**

Conceptually related to **occupational identity disruption** in the job displacement literature — the documented difficulty of professional transition when the identity invested in a role is lost alongside the economic role itself. Not the same as voluntary career change, where identity is more often preserved through the transition.

**Three resolutions from S3X:**

```markdown
### Transitions out of S3X

- → **Occupational transition:** The person's skills transfer to adjacent work — a translator becomes an AI output editor, a paralegal moves into legal strategy that AI cannot replicate. This is S7M Maturity in a new domain — the person enters a new instance of the model at S0 Baseline or S1 Initial Encounter for the new domain. The psychological work of transitioning identity is real and the model applies again from the start in the new domain.

- → **Principled exit from knowledge work:** The person does not transition to an adjacent role but leaves the field entirely. This is a legitimate resolution, not a failure. The model does not prescribe outcomes. Some people exit, remain productive in other ways, and carry no unresolved S3X dynamics.

- → **Adversarial advocacy:** The person becomes an activist for regulation, labor protection, economic redistribution, or other forms of resistance to AI displacement. This is a stable non-adoption position with external advocacy attached. It is structurally outside the integration cycle. It is *not* S7V Evangelism (which is integration-side advocacy); it belongs to a different track the model does not currently describe in full. V6 acknowledges this track exists and leaves it for future development.
```

**What S3X is not:**

- Not emotional dropout. Emotional dropout happens at any state when the psychological cost exceeds what the person is willing to pay. S3X is about structural non-viability, not insufficient willingness to continue.
- Not S3B Bargaining. Bargaining is available when there is something to bargain around — a residual domain to protect. S3X is reached when that domain is gone.
- Not S7B Burnout. Burnout follows high engagement; S3X can be reached without significant prior engagement.

**Healthiness:**

S3X is a legitimate position, not a pathology. The model should not imply people in S3X have failed or should have adapted better. The state reflects a structural fact about the labor market. The psychological work in S3X is: accepting the structural reality, grieving the role if needed, and finding where to direct energy and identity next.

## State graph update

In `02-state-graph.md` and the mermaid diagram, add:

```
S3E -->|economic non-viability| S3X
S3X -->|occupational transition| S0
S3X -->|principled exit| Dropout
S3X -->|adversarial advocacy| AdversarialAdvocacy
```

The adversarial advocacy track can be represented as a labeled dropout variant or as a named state — the implementer should decide based on whether there is enough content to justify a named state. A labeled dropout is the minimal approach.

## File to create

`states/S3X-structural-displacement.md` using the standard state-file template from slice 01.

## Addition to populations.md

A note cross-referencing S3X belongs in `populations.md` under an "Economic Displacement" section:

```markdown
## Economic Displacement (S3X)

The model assumes viable human-AI collaborative work exists in the person's domain. This assumption is false for a growing population of workers. For these users, the standard arc (S3E Ego Shock → S3B Bargaining → S5 Understanding → S7M Maturity) is not available — not because the person is unwilling to adapt, but because there is no role to adapt into.

S3X Structural Displacement is the model's acknowledgment that this population exists. See `states/S3X-structural-displacement.md`.

The model explicitly does **not** claim to predict which roles will become economically non-viable, or when. That is an economics question. The model describes what happens psychologically when someone concludes their role is non-viable.

One additional commitment V6 makes that V5 did not: the states S7M Maturity, S7I Identity Expansion, and S7V Evangelism all assume viable human-AI collaborative work exists in the person's domain. This is now stated explicitly. The optimistic end states are not available to everyone; the model should not be read as promising they are.
```

## Verification checklist

- [ ] `states/S3X-structural-displacement.md` exists with all standard sections.
- [ ] S3E Ego Shock file has the outbound edge to S3X with the entry condition.
- [ ] Mermaid diagram includes S3X.
- [ ] `populations.md` has the Economic Displacement section.
- [ ] S7M Maturity, S7I Identity Expansion, S7V Evangelism descriptions note the viable-domain assumption explicitly.
- [ ] Adversarial advocacy is labeled clearly as a named track the model does not fully describe yet.
