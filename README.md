<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=6C63FF&center=true&vCenter=true&width=550&height=70&lines=Hi+%F0%9F%91%8B%2C+I'm+Rishi+Soni;Software+Engineer;Java+21+%26+Spring+Boot+Specialist;Building+modular%2C+high-throughput+systems" alt="Typing SVG" />
</div>

<p align="center">
  <b>Software Engineer based in Indore, India</b><br/>
  Specializing in Spring Boot, Modular Monoliths, Hexagonal Architecture, and High-Performance Mobile/Web Applications.
</p>

<p align="center">
  <a href="https://linkedin.com/in/rishi-soni-7427b4252"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:rishisoni.tech@gmail.com"><img src="https://img.shields.io/badge/Email-rishisoni.tech%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://leetcode.com/u/rishisoni1545"><img src="https://img.shields.io/badge/LeetCode-400%2B_Solved-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
  <a href="https://github.com/RISHI-SONI345"><img src="https://img.shields.io/badge/GitHub-RISHI--SONI345-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

---

### ⚡ Highlights & Impact

- **Production Scale:** Built and shipped client applications serving **10K+ Monthly Active Users**.
- **Latency Optimization:** Cut client-side API response latency by **40%** (2.5s → 1.5s) via query caching, pagination, and payload optimization.
- **Frontend Performance:** Boosted dashboard responsiveness and initial load speeds by **35%** using component memoization and state optimization.
- **System Architecture:** Engineered an 11-module modular monolith (**StageMinute**) with Java 21 virtual threads, Spring Modulith, sub-12s p95 asynchronous AI pipelines, and **99% test branch coverage**.
- **Competitive Problem Solving:** Solved **400+** Data Structures & Algorithms problems across LeetCode, GeeksforGeeks, and HackerRank.
- **Leadership:** **Smart India Hackathon 2024 Finalist** — led a 6-member engineering team and owned the full system architecture.

---

### 🛠️ Technical Stack

| Category | Technologies & Tools |
| :--- | :--- |
| **Languages** | Java 21, SQL, TypeScript, JavaScript |
| **Backend & Systems** | Spring Boot, Spring Modulith, REST APIs, OpenAPI, PostgreSQL, Redis, Flyway |
| **Architecture & Patterns** | Modular Monolith, Hexagonal Architecture, Event-Driven Architecture, Transactional Outbox, Idempotency, Database Transactions |
| **Frontend & Mobile** | React.js, Next.js, React Native (Expo), Zustand, TanStack Query, Tailwind CSS |
| **DevOps & Testing** | Docker, GitHub Actions, CI/CD, Git, JUnit 5, Testcontainers, ArchUnit, Integration Testing |
| **Core Concepts** | Data Structures & Algorithms, System Design, OOP, DBMS |

<p align="left">
  <img src="https://img.shields.io/badge/Java_21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 21" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React Native" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

---

### 💼 Experience

#### **Software Engineer** — Lost Ferry Interactive
*Aug 2025 – Aug 2026 · Remote*

- **DocIt — Secure Document Vault** *(10K+ Monthly Active Users)*  
  *Stack: React Native, Expo, TypeScript, PostgreSQL, Zustand, TanStack Query*
  - Reduced client-side API response latency by **40%** (2.5s to 1.5s) through query caching, pagination, and payload optimization.
  - Architected and built the cross-platform application in TypeScript from Figma specifications, using Clean Architecture, Zustand, and TanStack Query for offline-first data synchronization.
  - Implemented biometric authentication (Face ID and fingerprint), Keychain/Keystore token storage, and PIN-protected vaults.
  - Shipped camera-based document capture with edge detection, PDF/image viewing, expiry reminders, search, and role-based sharing.

- **Client Engagement: FarbenBridge — Financial Analytics Platform**  
  *Stack: Java, Spring Boot, Next.js, React, PostgreSQL, Redis*
  - Developed Spring Boot REST APIs backed by PostgreSQL and Redis caching to support portfolio analytics and transaction data retrieval.
  - Implemented idempotency keys for transaction-creating endpoints, preventing duplicate records during client retries.
  - Implemented ETag-based conditional HTTP requests, returning `304 Not Modified` responses for unchanged dashboard data.
  - Developed role-based financial dashboards for portfolio visualization, transaction tracking, and access-controlled data views; improved page-load performance by **35%** through component memoization and state management optimization.

---

### 🚀 Featured Projects

#### **StageMinute — AI Speech-Coaching Platform**
[Website: stageminute.app](https://stageminute.app)  
*Java 21, Spring Boot 4, PostgreSQL 17, Spring Modulith, React Native, OpenAPI, Resilience4j*

- Architected an **11-module modular monolith** using Spring Modulith and Hexagonal Architecture, enforcing module boundaries and non-cyclic dependencies through ArchUnit; enforced contract-first API development using OpenAPI.
- Built an asynchronous AI analysis pipeline integrating Deepgram Nova-3 and Gemini Flash using **Java 21 virtual threads**, Resilience4j bulkheads, timeouts, and controlled retries; achieved p95 processing latency under **12 seconds**.
- Implemented deterministic speech scoring using structured LLM outputs and a pure domain core, eliminating LLM-generated scoring decisions; achieved **99% branch coverage across 42 audio fixtures**.
- Engineered concurrency-safe usage quotas and AI cost controls using **atomic SQL updates, unique-key ledgers, idempotency, and sliding-window rate limiting**, preventing quota races and duplicate operations.
- Implemented event-driven workflows using a **transactional outbox, durable webhook inbox, event deduplication, and subscription entitlement synchronization**; integrated account deletion, retention workflows, and Sentry observability.

#### **Distributed URL Shortener with Analytics**
[GitHub Repository](https://github.com/RISHI-SONI345/Distributed-URL-Shortener-with-Analytics)  
*Java, Spring Boot, MySQL, Redis, Docker*

- High-throughput distributed URL shortening system utilizing Base62 encoding, Redis caching (LRU), and Token Bucket rate limiting.
- Designed with click analytics tracking, fault tolerance, and containerized deployment.

---

### 📊 GitHub Activity & Metrics

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=RISHI-SONI345&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=RISHI-SONI345&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" height="165" />
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=RISHI-SONI345&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</div>

---

### 🎓 Education

**Lakshmi Narain College of Technology (LNCT)** *(2022 – 2026)*  
Bachelor of Technology in Computer Science and Engineering — Bhopal, India

---

### 📬 Connect

<p align="center">
  <a href="mailto:rishisoni.tech@gmail.com"><b>rishisoni.tech@gmail.com</b></a> •
  <a href="https://linkedin.com/in/rishi-soni-7427b4252"><b>LinkedIn</b></a> •
  <a href="https://leetcode.com/u/rishisoni1545"><b>LeetCode</b></a> •
  <a href="https://github.com/RISHI-SONI345"><b>GitHub</b></a>
</p>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=RISHI-SONI345&color=6C63FF&style=flat-square&label=Profile+Views" alt="Profile Views" />
</div>
