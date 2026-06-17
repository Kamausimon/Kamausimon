# Hi, I'm Simon Kamau 👋

## AWS Certified Solutions Architect | Backend Engineer | Go · Rust · Node.js

I build cloud-native backend systems that handle real money and real users at scale.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/simon-kamau-codes/)
[![AWS Certified](https://img.shields.io/badge/AWS-Solutions_Architect_Associate-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://www.credly.com/badges/2c9e8d15-5e27-4bae-b869-636b11213b92/public_url)
[![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/Kamau_codes)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://kamausimon.vercel.app/)
[![TikTok](https://img.shields.io/badge/TikTok-%23000000.svg?logo=TikTok&logoColor=white)](https://tiktok.com/@kamau_codes)

[![wakatime](https://wakatime.com/badge/user/018c5a56-9679-4410-abca-5b63505115e4.svg)](https://wakatime.com/@018c5a56-9679-4410-abca-5b63505115e4)

---

## 🚀 Featured Projects

### [🎫 Event Ticketing Platform](https://github.com/kamausimon/ticketing_system) — Go · PostgreSQL · Redis · Kafka · AWS

Production-grade event ticketing platform built and **deliberately rebuilt three times** to demonstrate architectural progression — from a monolith to event-driven microservices to a fully cloud-native AWS deployment. Each version is a complete, runnable application implementing the same domain: authentication, payments, PDF ticket generation, real-time inventory, refund workflows, analytics, and email delivery.

| Version | Architecture | Key Technologies |
|---------|-------------|-----------------|
| **v1** | Monolithic REST API | Go, PostgreSQL, Redis, S3 |
| **v2** | Event-driven microservices | Go, Apache Kafka, PostgreSQL, Redis, S3 |
| **v3** | Cloud-native on AWS | Go, SNS/SQS, Aurora PostgreSQL, ElastiCache, S3, Terraform |

- **1,000+ concurrent users** · 99.9% uptime · sub-200ms response times validated under K6 load testing
- Latency reduced **450ms → 120ms** via query optimisation and connection pooling
- JWT + TOTP 2FA · Stripe, IntaSend & M-Pesa payments · 5-tier rate limiting
- **11 independent worker binaries** in v2/v3 (payment, ticket, email, refund, waitlist, analytics, etc.) communicating via Kafka topics and the **transactional outbox pattern** — guaranteeing zero event loss under failure
- v3 infrastructure fully provisioned with **Terraform**: SNS, SQS (14 queues + DLQs), Aurora, ElastiCache
- Prometheus + Grafana monitoring tracking 20+ KPIs with real-time alerting
- AI-assisted admin support ticket classification · promotional codes · organiser payout management
- **60+ test cases** · 85% coverage · TDD methodology

`Go 1.22` `PostgreSQL` `Redis` `Apache Kafka` `Amazon SNS/SQS` `Aurora PostgreSQL` `ElastiCache` `Docker` `Terraform` `AWS EC2` `AWS S3` `Nginx` `Prometheus` `Grafana` `Stripe` `IntaSend` `JWT` `TOTP`

🔗 [Live Demo](https://ticketing-system-steel-zeta.vercel.app/) | 📖 [API Docs](https://documenter.getpostman.com/view/28274964/2sBXVhCqZ2) | [Repository](https://github.com/Kamausimon/ticketing_system)

---

### [🦀 Sokavi — Service Provider Marketplace](https://github.com/Kamausimon/mtaalink) — Rust · Axum · PostgreSQL · AWS

High-performance Kenyan marketplace backend connecting clients, service providers, and businesses — built in Rust for maximum throughput with a 23-table PostgreSQL schema and 30+ REST endpoints.

- **<300ms p95 latency** · 20K+ monthly requests · compile-time-verified SQLx queries
- **M-Pesa Daraja STK Push** payments with automatic booking confirmation and wallet crediting; Africa's Talking SMS for booking and payment alerts
- **Real-time WebSocket** messaging and in-app notification system using Axum's built-in WS + tokio broadcast channels
- **PostgreSQL full-text search + haversine geo-proximity** supporting 10,000+ provider listings with optimised indexing
- Provider analytics dashboard (revenue, bookings over time, top services, repeat client rate), wallet & payout flows, and verified reviews gated behind completed bookings
- Service package bundling · weekly availability scheduling · favourites with real-time post alerts
- Manual AWS S3 v4 request signing — no SDK required · switchable local/S3 storage backend via env var
- tower-governor rate limiting (5 req/min on auth, 100 req/min global) · Argon2 password hashing
- 35% reduction in operational costs via caching and rate limiting · 12 incremental SQL migrations auto-applied at startup

`Rust` `Axum` `PostgreSQL` `SQLx` `AWS S3` `WebSockets` `M-Pesa Daraja` `Africa's Talking` `Docker` `JWT` `Argon2` `Tokio`

📖 [GitHub](https://github.com/Kamausimon/sokavi) | 🔗 [Live Version](https://sokavi.vercel.app/)verc

---

### [🏪 Multi-Tenant Inventory SaaS](https://github.com/Kamausimon/MTIS) — Node.js · MongoDB

Multi-tenant SaaS inventory platform with full tenant isolation and role-based access control.

- **50+ business tenants** with 100% data isolation
- RBAC managing **150+ users** with granular permissions
- Dashboard load time reduced **50%** via MongoDB aggregation pipeline optimisation
- CI/CD pipeline with automated rollback on Railway

`Node.js` `MongoDB` `Redis` `Docker` `GitHub Actions` `JWT`

📖 [GitHub](https://github.com/Kamausimon/MTIS)

---

## 🛠️ Tech Stack

**Languages**

![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)

**Backend & Frameworks**

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white)

**Messaging & Event-Driven**

![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka)
![Amazon SNS](https://img.shields.io/badge/Amazon%20SNS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Amazon SQS](https://img.shields.io/badge/Amazon%20SQS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)

**Databases**

![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

---

## 📈 GitHub Stats

<div align="center">

[![Kamausimon's GitHub stats](https://github-readme-stats-eight-theta.vercel.app/api?username=Kamausimon&show_icons=true&theme=material-palenight&include_all_commits=true&count_private=true)](https://github.com/Kamausimon)

![](https://nirzak-streak-stats.vercel.app/?user=kamausimon&theme=dark&hide_border=false)

![](https://github-readme-stats.vercel.app/api/top-langs/?username=kamausimon&theme=dark&hide_border=false&include_all_commits=true&count_private=true&layout=compact)

</div>

---

## 🎯 Currently

- ☁️ **Certified:** AWS Solutions Architect Associate (SAA-C03) — 2026
- 📚 **Learning:** Kubernetes · Terraform · AWS Certified DevOps Engineer – Professional
- 💼 **Open to:** Backend Engineer, Cloud Engineer, or Solutions Architect roles
- 🌍 **Location:** Nairobi, Kenya · Remote-friendly

---

## 📫 Let's Connect

- 📧 [kamausimon217@gmail.com](mailto:kamausimon217@gmail.com)
- 💼 [linkedin.com/in/simon-kamau-codes](https://linkedin.com/in/simon-kamau-codes/)
- 🌐 [kamausimon.vercel.app](https://kamausimon.vercel.app/)
- 🐦 [@Kamau_codes](https://x.com/Kamau_codes)

---

<div align="center">

### 💼 Open to Backend · Cloud · Solutions Architect Roles | 🌍 Remote or Nairobi, Kenya

**"Code that works in production, not just on localhost"**

[![](https://visitcount.itsvg.in/api?id=kamausimon&icon=0&color=0)](https://visitcount.itsvg.in)

</div>
