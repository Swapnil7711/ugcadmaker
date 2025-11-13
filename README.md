
# UGC AdMaker

**Mission:** Build a production-grade UGC-style AI ad generator (Veo3) that demonstrates senior-level system design, Next.js expertise, cloud engineering, and DevOps — aimed at landing a $100k remote job.

## Quick links
- Project board: https://github.com/users/Swapnil7711/projects/1/views/1
- Day 1 checklist: DAY1.md
- Architecture notes: ARCHITECTURE.md

## High level
This repo is a monorepo (Turborepo) with:
- `apps/web` — Next.js 16 app (frontend + server actions)
- `apps/worker` — Cloudflare Worker for job processing + webhook
- `packages/db` — Prisma schema
- `packages/shared` — shared types & utils
- `packages/ui` — UI components (shadcn + tailwind)

## How to contribute
1. Create branch `feature/<short-desc>` from `dev`.
2. Open PR to `dev` with the PR template.
3. Run tests locally and include screenshots where relevant.

## Goals for MVP (15 days)
- Auth (Google Sign-in)
- LLM script generator
- Upload product media → create job
- Worker calls Veo3 → stores video in R2
- Dashboard + preview

## Contact
Swapnil — project owner
Mentor: ChatGPT
