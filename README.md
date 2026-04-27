# TradeInTune

Interactive forex education platform built for self-directed learners.

[tradeintune.com](https://tradeintune.com)

---

## What it is

A skill-building platform for forex trading. Lessons are short, interactive, and focused on reps over passive video consumption. Users move through a structured curriculum of 14 modules covering everything from "what is a currency pair" to live trade journaling and prop firm scaling.

The platform is built around a verified track record (ASIC-regulated brokerage, public MYFXBOOK results) and treats trading as a hard skill that takes deliberate practice, not a get-rich-quick pitch.

---

## Tech stack

**Frontend**
- [Next.js 16](https://nextjs.org) (App Router, Turbopack)
- TypeScript
- Tailwind CSS
- [Framer Motion](https://www.framer.com/motion/) for transitions and lesson animations
- [Lucide](https://lucide.dev) for icons
- [next-themes](https://github.com/pacocoursey/next-themes) for dark mode

**Backend & infra**
- [Supabase](https://supabase.com) — Postgres, Auth, Storage, Row Level Security
- [Vercel](https://vercel.com) — hosting and edge functions
- [Stripe](https://stripe.com) — subscription billing (monthly + yearly tiers)
- [PostHog](https://posthog.com) — product analytics

**Data layer**
- [@tanstack/react-query](https://tanstack.com/query) — client-side caching and invalidation
- [Zod](https://zod.dev) — runtime validation at API boundaries

---

## Architecture notes

- App Router with route groups: `(marketing)`, `(auth)`, `(app)`, `(lesson)`
- Lesson route group is a full-screen takeover bypassing the standard app shell — no sidebar, no bottom nav
- Streak math is user-local (not UTC) to prevent timezone bugs for non-UTC users
- Admin gating is UUID-based via env var, never email
- All XP-writing operations are gated by check constraints + planned to move behind a server RPC

---

## Curriculum

14 modules. ~123 lessons. ~350-400 interactive quiz questions across 20+ unique question types — not just multiple choice, but swipe-card validation, matching, fill-in, scenario drills, risk calculators, and chart annotation tasks.

Modules 1-5 are free. Modules 6-14 are gated behind the paid subscription.

---

## Status

Live in production at [tradeintune.com](https://tradeintune.com).

This repo intentionally contains only documentation. The application source is private.
