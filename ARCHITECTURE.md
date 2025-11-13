
# ARCHITECTURE — UGC AdMaker

Start: (we will expand this)

## Domains
- Web: Next.js 16 (App router, Server Actions)
- Worker: Cloudflare Workers + Queues
- Storage: Cloudflare R2
- DB: PostgreSQL + Prisma

## Basic flow
User -> apps/web -> POST /api/jobs -> Queue -> Worker -> Veo3 -> Webhook -> R2 -> apps/web (signed URL)

## To fill
- Data models
- Queue message shape
- Security & idempotency
- Observability plan
