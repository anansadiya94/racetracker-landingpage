## Design Context

### Users
Runners of all levels — from casual 5K participants doing a few races a year to dedicated marathoners and ultra runners who chase PRs obsessively. Used in two distinct moments: (1) post-race logging — the quiet satisfaction of entering a finish time you're proud of; (2) planning mode — reviewing upcoming races, setting goals, staying motivated. The app is a personal record, not a social one.

### Brand Personality
Three words: **Precise. Earned. Steady.**

The intersection of a race timer's clarity, the quiet pride of a personal record, and the reliability of a training partner you can always count on. Motivating without being loud. Energetic without being aggressive. Clean without being cold.

Not a hype machine. Not a health dashboard. The feeling of looking at your official results after a race you worked hard for.

### Aesthetic Direction
- **Theme**: Light primary, dark secondary (supports both — follows system preference). Users browse the landing page in any context; the app is used in daylight and evening equally.
- **Visual tone**: Refined precision. Think timing boards, race bibs, official results sheets — not sports marketing, not wellness apps. Numbers matter and should look important.
- **Anti-references**: Generic health app (pastel cards, Apple Health aesthetic), social media (feeds, leaderboards), sports brand marketing (aggressive, high-contrast, loud).
- **References to keep from current landing**: The Cormorant Garamond + Archivo pairing direction is *right in spirit* (display serif + clean sans) but Cormorant Garamond is overused — find a fresher serif or distinctive display face with the same elegance.

### Design Principles
1. **Numbers are the hero** — finish times, PRs, distances deserve typographic emphasis. Big, legible, beautiful numerals.
2. **Achievement, not activity** — this is a log of races completed and goals set, not a training tracker. Every design choice should feel like it honors the effort of actually racing.
3. **Quiet confidence** — the interface doesn't need to shout. Restrained use of color, generous space, clear hierarchy.
4. **Personal over social** — no leaderboards, no feeds, no comparison. Every screen is about *your* journey.
5. **Precision matters** — if a runner cares about 3:28:27 vs 3:29:14, the interface should too. Mono-spaced time displays, sharp data presentation.

### Platform Notes

**Landing page** (`/Users/anan.sadiya/Developer/racely`):
- Single HTML file, pure CSS — no build system
- Fonts: Cormorant Garamond (banned — needs replacement) + Archivo (fine)
- Current issues to address on next polish pass:
  - Gradient text on logo and `<em>` in hero heading — BANNED by impeccable guidelines
  - Top accent stripes on bento cards (`.bc::before`) — acceptable (not side-stripe), but monotonous
  - Font: replace Cormorant Garamond with something equally distinctive but less overused

**iOS app** (`/Users/anan.sadiya/Developer/racely-ios`):
- SwiftUI + TCA, iOS 18+
- Quality bar: Polished & native — SF Pro, system conventions, exceptionally well executed
- Colors: currently all system colors (`.blue`, `.purple`) — fine for native feel, no custom branding needed
- Typography: system `.rounded` for numbers — good for native feel
