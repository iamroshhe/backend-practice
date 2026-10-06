# Roadmap: one commit a day

Each line is one day's work and one commit. Every step should leave the project in a working state.
Tick it off when it's pushed.

## 01 URL Shortener
- [x] Day 1: repo skeleton, README, roadmap
- [ ] Day 2: `npm init`, Express server, `GET /health`
- [ ] Day 3: `POST /shorten` with an in-memory store and short ID generation
- [ ] Day 4: `GET /:code` redirect (302) and click counter, `GET /stats/:code`
- [ ] Day 5: move storage to SQLite, add a unique index on `code`
- [ ] Day 6: input validation (bad URLs, unknown codes return 404)
- [ ] Day 7: tests with `node:test` + supertest, finish README "What I learned"

## 04 Rate Limiter
- [ ] Day 1: Express app plus fixed-window limiter in memory (10 req/min per IP)
- [ ] Day 2: return 429 and `Retry-After` / `X-RateLimit-*` headers
- [ ] Day 3: token bucket version, a switch to pick the algorithm
- [ ] Day 4: Redis-backed fixed window (`INCR` + `EXPIRE`)
- [ ] Day 5: run 2 servers to show the in-memory limiter failing and Redis working
- [ ] Day 6: tests, README with the comparison

## 07 Job Queue Worker
- [ ] Day 1: Redis + BullMQ setup, `POST /jobs/email` adds a job
- [ ] Day 2: worker process that "sends" the email (console log + fake delay)
- [ ] Day 3: retries with backoff, a job that fails randomly
- [ ] Day 4: failed-job handling and `GET /jobs/:id` status endpoint
- [ ] Day 5: second job type: image resize with `sharp`
- [ ] Day 6: tests, README

## 10 Tiny RAG: chat with a PDF
- [ ] Day 1: read a PDF and print its text
- [ ] Day 2: split the text into overlapping chunks
- [ ] Day 3: embed chunks and save them to a JSON file
- [ ] Day 4: embed the question, find the top matching chunks (cosine similarity)
- [ ] Day 5: send the chunks + question to an LLM and print the answer
- [ ] Day 6: clean up to ~100 lines, README

## Later
- [ ] 02 CLI Todo / Expense Tracker
- [ ] 03 Mini Express from scratch
- [ ] 05 Pastebin with expiry
- [ ] 06 Caching layer demo
- [ ] 08 Webhook receiver
- [ ] 09 Real-time chat room

Daily plans for these get added when I start them.
