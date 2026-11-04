# Questline

A gamified planner PWA that breaks a goal into milestones and daily tasks, tracks XP, levels and streaks, and reschedules missed tasks.

- Vanilla HTML, CSS and JavaScript, data in localStorage, works offline, installable
- XP: 10 per task, 50 per milestone, 200 per goal. Level = floor(sqrt(XP / 40)) + 1
- Coach: rule-based. `coach()` decides what to say, `rebalance()` respawns pending tasks across the days left

## Roadmap
1. Accounts and database (Supabase)
2. AI agent: replace or extend `coach()` and `rebalance()` with a backend function that calls an AI model

## Run
Serve over https or localhost (service worker needs it): `npx serve .`
