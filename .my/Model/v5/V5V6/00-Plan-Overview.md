# V5 → V6 Implementation Plan — Overview

This folder holds the implementation plan for moving Model V5 to Model V6. The source request is in [1. Update from V5 to V65.md](1.%20Update%20from%20V5%20to%20V65.md). This document is the index. Each numbered file below covers one slice of the work.

V6 lives in a new folder per the model versioning rule: `.my/Model/v6/`. The V5 folder stays frozen.

## Headline framing of V6

V6 is a **descriptive-first** rewrite of V5. The substantive shape of the model (states, axes, transitions) is preserved. What changes:

- The model declares itself descriptive, not predictive. Testability is signposted but not claimed.
- Mechanism anchors become *Related literature* — conceptual connections, not causal claims.
- Scope is stated explicitly at the top. Out-of-scope populations are listed.
- Healthiness, usage, and meaning sections are added so the reader knows what the model is *for* before reading the states.
- Three structural additions: the S2T → S2D edge, the direct S3E → S5 edge, a Structural Displacement branch (S3X), and a pre-emptive ethical rejection path.
- State coexistence rules are spelled out instead of left implicit.
- Identity-domain scoping is made explicit: defensive evaluation only fires inside identity-threatened domains.
- Grief language is removed from S3E.
- Files are split. Each state gets its own file. Diagrams move to mermaid.

V6 does **not** add a numerical intensity formula, transition probabilities, or empirical validation. Those remain explicitly out of scope.

## Planned V6 folder structure

```
.my/Model/v6/
├── Model6.md                       — entry point: scope, axes, meaning, reading guide, healthiness, usage
├── 00-relationship-to-prior.md     — V4/V5 lineage and what changed
├── 01-axes.md                      — Identity Stakes, Task Delegation Level, Delegation Ceiling
├── 02-state-graph.md               — full state graph (mermaid), occupancy rules, transition rules
├── states/
│   ├── S0-baseline.md
│   ├── S1-initial-encounter.md
│   ├── S2T-trust-evaluation.md
│   ├── S2D-defensive-resistance.md
│   ├── S3E-ego-shock.md
│   ├── S3B-bargaining.md
│   ├── S3X-structural-displacement.md   — new in V6
│   ├── S5-understanding.md
│   ├── S6E-enthusiastic-overuse.md
│   ├── S6D-dependent-overuse.md
│   ├── S6R-driven-overuse.md
│   ├── S6S-social-overuse.md
│   ├── S7M-maturity.md
│   ├── S7I-identity-expansion.md
│   ├── S7E-ethical-integration.md
│   ├── S7B-burnout.md
│   ├── S7V-evangelism.md
│   └── PEN-pre-emptive-non-adoption.md  — new in V6
├── triggers.md                     — external trigger layer, ⚡ rules
├── social-context.md               — ambient field
├── dropout.md                      — two-axis dropout
├── populations.md                  — scope, AI-native pathway, non-knowledge work, accessibility, economic dependence
├── healthiness.md                  — global healthiness frame and per-state mapping
├── usage.md                        — what the model is for, what it cannot (yet) be used for
├── observation-guide.md            — concrete behavioral markers per state, S6 in particular
└── limits-of-operationalization.md — what is testable, longitudinal-only, conjecture
```

The file split is for editor and reader convenience, not for size reasons. Each state file is short (one screen each).

## Implementation slices (one per file in this folder)

| File | Covers source items | Purpose |
| ---- | ------------------- | ------- |
| [01-file-structure-and-diagrams.md](01-file-structure-and-diagrams.md) | 1, 1b | Split layout, mermaid diagrams |
| [02-state-graph-changes.md](02-state-graph-changes.md) | 2, 4, 5 | S2T→S2D edge, S3E→S5 edge, occupancy rules |
| [03-mechanism-anchors-reframe.md](03-mechanism-anchors-reframe.md) | 6, 12 | Rename to "Related literature", diagnostic disclaimer |
| [04-triggers-and-cycling.md](04-triggers-and-cycling.md) | 7, 8, 9 | ⚡ adjustments, cycling drivers, evangelist claim |
| [05-identity-domain-scoping.md](05-identity-domain-scoping.md) | 10, 18 | Defensiveness scope, S3B vs S7M rewrite |
| [06-scope-and-populations.md](06-scope-and-populations.md) | 13 | Scope statement, AI-native, non-knowledge, accessibility, delegation ceiling |
| [07-structural-displacement.md](07-structural-displacement.md) | 19 | New S3X branch |
| [08-pre-emptive-ethical-rejection.md](08-pre-emptive-ethical-rejection.md) | 20 | New path from S1 |
| [09-front-matter-and-meaning.md](09-front-matter-and-meaning.md) | 11, 14a, 14b, 14d, 14e, 14g, 15, 16, 17 (usage) | Scope-first framing, "What does the model mean", related-literature citations, descriptive-only stance, healthiness, usage |
| [10-state-descriptions-and-cleanup.md](10-state-descriptions-and-cleanup.md) | 14c, 14f, 17 (state descriptions) | S6 observation guide, grief language strip, per-state description updates from 1-Answers |

Each slice document follows the same shape:

1. **What the source asks for** — one-line restatement.
2. **Concrete change** — what gets added, renamed, moved, or deleted, in which file.
3. **Exact wording** — proposed text where it is short enough to include.
4. **Risks / open questions** — flagged where the change has knock-on effects.

## Ordering of implementation

Implementation should follow the order below. Earlier slices set up structure that later slices fill in.

1. Slice 01 — create the V6 folder structure, copy V5 content into the new files unchanged, convert ASCII diagrams to mermaid.
2. Slice 09 — add the front-matter sections (scope, meaning, related-literature framing, descriptive-only stance, healthiness, usage). This sets the tone before any state changes are made.
3. Slice 03 — rename mechanism anchors to "Related literature" globally and add the diagnostic disclaimer. Touches every state file but is mechanical.
4. Slice 02 — apply state-graph changes (edges, occupancy).
5. Slice 04 — apply trigger and cycling adjustments.
6. Slice 05 — rewrite S3B vs S7M and tighten defensiveness scope.
7. Slice 10 — apply per-state description updates, observation guide, grief language strip.
8. Slice 06 — add scope statement and populations file.
9. Slice 07 — add S3X Structural Displacement.
10. Slice 08 — add the pre-emptive non-adoption path.

This ordering puts cosmetic and structural changes first, then content rewrites, then additions. It minimises rework: the additions land into a model that already has the right framing.

## Out of scope for V6

For clarity, things explicitly **not** done in V6:

- No transition probabilities or dwell times.
- No empirical validation of any claim.
- No Adoption Ceiling as originally proposed (delegation ceiling per person is added; population-wide ceiling is not).
- No reframe around economic viability as the lead question. That waits for V7 or later, conditional on need.
- No companion model. Economic displacement is added to V6 as a branch (S3X), not as a separate document.

## Cross-document references

Many slices reference content already in the answer documents:

- [1-Answers-Model5.md](../../Questions/1-Answers-Model5.md) — healthiness mapping, state interpretations.
- [3-Answers-Model5.md](../../Questions/3-Answers-Model5.md) — S3B vs S7M, S3X structural displacement, pre-emptive ethical rejection.
- The 12 reviews under [.my/Reviews/v5/](../../Reviews/v5/) — source for many of the 20 items.

Slice documents quote or paraphrase from these as needed. They do not require the implementer to re-derive any of that material.
