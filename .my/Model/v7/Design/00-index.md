# V7 Design — Index

This folder holds the design documents for Version 7 of the AI Psychological Adaptation model. It is a **design set**, not the finished model. The files here specify what V7 should be, what has to be decided before it can be written, how it could be tested, and how it would be used.

V7 is a response to three pressures:

1. **The identifier scheme has failed.** V6's `S0`–`S7` numbering carries an ordinal reading the model explicitly disclaims, contains a gap at `S4`, groups states into families that do not share structure, and has been renumbered twice already. Every proposed fix that keeps numbers requires another renumbering. See [02-identifiers.md](02-identifiers.md).
2. **Eighteen states is too many.** Four of them differ only by motive, three of them differ only by style. The V6 discussion documents concluded these should collapse into states carrying attributes. V7 implements that.
3. **The environment moved.** V6 was written against a world of turn-by-turn assistants. Long-horizon autonomous agents, mandated workplace adoption, and verification-dominant workflows change which parts of the model carry weight. See [07-environment-shift.md](07-environment-shift.md).

## Reading order

**Start here if the goal is to understand the model:**

| File | Contents |
| --- | --- |
| [01-model-v7.md](01-model-v7.md) | What the model is, what it claims, scope, epistemic stance, and the resolved descriptive-versus-prescriptive question |
| [02-identifiers.md](02-identifiers.md) | The new identifier scheme, why numbers were dropped, and the full V6 → V7 translation table |
| [03-axes.md](03-axes.md) | Identity Stakes, Delegation Level (D1–D5), Delegation Ceiling, Verification Burden |
| [04-state-graph.md](04-state-graph.md) | The graph, the five families, occupancy and coexistence rules |
| [05-states-early.md](05-states-early.md) | Pre-engagement, Stance, and Disruption families |
| [06-states-working.md](06-states-working.md) | Working and Exit families, plus the Advocacy overlay |
| [07-environment-shift.md](07-environment-shift.md) | What changed between V6 and V7 in the AI environment, and which model parts it affects |

**Start here if the goal is to move the project forward:**

| File | Contents |
| --- | --- |
| [10-decisions.md](10-decisions.md) | Every open decision, each with options as a task list and a recommended option already marked |
| [20-testing.md](20-testing.md) | How to test the model — instruments, study designs, falsifiers, and a staged validation programme |
| [30-practitioner-use.md](30-practitioner-use.md) | How practitioners can actually use the model, with protocols, worked examples, and misuse limits |

## Status of the material in this folder

Everything in this folder inherits V6's epistemic position: the model is a **speculative conceptual framework**. Nothing has been empirically validated. The state descriptions are written concretely so that they can be argued with and tested, not because they are established.

Three markers appear throughout:

- **(no marker)** — a well-grounded but unvalidated hypothesis, or a pattern with reasonable support in adjacent literature.
- **Conjecture —** a claim made because it is a useful frame, not because it has been observed.
- **Testable —** a claim with a defined study that could confirm or refute it.

A fourth marker appears in V7 for material introduced from the post-V6 environment:

- **New in V7 —** a construct that did not exist in V6 and has had no review cycle at all. These are the least settled parts of the model.

## What V7 does not change

The substantive psychology is preserved. Identity threat under capability replication, defensive evaluation, shock, scope negotiation, calibrated use, overuse, and integration all survive intact. A reader who knows V6 will recognise every pattern. What changes is how the patterns are named, how many separate names they need, and which axes modulate them.
