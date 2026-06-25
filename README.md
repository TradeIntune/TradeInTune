<div align="center">

# TradeInTune

**Duolingo for forex.**

Gamified, interactive forex education. You do not watch videos. You press the button, read the chart, answer the question, and get graded in real time.

[![Status](https://img.shields.io/badge/status-pre--launch-blue)](https://tradeintune.com)
[![Site](https://img.shields.io/badge/web-tradeintune.com-146ef5)](https://tradeintune.com)
[![Built in public](https://img.shields.io/badge/built-in%20public-7a3dff)](https://tradeintune.com)

</div>

## What this is

Forex is one of the most-searched skills on the internet and one of the worst-taught: endless YouTube playlists, signal groups that keep you dependent, and gurus who profit whether you learn or not.

TradeInTune is the structural fix. A 14-module, 123-lesson curriculum taught entirely through interactive beats, gated by graded checkpoints, and wrapped in game mechanics that make showing up tomorrow the path of least resistance. You build the skill by doing the reps yourself, not by watching someone else do them. That is the point.

## How it teaches

- **15 beat types per lesson.** Teach screens with optional voice-over, video beats, and 12 quiz formats: multiple choice, true/false, fill-in-the-blank, swipe decks, matching, screenshot reading, sequencing, multi-select, categorize, numeric estimate, odd-one-out, and chart-draw, where you draw a level or trendline on a real candle tape, get graded against price and time tolerances, then watch the remaining bars replay forward.
- **Checkpoints.** Every module ends in a graded exam: one attempt per question, 85% to pass. No skipping fundamentals on vibes.
- **Hearts, XP, gems, streaks.** Wrong answers cost hearts. Consistency pays for the safety net. All awards are server-authoritative with evidence checks, so the leaderboard cannot be forged from a browser console.
- **An adaptive engine.** Every answer is logged against 46 tagged concepts. Your weakest concept becomes your next drill, and every mistake you make becomes a replayable review queue.

## Features

- 14 modules / 123 lessons, first 5 modules free
- 43 scenario drills on a real candle chart engine
- Adaptive weak-spot drills across 46 concepts
- Mistakes review: your wrong answers become your curriculum
- Road Map: 35 real-world homework tasks (open the demo account, sit out the news release)
- Daily challenge from a 206-question adaptive bank
- 147-term progress-gated glossary
- 24 badges computed live from real stats
- Global and friends leaderboards, community feed, public profiles
- Free browser tools: position size and compounding calculators, no account needed

## Stack

| Layer | Tech |
|---|---|
| Framework | Next.js 16 (App Router), React 19, TypeScript |
| Styling | Tailwind CSS v4, Framer Motion |
| Backend | Supabase (Postgres + RLS, Auth, Storage), server-authoritative game economy |
| Payments | Stripe (subscriptions, webhooks, customer portal) |
| Charts | lightweight-charts v5 powering the drill engine |
| Data layer | TanStack Query 5 with server-seeded caches |
| Hosting | Vercel, static-rendered marketing pages on the edge |

## Honesty, enforced in code

Testimonials on the site are gated behind a literal `TESTIMONIALS_ARE_REAL = false` flag and will not render until real ones exist. No earnings projections anywhere. No signals, no copy-trading, no live-account mirror. The product is built so users outgrow it, on purpose.

## Status

**Pre-launch.** The product is built end to end and live at [tradeintune.com](https://tradeintune.com); the user base is currently zero and we say so. Built solo by a 20-year-old forex trader who got tired of watching the skill get taught with playlists and hype.

Building in public. The streak starts at launch.
