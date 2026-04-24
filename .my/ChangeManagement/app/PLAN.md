# Plan: AI Adoption Scorecard — Interactive HTML App

## Goal

A single-page HTML application that lets users answer the 21 scorecard statements (randomised) plus 2 bonus questions, then shows their AI adoption phase results. Supports both individual and team perspectives in both Dutch and English.

---

## Architecture

### Single file: `index.html`

No build tools, no dependencies, no frameworks. One self-contained HTML file with embedded CSS and JavaScript. Can be opened directly from the filesystem or hosted anywhere.

### Why single file?

- Zero deployment friction — share as an attachment, open locally, or drop on any static host
- No CORS issues, no API calls, no cookies, no tracking
- All data stays in the browser — nothing is sent anywhere

---

## Data Model

### Four question sets (mode × language)

Each mode+language combination has:
- **21 main statements** in 7 blocks (A–G), 3 per block
- **2 bonus statements** (emotional vs practical)
- **7 phase result descriptions** (one per block)
- **Bonus interpretation text**

The blocks map to phases:
| Block | EN Phase | NL Phase |
|-------|----------|----------|
| A | Dismissal | Afwijzing |
| B | Resistance | Weerstand |
| C | The Hit (Ego Shock) | De klap |
| D | The Deal (Bargaining) | De deal |
| E | Building Trust | Vertrouwen opbouwen |
| F | Understanding & Overcompensation | Begrip en overcompensatie |
| G | Stabilisation | Stabilisatie |

### Data structure (JS object)

```javascript
const DATA = {
  en: {
    individual: {
      title: "Where do you stand with AI?",
      subtitle: "A personal scorecard",
      intro: "...",
      scoreLabels: ["No, doesn't apply to me", "Somewhat / sometimes", "Yes, that's me right now"],
      statements: [
        { id: 1, block: "A", text: "I don't really see how AI is relevant to my work." },
        { id: 2, block: "A", text: "When AI comes up in conversation, I don't have much to contribute." },
        // ... all 21
      ],
      bonus: {
        intro: "Two more statements...",
        a: { text: "My hesitation about AI is mainly about what it means for my role and identity." },
        b: { text: "My hesitation about AI is mainly about the quality and usability of the tools." },
        interpretations: { aHigher: "...", bHigher: "...", equal: "..." }
      },
      results: {
        A: { phase: "Dismissal", tagline: "AI isn't relevant to me", description: "...", helpText: "..." },
        // ... all 7
      },
      interpretationNotes: "..."
    },
    team: { /* same structure, team-observer statements */ }
  },
  nl: {
    individual: { /* Dutch individual statements */ },
    team: { /* Dutch team statements */ }
  }
};
```

---

## User Flow

```
┌─────────────────────────────────────┐
│  START SCREEN                       │
│                                     │
│  ┌──────────┐  ┌──────────┐        │
│  │ Personal │  │   Team   │        │
│  └──────────┘  └──────────┘        │
│                                     │
│  ┌────┐  ┌────┐                    │
│  │ EN │  │ NL │                    │
│  └────┘  └────┘                    │
│                                     │
│        [ Start → ]                  │
└──────────────────────────────────────┘
              │
              ▼
┌─────────────────────────────────────┐
│  QUESTIONS (one at a time)          │
│                                     │
│  Statement 3 of 21                  │
│  ━━━━━━━━━━━━━░░░░░░ progress bar   │
│                                     │
│  "I've tried AI and it mostly       │
│   disappoints."                     │
│                                     │
│  ○ No, doesn't apply to me    (0)  │
│  ○ Somewhat / sometimes       (1)  │
│  ○ Yes, that's me right now   (2)  │
│                                     │
│  [ ← Back ]          [ Next → ]    │
└──────────────────────────────────────┘
              │ (after Q21)
              ▼
┌─────────────────────────────────────┐
│  BONUS QUESTIONS                    │
│                                     │
│  "Two final statements..."         │
│                                     │
│  [a] emotional statement  ○ 0 1 2  │
│  [b] practical statement  ○ 0 1 2  │
│                                     │
│       [ See results → ]            │
└──────────────────────────────────────┘
              │
              ▼
┌─────────────────────────────────────┐
│  RESULTS                           │
│                                     │
│  Your dominant phase:               │
│  ┌─────────────────────────────┐   │
│  │ THE DEAL (BARGAINING)       │   │
│  │ "Only for X"                │   │
│  │ Description text...         │   │
│  └─────────────────────────────┘   │
│                                     │
│  Phase scores:                      │
│  A ██░░░░ 2/6  Dismissal           │
│  B ████░░ 4/6  Resistance           │
│  C ███░░░ 3/6  The Hit              │
│  D █████░ 5/6  The Deal       ← ★  │
│  E ████░░ 4/6  Building Trust       │
│  F ██░░░░ 2/6  Overcompensation     │
│  G █░░░░░ 1/6  Stabilisation        │
│                                     │
│  Bonus: Your hesitation is mainly   │
│  emotional / practical / both       │
│                                     │
│  [Interpretation notes]             │
│  [ Start over ]                     │
└──────────────────────────────────────┘
```

---

## Feature Specification

### Start screen
- Two toggle choices: Individual / Team, EN / NL
- Both default to Individual + EN (or detect browser language for NL)
- Brief intro text adapts to selected mode+language
- Single "Start" button

### Question screen
- Shows **one statement at a time** (not all 21 on one page)
- Questions are **randomised on start** — shuffle the 21 statements (tracking block membership internally)
- Progress bar: "Statement X of 21"
- Three radio buttons for 0 / 1 / 2 with labels
- Back button (navigate to previous question, answer preserved)
- Next button (enabled only after selecting an answer)
- Keyboard support: 1/2/3 keys for quick scoring, Enter for next
- Answers stored in a JS array, no persistence beyond the session

### Bonus screen
- After Q21, a separate screen for the 2 bonus statements
- Both shown on the same screen (not one-at-a-time)
- Same 0/1/2 scoring

### Results screen
- **Dominant phase** highlighted at top with phase name, tagline, and description
- **Bar chart** showing all 7 block scores (horizontal bars, CSS-only, no chart library)
- Highest bar visually marked (star, highlight, or bold)
- **Tied phases**: if two blocks share the highest score, show both with a "you're in transition" note
- **Bonus result**: emotional / practical / both — with interpretation text
- **Interpretation notes** at bottom (from the scorecard content)
- "Start over" button → back to start screen, all state cleared

### Team-mode extras
- After each block of 3 questions (NOT after each question), ask the spread question: "1-2 people / part of the team / majority"
  - Implementation: after questions 3, 6, 9, 12, 15, 18, 21 in the ORIGINAL block order — but since questions are randomised, track when all 3 questions from a block are answered and show the spread question then
  - Simpler approach: show spread questions on the results screen instead, as a post-scoring reflection
  - **Decision: show spread questions on results screen.** This avoids breaking the randomised flow and keeps the question phase simple.
- Results show spread selector per phase alongside the bar chart

---

## Visual Design

### Principles
- Clean, minimal, professional — matches the tone of the playbook (reliable, driven)
- Mobile-first responsive (people will use this on phones during workshops)
- No images, no icons (except maybe a simple ★ for the dominant phase)
- Colour palette: neutral greys + one accent colour for the dominant phase highlight
- Typography: system font stack (`-apple-system, BlinkMacSystemFont, "Segoe UI", ...`)
- Smooth transitions between screens (CSS transitions, not JavaScript animations)

### Layout
- Max-width container (640px) centred on page
- Generous whitespace
- Large touch targets for radio buttons (full-width clickable rows)
- Progress bar: thin, coloured, top of question area

### Colour usage
- Phase bars: a single muted colour, dominant phase bar in accent colour
- Bonus result: subtle background tint (warm for emotional, cool for practical)

---

## Technical Implementation

### Structure

```
index.html
├── <style> — All CSS inline
├── <div id="app">
│   ├── <div id="screen-start">
│   ├── <div id="screen-question">
│   ├── <div id="screen-bonus">
│   └── <div id="screen-results">
└── <script> — All JS inline
    ├── DATA object (all 4 question sets)
    ├── State management (current screen, answers, mode, language)
    ├── Shuffle function (Fisher-Yates)
    ├── Screen render functions
    ├── Score calculation
    └── Event handlers
```

### Key functions

```
init()              — Set up event listeners, show start screen
startQuiz(mode, lang) — Load question set, shuffle, reset state
showQuestion(index) — Render one statement with radio buttons
nextQuestion()      — Save answer, advance or go to bonus
prevQuestion()      — Navigate back
showBonus()         — Render bonus questions
showResults()       — Calculate scores, render results screen
calculateScores()   — Sum answers per block, find dominant phase
shuffle(array)      — Fisher-Yates randomisation
switchScreen(id)    — Show one screen, hide others
```

### State

```javascript
let state = {
  mode: 'individual',    // 'individual' | 'team'
  lang: 'en',            // 'en' | 'nl'
  questions: [],          // shuffled array of {id, block, text, originalIndex}
  answers: {},            // { questionId: score }
  bonusA: null,           // 0, 1, or 2
  bonusB: null,           // 0, 1, or 2
  currentIndex: 0,        // which question we're showing
  spread: {}              // team mode: { A: '1-2' | 'part' | 'majority', ... }
};
```

### Accessibility
- Semantic HTML: `<fieldset>`, `<legend>`, `<label>` for radio groups
- `role="progressbar"` with `aria-valuenow`
- Focus management on screen transitions
- Keyboard navigation (1/2/3 for scoring, Enter for next, Backspace for back)
- Sufficient colour contrast (WCAG AA)
- `lang` attribute updated on language switch

### No external dependencies
- No jQuery, no React, no chart.js
- Bar chart: CSS flexbox + percentage widths
- Transitions: CSS `transition` property
- Shuffle: Fisher-Yates in ~5 lines

---

## File Size Estimate

| Component | Estimate |
|-----------|---------|
| HTML structure | ~2 KB |
| CSS | ~4 KB |
| JavaScript logic | ~6 KB |
| Data (4 question sets × 21 + results + bonus) | ~15 KB |
| **Total** | **~27 KB** |

---

## What's NOT in scope

- No data persistence (localStorage, cookies, or server)
- No PDF/print export
- No sharing/social features
- No analytics or tracking
- No user accounts
- No animated charts (CSS bars only)
- No playbook content inline (links to .md files in results text are fine but won't work as clickable links in a standalone HTML — replace with "see the playbook for more" without href)

---

## Build Order

1. **Data layer** — All 4 question sets as JS objects (extract from scorecard .md files)
2. **Start screen** — Mode + language selection, start button
3. **Question screen** — One-at-a-time with shuffle, progress bar, back/next
4. **Bonus screen** — Two statements on one screen
5. **Results screen** — Score calculation, bar chart, dominant phase, bonus interpretation
6. **Team extras** — Spread selectors on results screen
7. **Polish** — Responsive, keyboard, accessibility, transitions
