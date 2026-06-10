# Studio Kairos Presentation Design System

A design system for creating presentation slides that match the Studio Kairos visual identity, derived from the "Internship Day 3" deck (Leadership & Project Management, 2026).

---

## Design Philosophy

Typography is the design. The slides rely on font weight, size contrast, and a tight color palette — not icons, gradients, or decoration. The tone is warm, direct, and professional. Every slide makes exactly one point.

Core traits:
- ALL CAPS for every heading and section title
- Numbered sections (01, 02, 03...)
- Bold one-liner maxims to close feature slides
- Cream backgrounds for content; near-black backgrounds for covers and transitions
- Orange accent used sparingly — numbers, emphasis phrases, taglines only

---

## Color Palette

| Role | Hex | Description |
|------|-----|-------------|
| Primary Background | `#F5F1E4` | Warm cream — default slide background |
| Secondary Background | `#F1EBE3` | Slightly darker cream — alternate sections |
| Light Tint | `#FFF6F1` | Near-white warm tint — subtle panel fills |
| Dark Background | `#1B1B1B` | Near-black — covers, closings, Q&A slides |
| Primary Text | `#1B1B1B` | Near-black — all body and heading text on light backgrounds |
| Secondary Text | `#363636` | Dark gray — supporting text, column headers |
| Accent | `#FB6636` | Vibrant orange — numbers, maxims, key emphasis |
| On-Dark Text | `#FFFFFF` | White — all text on dark backgrounds |

**Usage rules:**
- Never use `#FB6636` for body text or long-form content
- Never use pure white (`#FFFFFF`) as a slide background — use `#F5F1E4` instead
- Dark slides (`#1B1B1B`) are reserved for cover, closing, Q&A, and dramatic transition moments
- `#363636` is for secondary labels and column headers, not primary content

---

## Typography

### Font Stack

| Font | Weights Used | Role |
|------|-------------|------|
| **Archivo Black** | 900 | Display headlines — cover title, closing, big statements |
| **Raleway** | Bold (700), SemiBold (600), Medium (500) | Section headings, body text, numbered labels |
| **Montserrat** | Bold (700) | Supporting labels, callouts, tags |

Import (Google Fonts):
```
Archivo Black
Raleway: 500, 600, 700
Montserrat: 700
```

### Type Scale

| Level | Font | Weight | Approximate Size | Usage |
|-------|------|--------|-----------------|-------|
| Display | Archivo Black | 900 | 5–8rem | Cover title, closing slide headline |
| H1 | Raleway | Bold | 3–4rem | Main slide heading |
| H2 | Raleway | SemiBold | 2–2.5rem | Section label / numbered prefix |
| H3 | Raleway | SemiBold | 1.5–2rem | Column headers, sub-headings |
| Body | Raleway | Medium | 1–1.25rem | Paragraph text, descriptions |
| Label | Montserrat | Bold | 0.85–1rem | Tags, captions, small labels |
| Maxim | Raleway | SemiBold | 1.1–1.3rem | Closing tagline on a slide |

### Style Rules

- **Headings:** Always ALL CAPS, no exceptions
- **Numbers:** `01.` format, Raleway Bold, accent orange (`#FB6636`)
- **Maxims:** Short imperative sentence (e.g., *"The best leaders serve others first."*) in Raleway SemiBold, smaller than the heading, often in accent orange or `#363636`
- **Body paragraphs:** 2–3 sentences max per slide. Raleway Medium.
- **Letter spacing:** Slightly expanded on display and H1 text (`letter-spacing: 0.05em`)
- **Line height:** 1.15–1.25 for headings; 1.5–1.6 for body

---

## Slide Layout Templates

### A. Cover Slide

**Background:** `#1B1B1B`

```
┌─────────────────────────────────────────┐
│                                         │
│   [YEAR in accent orange, small]        │
│                                         │
│   MAIN HEADLINE                         │
│   SPANNING TWO                          │
│   OR THREE LINES                        │
│   [Archivo Black, white, display size]  │
│                                         │
│   Subtitle or tagline                   │
│   [Raleway Medium, white, small]        │
│                                         │
│   STUDIO NAME | DAY NUMBER              │
│   [Raleway Medium, #363636, xsmall]     │
│                                         │
└─────────────────────────────────────────┘
```

Example — Slide 1:
> `2026` (orange) / `LEADERSHIP &` / `PROJECT MANAGEMENT` (white, Archivo Black) / `LEAD PEOPLE WELL. SHIP PROJECTS ON TIME.` (white, small) / `STUDIO KAIROS | DAY THREE` (gray, xsmall)

---

### B. Section Intro Slide

**Background:** `#1B1B1B` or `#F5F1E4`

```
┌─────────────────────────────────────────┐
│                                         │
│   [Large decorative label — faint,      │
│    e.g. compass letter N/S/E/W]         │
│                                         │
│   SECTION TITLE                         │
│   [Archivo Black, large]                │
│                                         │
│   One-liner context sentence            │
│   [Raleway Medium, body size]           │
│                                         │
└─────────────────────────────────────────┘
```

Example — Compass Section:
> `4 DIRECTIONS. 1 TRUE ESSENCE.` (large, white) / `COMPASS PERSONALITY TEST` (Raleway SemiBold, orange) / compass letters N/S/E/W decoratively placed

---

### C. Numbered Feature Slide (most common)

**Background:** `#F5F1E4`

```
┌─────────────────────────────────────────┐
│  01. SECTION NAME                       │
│  [orange number · SemiBold · H2]        │
│                                         │
│  MAIN HEADLINE                          │
│  [Archivo Black · H1 · dark]            │
│                                         │
│  Body paragraph text. Two to three      │
│  sentences explaining the concept.      │
│  [Raleway Medium · body · dark]         │
│                                         │
│  "The best leaders serve others first." │
│  [Raleway SemiBold · maxim · orange]    │
└─────────────────────────────────────────┘
```

Example — Slide 15:
> `SERVANT LEADERSHIP` (H1) / "Prioritize the growth, well-being, and success of your team..." (body) / `"The best leaders serve others first."` (maxim, orange)

---

### D. Detail / Three-Column Slide

**Background:** `#F5F1E4`

```
┌─────────────────────────────────────────┐
│  01. CATEGORY                           │
│                                         │
│  Strengths    │  Weaknesses  │  Work    │
│  ──────────── │  ──────────  │  Style   │
│  Item one     │  Item one    │  Item    │
│  Item two     │  Item two    │  Item    │
│  Item three   │  Item three  │  Item    │
│                                         │
│  [Raleway Medium · dark · no bullets]   │
└─────────────────────────────────────────┘
```

Column headers: Raleway SemiBold, `#363636`
Column items: Raleway Medium, `#1B1B1B`, stacked with line-height spacing (no bullet glyphs)

---

### E. Big Statement Slide

**Background:** `#1B1B1B` or `#F5F1E4`

```
┌─────────────────────────────────────────┐
│                                         │
│   SINGLE BOLD                           │
│   CLAIM HERE                            │
│   [Archivo Black · display · white      │
│    or accent orange]                    │
│                                         │
│   One supporting sentence.              │
│   [Raleway Medium · white or dark]      │
│                                         │
└─────────────────────────────────────────┘
```

Example — "WHAT MAKES A GREAT LEADER?" with bullet list below, or a single-phrase dramatic statement.

---

### F. Definition Slide

**Background:** `#F5F1E4`

```
┌─────────────────────────────────────────┐
│                                         │
│  TERM TITLE                             │
│  [Raleway Bold · H1 · dark]             │
│                                         │
│  Term: full definition sentence that    │
│  explains what the concept is.          │
│  [Raleway Medium · body]                │
│                                         │
│  Clarifying context sentence.           │
│  [Raleway SemiBold · smaller · orange   │
│   or #363636]                           │
│                                         │
└─────────────────────────────────────────┘
```

Example — Slide 29 (PRD):
> `PRODUCT REQUIREMENTS DOCUMENT` / "Product Requirements Document (PRD): a foundational guide..." / "A PRD is created before development begins."

---

### G. Numbered List / Phases Slide

**Background:** `#F5F1E4`

```
┌─────────────────────────────────────────┐
│                                         │
│   N [TOPIC] TITLE                       │
│   [Raleway SemiBold · H2]               │
│                                         │
│   01. PHASE ONE   │  02. PHASE TWO      │
│   03. PHASE THREE │  04. PHASE FOUR     │
│                   05. PHASE FIVE        │
│                                         │
│   [Numbers in orange · Labels in dark]  │
│                                         │
└─────────────────────────────────────────┘
```

---

### H. Q&A / Transition Slide

**Background:** `#1B1B1B`

```
┌─────────────────────────────────────────┐
│                                         │
│                                         │
│         ANY                             │
│         QUESTIONS?                      │
│         [Archivo Black · display · white]│
│                                         │
│                                         │
└─────────────────────────────────────────┘
```

Single phrase, centered or left-aligned, nothing else on the slide.

---

### I. Closing Slide

**Background:** `#1B1B1B`

```
┌─────────────────────────────────────────┐
│                                         │
│   THAT'S                                │
│   DAY 3                                 │
│   [Archivo Black · display · white]     │
│                                         │
│   GO SLOW. STAY CURIOUS. SERVE PEOPLE   │
│   WELL.                                 │
│   [Raleway Medium · accent orange]      │
│                                         │
│   Looking-ahead note in small text.     │
│   [Raleway Medium · white · small]      │
│                                         │
└─────────────────────────────────────────┘
```

---

## Component Patterns

### Numbered Section Prefix
```
01. SECTION TITLE
```
- `01.` → Raleway Bold, `#FB6636`
- `SECTION TITLE` → Raleway SemiBold, `#1B1B1B`
- Always on the same line, H2 size

### Slide Maxim / Tagline
A one-liner placed below body content that distills the slide's lesson:
- Font: Raleway SemiBold or Medium
- Size: slightly smaller than body (0.9–1rem)
- Color: `#FB6636` for emphasis, or `#363636` for softer contrast
- Often formatted as a quote or imperative sentence
- Examples: *"Trust is built on honesty."* / *"People work harder for leaders they believe in."*

### Three-Column Grid
Used for Strengths / Weaknesses / Work Style breakdowns:
- Equal-width columns with `#F1EBE3` or transparent fill
- Column header: Raleway SemiBold, `#363636`, H3 size
- Items: Raleway Medium, `#1B1B1B`, stacked with generous line-height
- No bullet glyphs — whitespace separation only

### Kanban Board Columns
Five columns: **TO DO · UPCOMING · IN PROGRESS · REVIEW · DONE**
- Each column: rounded-corner card, light fill
- Column title: Raleway Bold, dark, centered
- Description: Raleway Medium, small, centered
- Visual note at bottom: *"Cards move left to right as work progresses."*

### Phase Steps (01–05 grid)
Used for project phases, 5-item processes:
- Grid layout: 2×2 + 1 centered, or horizontal strip
- Phase number: `01.` in orange, Raleway Bold
- Phase name: ALL CAPS, Raleway SemiBold, dark

---

## Slide-by-Slide Reference

| # | Layout Type | Key Content |
|---|-------------|-------------|
| 1 | Cover | "LEADERSHIP & PROJECT MANAGEMENT 2026" |
| 2 | Section Intro | "COMPASS PERSONALITY TEST" with compass graphic |
| 3 | Activity Prompt | Find Your North Star — worksheet instructions |
| 4 | Section Intro (updated) | Compass with N/S/E/W personality labels |
| 5 | Body/Context | Compass overview — no direction is better than another |
| 6 | Numbered Feature | 01. NORTH — The Driven Leader |
| 7 | Detail 3-Column | 01. NORTH — Strengths / Weaknesses / Work Style |
| 8 | Numbered Feature | 02. SOUTH — The Team Builder |
| 9 | Detail 3-Column | 02. SOUTH — Strengths / Weaknesses / Work Style |
| 10 | Numbered Feature | 03. EAST — The Quality Analyst |
| 11 | Detail 3-Column | 03. EAST — Strengths / Weaknesses / Work Style |
| 12 | Numbered Feature | 04. WEST — The Creative Visionary |
| 13 | Detail 3-Column | 04. WEST — Strengths / Weaknesses / Work Style |
| 14 | Big Statement / List | "WHAT MAKES A GREAT LEADER?" — 7 traits |
| 15 | Numbered Feature | SERVANT LEADERSHIP |
| 16 | Numbered Feature | EMPATHY & LISTENING |
| 17 | Numbered Feature | PERSUASION OVER COERCION |
| 18 | Numbered Feature | HONESTY |
| 19 | Numbered Feature | SKILL DEVELOPMENT |
| 20 | Numbered Feature | ELEVATE OTHERS |
| 21 | Numbered Feature | DELEGATE WORK |
| 22 | Section Intro | PROJECT MANAGEMENT intro + definition |
| 23 | Phase Grid | 5 PROJECT PHASES overview (01–05 grid) |
| 24 | Numbered Feature | 01. INITIATION |
| 25 | Numbered Feature | 02. PLANNING |
| 26 | Numbered Feature | 03. EXECUTION |
| 27 | Numbered Feature | 04. TRACKING |
| 28 | Numbered Feature | 05. CLOSING |
| 29 | Definition | PRODUCT REQUIREMENTS DOCUMENT |
| 30 | List | KEY PARTS OF A PRD — 5 items |
| 31 | Definition | STANDARD OPERATING PROCEDURE |
| 32 | List | KEY PARTS OF AN SOP — 5 items |
| 33 | Kanban Board | TRELLO & THE KANBAN BOARD |
| 34 | Q&A | "ANY QUESTIONS?" |
| 35 | Transition | "GIVE HENRY A WARM WELCOME!" |
| 36 | Q&A | "ANY QUESTIONS?" |
| 37 | Closing | "THAT'S DAY 3" + tagline + looking ahead |

---

## Quick-Reference Cheat Sheet

When creating a new slide in this system, apply this checklist:

```
□ Background: #F5F1E4 (content) or #1B1B1B (cover/transition)
□ Headings: ALL CAPS, Archivo Black or Raleway Bold/SemiBold
□ Numbers: 01. format in #FB6636
□ Body: Raleway Medium, #1B1B1B, max 3 sentences
□ Maxim: Raleway SemiBold, #FB6636 or #363636, at slide bottom
□ Orange: only for accent — never body text
□ No bullets: use whitespace and line breaks instead
□ One idea per slide
```
