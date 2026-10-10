<div align="center">

<h1>Kasra Karami</h1>

<p><strong>Technical Lead &nbsp;·&nbsp; Full-Stack Software Engineer &nbsp;·&nbsp; Distributed Systems &amp; Applied AI</strong></p>

<p>
Head of Technical Development — <a href="https://www.techsuite.ai/">Techsuite</a>, London, United Kingdom<br/>
Technical Lead (Contract) — Embargo, London, United Kingdom
</p>

<p>
<a href="https://www.linkedin.com/in/kasra-karami/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Kasra%20Karami-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="https://orcid.org/0009-0005-3299-370X"><img alt="ORCID" src="https://img.shields.io/badge/ORCID-0009--0005--3299--370X-A6CE39?style=for-the-badge&logo=orcid&logoColor=white"/></a>
<a href="mailto:kasra.karami.dev@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-Get%20in%20touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://www.techsuite.ai/"><img alt="Website" src="https://img.shields.io/badge/Web-techsuite.ai-1A2E4A?style=for-the-badge&logo=googlechrome&logoColor=white"/></a>
</p>

</div>

---

## Professional Summary

Technical Lead with **9+ years of professional experience** architecting, building and launching complex digital products across **hospitality, financial technology and SaaS**. I own technical direction end to end — architecture, platform implementation, and the delivery of **AI-powered, high-throughput, mission-critical systems used by millions of customers**.

Since 2021 I have led engineering for **UK technology companies** — first as Technical Lead at **Embargo (London)** and currently as **Head of Technical Development at Techsuite (London)** — building multi-tenant SaaS platforms, real-time distributed systems and production AI capabilities, alongside the teams, standards and processes that keep them sustainable.

My work sits at the intersection of **systems architecture, applied AI and engineering leadership**: translating business strategy into technical reality, scaling engineering organisations, and raising the technical level of everyone around me.

---

## Leadership &amp; Technical Direction

- **Own technical strategy end to end** — architecture, scalability and availability planning, technology selection, and delivery across multiple concurrent products.
- **Set engineering standards** — authored the coding standards, naming conventions and architectural guidelines adopted across all engineering teams, documented via **Architecture Decision Records**.
- **Build and grow teams** — own the full technical hiring pipeline (assessment design, interviews, final decisions), personally onboard every new engineer, and mentor across all seniority levels through regular one-to-ones.
- **Drive engineering process** — introduced retrospectives, async stand-ups, a structured technical-debt pipeline (later AI-assisted), API versioning policy, and a full unit / integration / E2E testing strategy with CI/CD integration.
- **Represent engineering externally** — lead technical due diligence and architecture reviews with third-party vendors, translating outcomes into execution plans.
- **Align business and engineering** — sprint planning across multiple products, trade-off analysis across time, cost, quality and risk, and stakeholder communication before commitment.

---

## Selected Impact

| Domain | Outcome |
| :-- | :-- |
| **Scale** | Architected and led delivery of customer-facing web platforms serving **1.65M+ active users** with high reliability |
| **Product quality** | Systematically rebuilt a flagship mobile application, driving it to a **4.8 App Store rating** |
| **Revenue** | Delivered an e-commerce platform that outperformed physical branches, contributing to a **35% revenue increase** within six months |
| **Delivery speed** | Jenkins CI/CD with automated testing cut deployment time by **40%**; an API-first workflow increased delivery speed by **25%** |
| **Engineering efficiency** | A centralised Node.js error handler that resolves exact file, line and context cut debugging time by **~50%** across all backend projects |
| **Automation** | A Go web scraper reduced per-product data entry from **5–6 minutes to under a second** |
| **Content operations** | A no-code drag-and-drop site and landing page builder cut content deployment time by **60%** |
| **Performance** | SSR rewrite improved initial load by **30%** and SEO by **20%**; frontend optimisation delivered up to **60%** improvement |
| **Integration breadth** | Led end-to-end integration of **25+ third-party services**, owning implementation and provider relationships |
| **Onboarding** | Structured API documentation (Swagger, Compodoc, Confluence, Miro) cut developer onboarding time by **50%** and support queries by **30%** |

---

## Innovation &amp; Original Technical Contributions

Systems I have designed and built that did not exist before, several of which are open source and in use beyond the organisation that commissioned them.

**Applied AI &amp; machine learning**

- **AI notification engine** — a production system for a multi-tenant F&amp;B SaaS platform combining **item-based collaborative filtering** with **LLM personalisation** to generate unique push notifications per customer, segmented by habit stage, with deterministic **A/B testing across eight copy variants** and open-rate reporting via an append-only event table.
- **Three-phase AI campaign pipeline** — operators brief an LLM conversationally, bulk copy is streamed over **SSE**, and campaigns enter an approval queue before dispatch, removing the need for technical knowledge to run personalised CRM campaigns.
- **Cron dispatch architecture** — a five-minute dispatch loop with **Firebase Cloud Messaging** batch delivery and a **three-layer suppression system** (eligibility, generation, send-time) preventing duplicate sends against live PostgreSQL order data.
- **AI support assistant** — automatic knowledge-base synchronisation plus a streaming **WebSocket** pipeline that answers questions in real time with direct links to source documentation.
- **Internal vector search engine** built on proprietary data for semantic retrieval and knowledge discovery, plus an **OCR pipeline** that converts photographed receipts from API-less POS systems into structured orders to keep inventory and accounting in sync.

**Platform &amp; distributed systems**

- **Multi-tenant architecture** where each business runs on an isolated database and service instance, with login-aware routing that resolves the correct tenant for every API call automatically.
- **Observability stack built from scratch** — a Go activity-logging service and a **Rust log aggregator** tied into Elastic Stack, APM and Grafana for metrics, tracing and log analysis across services.
- **Redis Pub/Sub WebSocket fan-out** for consistent real-time delivery across clustered nodes, and **Redis caching plus gRPC** inter-service communication to materially reduce latency versus REST.
- **Worldpay payment service over STOMP WebSockets** with full event lifecycle management, heartbeat monitoring, automatic disconnect on failure and worker-offloaded concurrent processing.
- **Protocol-complete authentication layers** across TCP, GraphQL, WebSocket and gRPC, plus a centralised Node.js/Express **API Gateway** and a versioned **gRPC SDK** distributed as a private NPM package.
- **Samsung Tizen TV application** for restaurant digital signage — published to the Samsung store — with real-time menu sync over WebSocket, schedule-based content switching, live stock updates and QR-code login to bypass TV input constraints.

**Developer tooling**

- **Rust CLI** that scaffolds backend modules, eliminating boilerplate and enforcing consistent architecture across teams.
- **Custom ORM** that auto-generates queries and boilerplate for common database operations across all team projects.
- **Email templating framework with a CLI** that compiles components into email-client-compatible HTML, plus a **drag-and-drop receipt template builder** extended to cloud printers without template changes.
- **Shared UI component library** on top of Quasar, distributed as a Git submodule to standardise components, spacing and styling across projects.

---

## Open Source Work

| Project | Description | Stack |
| :-- | :-- | :-- |
| **[SchemaLoom](https://github.com/KasraK2K/SchemaLoom)** | Visual database design workspace: ERD canvas, per-object documentation, and an AI query assistant scoped strictly to what the user has selected and is permitted to see. SQL import, per-area sharing permissions. | TypeScript |
| **[ReqLoom](https://github.com/KasraK2K/ReqLoom)** | Self-hosted API workspace for building, sending, organising and tracing HTTP requests, with environments, history, Postman import and realtime team sync. | TypeScript |
| **[PM2Operator](https://github.com/KasraK2K/PM2Operator)** | Full-stack PM2 operations console for managing remote SSH hosts, inspecting Node.js processes, streaming live logs and running PM2 actions from a shared dashboard. | TypeScript |
| **[TranslateHub](https://github.com/KasraK2K/TranslateHub)** | Self-hosted translation management platform that moves application copy out of the codebase and serves it at runtime via API, with a web admin UI. | JavaScript · MIT |
| **[go-simple-monitoring](https://github.com/KasraK2K/go-simple-monitoring)** | Infrastructure monitoring tool aggregating CPU, RAM and PM2 service metrics from multiple servers into a single dashboard, with optional GUI mode. **Adopted across multiple companies.** | Go |
| **[Cloak-Windows](https://github.com/KasraK2K/Cloak-Windows)** | Windows port of an SNI-spoofing and Xray-based internet access tool, extending open internet access to a platform the original did not support. | Python · GPL-3.0 |
| **[clean-boilerplate](https://github.com/KasraK2K/clean-boilerplate)** · **[backend-solution](https://github.com/KasraK2K/backend-solution)** | Domain-Driven Design and production-grade Node.js starters covering error handling, validation, logging and monitoring. | TypeScript |
| **[graphql-rest-grpc-socket](https://github.com/KasraK2K/graphql-rest-grpc-socket)** · **[microservice-blog](https://github.com/KasraK2K/microservice-blog)** | Reference implementations of multi-protocol services and a full microservice system (gateway, user, article, asset, support). | TypeScript |
| **[rust-cli-ts](https://github.com/KasraK2K/rust-cli-ts)** · **[rust-cleanup](https://github.com/KasraK2K/rust-cleanup)** | Rust command-line tooling for TypeScript project scaffolding and resource-critical Linux maintenance. | Rust |
| **[project-base-recsys](https://github.com/KasraK2K/project-base-recsys)** · **[RecSysMovie](https://github.com/KasraK2K/RecSysMovie)** | Recommender-system research and reference implementations underpinning production personalisation work. | Python |

---

## Community, Mentorship &amp; Knowledge Sharing

Teaching has been part of my practice since I started programming in 2010.

- **Run regular internal training** across JavaScript, TypeScript, Node.js, React and Vue, raising the technical level of entire engineering departments.
- **Lead periodic code reviews** and own code quality standards across backend and frontend projects.
- **Publish open educational material** — [You-Dont-Know-JavaScript](https://github.com/KasraK2K/You-Dont-Know-JavaScript), [goLang-Course](https://github.com/KasraK2K/goLang-Course), [Event-Loop-Course](https://github.com/KasraK2K/Event-Loop-Course) and [Made-In-Iran-APIs](https://github.com/KasraK2K/Made-In-Iran-APIs), a community-referenced index of public APIs.
- **Contribute upstream** to the wider ecosystem, including the [Vue.js](https://github.com/vuejs/core) organisation.
- **Recognitions** — **GitHub Developer Program Member**, **Arctic Code Vault Contributor**, Pair Extraordinaire ×3, Pull Shark ×2, with **205 repositories** and **1,270+ contributions** in the past year.

---

## Career Timeline

| Period | Role | Organisation | Location |
| :-- | :-- | :-- | :-- |
| 2024 — present | **Engineering Lead / Head of Technical Development** | Techsuite | London, UK (Remote) |
| 2021 — present | **Technical Lead** (Independent Contractor) | Embargo | London, UK (Remote) |
| 2019 — 2021 | **Senior Software Engineer (Full-Stack) &amp; Frontend Technical Lead** | Jeanswest | Tehran, Iran |
| 2018 — 2019 | **Full-Stack Developer** | Roobitech | Canada (Remote) |
| 2016 — 2018 | **Backend Developer** | Pishrobot | Tehran, Iran |

**International delivery:** Techsuite (UK) · Embargo App (UK, Poland) · Mododuo (UK) · GrillaTech (UK) · Compare Electrical Car (UK)

---

## Technology

**Languages** &nbsp; TypeScript · JavaScript · Go · Rust · Python · SQL

**Backend** &nbsp; Node.js · Express · NestJS · gRPC · GraphQL · REST · WebSocket · STOMP · TCP · RabbitMQ · Redis Pub/Sub · Worker Threads

**Frontend** &nbsp; React · Next.js · Vue · Nuxt · Quasar · Storybook · PWA · SSR · Samsung Tizen

**Data** &nbsp; PostgreSQL · MongoDB · Redis · Elasticsearch · Vector search

**AI &amp; ML** &nbsp; LLM integration (Claude, OpenAI) · RAG &amp; semantic retrieval · Collaborative filtering · Recommender systems · OCR pipelines

**Infrastructure** &nbsp; Docker · Jenkins · CI/CD · Load balancing · DigitalOcean · Firebase Cloud Messaging · Elastic Stack · APM · Grafana · PM2

**Practice** &nbsp; Domain-Driven Design · Microservices · Multi-tenancy · Event-driven architecture · SOLID · Architecture Decision Records · API versioning · Unit / Integration / E2E testing

---

## Education &amp; Professional Identity

- **B.Sc. in Executive Civil Engineering** — Azad University (IAU), Arak, Iran, 2016
- **ORCID** — [0009-0005-3299-370X](https://orcid.org/0009-0005-3299-370X)
- **Nine years** of continuous professional software engineering practice, self-directed from first principles

---

<div align="center">

<img height="150" alt="GitHub statistics" src="https://github-readme-stats.vercel.app/api?username=KasraK2K&show_icons=true&hide_border=true&include_all_commits=true&count_private=true"/>
<img height="150" alt="Most used languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=KasraK2K&layout=compact&hide_border=true&langs_count=8"/>

</div>

---

## Contact

I am always open to conversations about **engineering leadership, distributed systems architecture, applied AI**, and collaboration with teams building ambitious products.

<div align="center">

[**LinkedIn**](https://www.linkedin.com/in/kasra-karami/) &nbsp;·&nbsp; [**Email**](mailto:kasra.karami.dev@gmail.com) &nbsp;·&nbsp; [**ORCID**](https://orcid.org/0009-0005-3299-370X) &nbsp;·&nbsp; [**Techsuite**](https://www.techsuite.ai/)

</div>
