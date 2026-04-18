# CLAUDE.md

## Project Overview

Racely landing page — a single-file HTML/CSS/JS marketing site for the Racely iOS app (race tracker for runners).

- **Stack**: Pure HTML + CSS + JS, no build system
- **File**: `index.html` (all styles and scripts inline)
- **Fonts**: Archivo (body) — display font TBD (see Design Context)
- **Hosted**: GitHub Pages at https://anansadiya94.github.io/racely/

## Design Context

### Users
Runners of all levels — from casual 5K participants to dedicated marathoners and ultra runners. Landing page visitors are discovering the app or looking for the App Store link.

### Brand Personality
Three words: **Precise. Earned. Steady.**

The intersection of a race timer's clarity, the quiet pride of a personal record, and the reliability of a trusted training partner. Motivating without being loud. Clean without being cold.

### Aesthetic Direction
- **Theme**: Light primary, dark secondary (user-toggleable, respects system preference)
- **Visual tone**: Refined precision. Numbers matter and should look important. Think timing boards, official race results — not sports marketing, not wellness dashboards.
- **Anti-references**: Generic health app (pastel cards, Apple Health aesthetic), social media (feeds, leaderboards), aggressive sports brand marketing
- **Font note**: Cormorant Garamond is overused/banned — find an equally elegant display face that's less common. Archivo body font is fine.

### Design Principles
1. **Numbers are the hero** — finish times, PRs, distances deserve typographic weight and presence
2. **Achievement, not activity** — race log, not training tracker. Design honors the effort of racing.
3. **Quiet confidence** — restrained color, generous space, clear hierarchy
4. **Personal over social** — every message is about *your* journey, not comparison
5. **Precision matters** — 3:28:27 ≠ 3:29:14. Sharp, legible data presentation

### Known Issues to Address
- Gradient text on logo `<span>` and hero `<em>` — banned pattern (`background-clip: text` + gradient)
- Cormorant Garamond — overused font, needs replacement with equally distinctive alternative
- Top accent stripes on bento cards (`.bc::before { height: 3px }`) — acceptable but monotonous
