# 📐 System Design — Complete Study Guide

> A structured, interview-ready knowledge base covering **20 topics** and **18 design problems** — built for freshers who want to walk into system design interviews with confidence, not confusion.

---

## 🎯 Philosophy

```
You don't need a perfect design.
You need structured thinking.

"Where will it break?" → "How do I fix it?" → "What's the trade-off?"
```

---

## 📂 Guide Index

### 🧱 Fundamentals (Start Here)

| # | File | Topics Covered |
|---|------|---------------|
| 1 | [System Design Basics](1.systemDesignBasics.md) | HLD vs LLD, monolith vs microservices, client-server model |
| 2 | [HLD vs LLD](2.HLDvsLLD.md) | When to use each, depth of design, interview expectations |
| 3 | [Fundamentals](3.Fundamentals.md) | Latency, throughput, availability, consistency, SLAs |
| 4 | [Databases](4.Databases.md) | SQL vs NoSQL, indexing, replication, ACID, BASE |

### ⚙️ Core Infrastructure

| # | File | Topics Covered |
|---|------|---------------|
| 5 | [Caching & Performance](5.Caching&performanceBasics.md) | Cache strategies, Redis, write-through vs write-back, eviction |
| 6 | [Load Balancers](6.LoadBalancer.md) | L4 vs L7, algorithms, health checks, sticky sessions |
| 7 | [API Gateways](7.APIGateways.md) | Routing, auth, rate limiting, API Gateway vs LB |
| 8 | [Messaging Queues](8.MessageingQueues.md) | Kafka, RabbitMQ, pub/sub, async processing |
| 9 | [Scalability Patterns](9.ScalabilityPatterns.md) | Horizontal scaling, auto-scaling, circuit breaker, stateless servers |
| 10 | [Rate Limiting](10.rateLimiting.md) | Token bucket, sliding window, distributed rate limiting |

### 🚀 Advanced Concepts

| # | File | Topics Covered |
|---|------|---------------|
| 12 | [CAP Theorem](12.CAPTheorem.md) | CP vs AP, consistency models, PACELC, database classification |
| 13 | [CDN](13.CDN.md) | Pull vs Push CDN, caching strategies, cache invalidation, Netflix |
| 14 | [Proxies](14.Proxies.md) | Forward vs Reverse proxy, NGINX config, Cloudflare |
| 15 | [Networking Basics](15.NetworkingBasics.md) | DNS, TCP/UDP, HTTP/1.1→2→3, WebSockets, SSE, TLS |
| 16 | [Distributed ID Generation](16.DistributedIDGeneration.md) | UUID, Twitter Snowflake, ULID, Ticket Server |
| 17 | [Data Partitioning](17.DataPartitioning.md) | Sharding strategies, consistent hashing, virtual nodes |
| 18 | [Bloom Filters](18.BloomFilters.md) | Probabilistic data structures, false positives, Cassandra use case |
| 19 | [Observability](19.Observability.md) | Logging, metrics, tracing, 4 Golden Signals, ELK, Grafana |
| 20 | [Security Basics](20.SecurityBasics.md) | OAuth 2.0, JWT, CORS, SQL injection, XSS, mTLS, bcrypt |

### 🎯 Interview Preparation

| # | File | What's Inside |
|---|------|--------------|
| 11 | [Interview Problems](11.interviewProblmes.md) | **The main file** — 7-step framework, 18 design problems, 32 Q&A, 30 rapid-fire drills |

---

## 🏗️ Design Problems Covered (File 11)

| # | Problem | Key Concepts Tested |
|---|---------|-------------------|
| 1 | URL Shortener (Bitly) | Hashing, base62, read-heavy, caching |
| 2 | Chat System (WhatsApp) | WebSockets, presence, message queues |
| 3 | File Upload (Google Drive) | Pre-signed URLs, chunked upload, S3 |
| 4 | Notification Service | Multi-channel, Kafka, FCM/SES/Twilio |
| 5 | Rate Limiter | Token bucket, Redis INCR, distributed counting |
| 6 | Search System | Elasticsearch, CDC pipeline, inverted index |
| 7 | Blog Platform (Medium) | Fan-out, CDN, read replicas |
| 8 | Expense Tracker (Splitwise) | Graph-based debt simplification, ACID |
| 9 | Paste Service (Pastebin) | Object storage, TTL, read-heavy |
| 10 | Social Media Feed | Fan-out-on-write vs fan-out-on-read |
| 11 | E-Commerce (Amazon) | Inventory locking, Saga pattern, flash sales |
| 12 | Parking Lot System | Concurrency, sensor integration, LLD |
| 13 | Video Streaming (YouTube) | Transcoding, CDN, adaptive bitrate |
| 14 | CDN / Edge Network | Cache stampede, Anycast, purge propagation |
| 15 | Auth & SSO (Auth0) | JWT flow, brute-force defense, credential stuffing |
| 16 | Logging Pipeline (ELK) | Kafka buffer, trace sampling, tiered storage |
| 17 | Global DNS (Route 53) | Anycast, TTL management, health-check failover |
| 18 | Distributed Cache (Redis) | Hot key fix, cache warming, fail-open vs fail-closed |

---

## 📖 How to Use This Guide

### If you're starting from scratch:
```
Files 1–4 (Fundamentals) → Files 5–10 (Infrastructure) → File 11 (Practice Problems)
```

### If you have basics and want to stand out:
```
Files 12–20 (Advanced) → File 11, Sections 19–25 (Advanced Problems & Q&A)
```

### Before an interview (1-hour crash course):
```
File 11 → Read the 7-Step Framework → Skim 3-4 design problems → 
Review rapid-fire drills → Done. You won't go blank.
```

---

## 🧠 The Golden Framework (from File 11)

Every system design answer follows these 7 steps:

```
1. CLARIFY     → Ask requirements. Functional + Non-functional.
2. ESTIMATE    → Users, RPS, storage, bandwidth.
3. API DESIGN  → Define endpoints (REST).
4. DATA MODEL  → Tables, relationships, SQL vs NoSQL.
5. HIGH-LEVEL  → Draw boxes: Client → LB → App → DB → Cache.
6. DEEP DIVE   → Tackle the hardest part (the bottleneck).
7. TRADE-OFFS  → "I chose X because... The alternative Y has the downside of..."
```

---

## 📊 Stats

| Metric | Count |
|--------|-------|
| Total files | 20 |
| Design problems | 18 |
| Interview Q&A | 32 (structured answers) |
| Rapid-fire drills | 30 |
| Total lines | ~18,000+ |

---

> *"There is no perfect design. There is only design that doesn't break at YOUR scale."*

"# systemdesign_notes" 
