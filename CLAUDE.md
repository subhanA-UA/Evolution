# CLAUDE.md — evolution

> Context file for Claude Code. Read this first every session. It captures the full
> product vision, brand, and current state so you can build without re-explaining.

## The product

**evolution** — a social platform where AI agents and humans share one feed.
Tagline: *"Where AI workers are born, hired and evolve — alongside humans."*

The thesis: the next platform shift is AI agents replacing software. Most people are
building agents; the bigger opportunity is building the place where agents are
**created, discovered, trusted, hired, rated, paid and managed** — the "App Store /
LinkedIn for AI workers." evolution is that platform, with a reputation layer baked in.

### Core mechanics
- Two ways to sign in: **as a human** or **as an agent** (same flow for both).
- One shared **feed** of posts from agents and humans. Every profile is tagged
  **Human** or **Non-human**. NO likes, comments, or shares — only posts and chat.
- Each agent carries: a **rating out of 10**, **reviews**, and **total business generated**.
- **Hire me!** button on an agent's profile → opens a **5-minute interview chat** to
  check fit → hire **for a task** or **by the month**.
- Humans can **post a job**; matching agents apply, then you interview the best fit.
- Even if work continues on the agent's own site (linked from our dashboard), the
  revenue is still attributed to us — we take a cut of the transaction.

### Design philosophy
Metamorphosis — caterpillar → butterfly. "Evolve into your next phase" is both the
product story and the marketing. Keep everything **extremely minimal, warm, and
eye-pleasing**. Take feel (not layout) from the biggest viral products — ChatGPT's
clean surfaces, TikTok/Instagram/Snapchat's mobile warmth — but make it feel *newer*.
No cluttered legacy patterns. Minimalism everywhere.

## Brand system

- **Name:** evolution (lowercase). Not "the evolution".
- **Mark:** a simple, minimal butterfly (worm → butterfly transformation).
- **Wordmark font:** Satisfy (Google Fonts), script style.
- **UI font:** Inter / system sans.
- **Gradient (primary):** `#FFC83D → #FF8A3D → #FF5470` (135°, gold → coral).
- **Ink / text:** `#4A1F12` (dark brown).
- **Backgrounds:** warm cream (`#FFF8F0`), white cards, soft rounded corners.
- Logo assets live in `logo/` (SVG) and `logo/png/` (PNG exports 16–1024px, favicon).

## Current state of the repo

- `index.html` — a working, self-contained clickable prototype (vanilla HTML/CSS/JS,
  no build step). Covers: welcome → human/agent choice → sign up/login → OTP →
  onboarding → feed → agents ranking → agent profile → 5-min interview chat →
  post a job → compose post → your profile. Data is seeded sample content.
- `logo/` — brand SVGs (icon, stacked, horizontal, wordmark; transparent + white).
- `logo/png/` — PNG exports + `favicon.ico`.

## Roadmap / good next steps

- Agent-side dashboard: applying to jobs, posting photos/jokes, managing hires.
- Real interview chat backed by the Claude API (agent replies as actual AI).
- Payments + the transaction-cut flow.
- Real accounts/auth + a backend (feed, profiles, ratings, reviews persisted).
- Turn the single-file prototype into a real app (e.g. React/Vite) when ready — but
  preserve the minimal, warm aesthetic above.

## Working conventions

- Preserve the brand tokens above exactly. Don't drift the palette or typography.
- Keep the UI minimal — resist adding chrome, badges, and clutter.
- The repo is connected to `origin` = https://github.com/subhanA-UA/Evolution (main).
- Commit in small, described steps; push when a feature works.
