<h1 align="center">Rishi Soni</h1>

<p align="center">
  <b>Software Engineer · Backend & Distributed Systems</b><br/>
  Indore, India · <a href="mailto:rishisoni.tech@gmail.com">rishisoni.tech@gmail.com</a>
</p>

<p align="center">
  <a href="https://linkedin.com/in/rishi-soni-7427b4252"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://leetcode.com/u/rishisoni1545"><img src="https://img.shields.io/badge/LeetCode-400%2B_Solved-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
  <a href="https://github.com/RISHI-SONI345"><img src="https://img.shields.io/badge/GitHub-RISHI--SONI345-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

<p align="center">
  <code>Java 21</code> • <code>Spring Boot 4</code> • <code>Spring Modulith</code> • <code>PostgreSQL 17</code> • <code>Redis</code> • <code>Resilience4j</code> • <code>ArchUnit</code> • <code>React Native</code>
</p>

---

### 📌 Engineering Snapshot

```
┌───────────────────────────────────┬───────────────────────────────────┐
│ Metric / Impact                   │ Technical Implementation          │
├───────────────────────────────────┼───────────────────────────────────┤
│ 10,000+ Production MAU            │ Shipped offline-first mobile vault│
│ 40% Client Latency Reduction      │ Query caching, payload batching   │
│ < 12s p95 Async AI Pipeline       │ Java 21 Virtual Threads + Retries │
│ 99% Test Branch Coverage          │ Pure domain core across 42 audios │
│ 0 Cyclic Dependencies             │ Enforced via ArchUnit suite       │
│ 400+ Algorithmic Problems Solved  │ LeetCode, GeeksforGeeks           │
└───────────────────────────────────┴───────────────────────────────────┘
```

---

### 🏛️ Flagship System: StageMinute

> **Production AI Speech-Coaching Platform** · [Live App: stageminute.app](https://stageminute.app) · [Architecture Blueprint: stageminute-architecture](https://github.com/RISHI-SONI345/stageminute-architecture)  
> *Stack: Java 21, Spring Boot 4, PostgreSQL 17, Spring Modulith, React Native, OpenAPI, Resilience4j, Sentry*

```
                              [ React Native / Web Client ]
                                            │
                                            ▼ (OpenAPI Contract)
┌─────────────────────────────────── Spring Boot 4 Application ───────────────────────────────────┐
│                                                                                                 │
│  [ Auth / Quota Module ] ──(Atomic SQL / Sliding Window)──▶ [ Postgres 17 User Ledger ]         │
│             │                                                                                   │
│             ▼                                                                                   │
│  [ Speech Processing Module ]                                                                   │
│             │                                                                                   │
│             ├──(Java 21 Virtual Threads)──▶ Deepgram Nova-3 (Streaming Transcription)          │
│             ├──(Resilience4j Bulkhead)────▶ Gemini Flash (Structured Acoustic Feedback)         │
│             │                                                                                   │
│             ▼                                                                                   │
│  [ Deterministic Scoring Core ] (Pure Domain Logic · 99% Branch Coverage · 42 Audio Fixtures)   │
│             │                                                                                   │
│             ▼                                                                                   │
│  [ Transactional Outbox Module ] ─────────▶ [ Durable Webhook Inbox & Entitlements Engine ]     │
│                                                                                                 │
│  * Architecture rules & non-cyclic module boundaries validated continuously via ArchUnit *      │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

<details>
<summary><b>🔍 Deep Dive: Architecture Decisions & Failure Modes Handled</b></summary>
<br/>

1. **Modular Monolith with Enforced Boundaries:**
   - Structured into 11 discrete modules using Spring Modulith. Cross-module calls communicate via bounded domain events and explicit module interfaces.
   - Enforced cyclomatic isolation and zero dependency leaks using strict ArchUnit architecture tests in CI.
2. **High-Throughput Asynchronous AI Pipeline:**
   - Utilizes Java 21 Virtual Threads (`Executors.newVirtualThreadPerTaskExecutor`) to handle concurrent external I/O without pin-locking OS threads.
   - Guarded with Resilience4j bulkheads, rate-limiters, and exponential backoff retries to guarantee a sub-12s p95 turnaround under spiky loads.
3. **Deterministic Speech Scoring:**
   - Speech evaluation uses a pure mathematical domain model running over LLM structured JSON output, eliminating hallucinations and ensuring 100% reproducible scoring across test runs.
4. **Concurrency-Safe Cost Controls:**
   - Quota tracking uses atomic SQL updates (`UPDATE quotas SET used = used + 1 WHERE used < limit`) and unique-key idempotency ledgers, preventing double-billing and race conditions.
5. **Reliable Event Delivery:**
   - Implemented the Transactional Outbox pattern paired with a durable Webhook Inbox to ensure zero event loss between payment processing and speech quota unlocks.

</details>

---

### 💼 Production Experience

#### **Software Engineer** — Lost Ferry Interactive
*Aug 2025 – Aug 2026 · Remote*

* **DocIt — Secure Document Vault** *(10K+ Monthly Active Users)*
  - **Performance Optimization:** Cut client-side API response latency by **40%** (2.5s → 1.5s) via query caching, pagination, and payload optimization.
  - **Offline Sync & Architecture:** Built cross-platform client in TypeScript from Figma specifications using Clean Architecture, Zustand, and TanStack Query for background data synchronization.
  - **Device Security:** Implemented biometric authentication (Face ID and fingerprint), OS Keychain/Keystore token storage, and PIN-protected vaults.
  - **Feature Delivery:** Shipped real-time camera document capture with automatic edge detection, PDF/image viewer, expiry reminders, and encrypted sharing.

* **FarbenBridge — Financial Analytics Platform** *(Client Engagement)*
  - **Backend API Design:** Developed Spring Boot REST APIs backed by PostgreSQL and Redis caching for portfolio analytics and transaction feeds.
  - **Data Consistency & Idempotency:** Implemented idempotency keys on mutating endpoints to eliminate duplicate transactions caused by client-side retries.
  - **Conditional Caching:** Implemented ETag-based HTTP caching returning `304 Not Modified` responses for static dashboard queries, minimizing database read load.
  - **UI Performance:** Built role-based financial dashboards in Next.js/React; improved page load performance by **35%** using component memoization and state optimization.

---

### 🧪 Systems & Infrastructure Lab

#### [Distributed URL Shortener with Analytics](https://github.com/RISHI-SONI345/Distributed-URL-Shortener-with-Analytics)
*Spring Boot, MySQL, Redis, Docker*
- High-throughput URL shortening service utilizing Base62 encoding and multi-tier caching (Redis LRU + in-memory buffers).
- Implemented Token Bucket rate limiting to safeguard redirect and generation endpoints against scraping bots.
- Instrumented real-time click analytics with geo and user-agent aggregation.

---

### 🛠️ Technical Competency

| Domain | Core Stack & Methodologies |
| :--- | :--- |
| **Languages** | Java 21, SQL, TypeScript, JavaScript |
| **Backend & Frameworks** | Spring Boot, Spring Modulith, Spring Security, REST APIs, OpenAPI, Resilience4j |
| **Data & Caching** | PostgreSQL, Redis, Flyway Database Migrations |
| **System Architecture** | Modular Monoliths, Hexagonal Architecture, Event-Driven Architecture, Transactional Outbox, Idempotency Keys |
| **Mobile & Frontend** | React Native (Expo), Next.js, React.js, Zustand, TanStack Query, Tailwind CSS |
| **Testing & Quality** | ArchUnit, JUnit 5, Testcontainers, Integration Testing, 99% Branch Coverage Design |
| **DevOps & Tooling** | Docker, GitHub Actions, CI/CD, Git, Linux |

---

### 🏆 Achievements & Problem Solving

- **Smart India Hackathon 2024 Finalist:** Led a 6-member engineering team; designed and owned the end-to-end software architecture for the team's AI-driven platform.
- **Algorithmic Problem Solving:** 400+ problems solved across LeetCode, GeeksforGeeks, and HackerRank with an emphasis on Graphs, Dynamic Programming, and Concurrency.

---

### 📬 Get In Touch

<p align="center">
  <a href="mailto:rishisoni.tech@gmail.com"><b>rishisoni.tech@gmail.com</b></a> •
  <a href="https://linkedin.com/in/rishi-soni-7427b4252"><b>LinkedIn</b></a> •
  <a href="https://leetcode.com/u/rishisoni1545"><b>LeetCode</b></a> •
  <a href="https://github.com/RISHI-SONI345"><b>GitHub</b></a>
</p>
