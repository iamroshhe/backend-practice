# backend-practice

Small backend projects. Each one teaches one backend skill. I add one folder per project and commit a small step every day.

Stack: Node.js, Express, PostgreSQL/SQLite, Redis, BullMQ, Socket.io.

## Projects

| #  | Project                     | Skill                                   | Status      |
|----|-----------------------------|-----------------------------------------|-------------|
| 01 | URL Shortener               | REST, unique IDs, indexes, redirects    | Not started |
| 02 | CLI Todo / Expense Tracker  | Node without Express, files, argv       | Not started |
| 03 | Mini Express from scratch   | `http` module, routing, middleware      | Not started |
| 04 | Rate Limiter                | Redis, fixed window vs token bucket     | Not started |
| 05 | Pastebin with expiry        | Postgres + Prisma, cron, Redis TTL      | Not started |
| 06 | Caching layer demo          | Cache-aside, invalidation, benchmarks   | Not started |
| 07 | Job queue worker            | BullMQ, workers, retries                | Not started |
| 08 | Webhook receiver            | HMAC signatures, idempotency            | Not started |
| 09 | Real-time chat room         | WebSockets, Redis pub/sub               | Not started |
| 10 | Tiny RAG: chat with a PDF   | Chunking, embeddings, retrieval         | Not started |


The daily plan is in [ROADMAP.md](ROADMAP.md).

## Folder layout

Each project folder has:

- `README.md`: what it does, how to run it, and "What I learned" in 3 lines
- `src/`: the code
- `test/`: a test or two
