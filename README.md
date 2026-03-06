# B. Venkatesh Reddy

**Backend Engineer** — Java · Spring Boot · Distributed Systems · AWS

Ex-SAP Labs India · M.Tech AI & ML (SRM University, 2025) · **Available for full-time SDE / Backend roles**

---

## About

I spent 10 months at SAP Labs India building backend services that handle real production traffic — optimising a high-load Spring Boot service by ~30%, owning test coverage from near-zero to 85%+, and shipping 3+ production releases. I also traced a Kubernetes pod memory leak to an unclosed connection pool and proposed decomposing an overloaded service into three smaller ones after noticing unrelated deployments blocking each other.

Outside SAP, I built two systems from scratch to explore problems I found interesting:

- **CodeCollab** — a distributed real-time code editor where I chose Redis Pub/Sub over direct WebSocket broadcast specifically because the editor needed to scale across multiple server instances. Sends only diffs between edits rather than full document state, keeping sync smooth at 50+ concurrent users with sub-100ms latency.

- **Enterprise Knowledge Assistant** — a RAG pipeline where documents are chunked, embedded via OpenAI, and stored in Pinecone. Used recursive character splitting after fixed-size splits produced mid-sentence breaks that degraded retrieval quality. Each service (ingestion, embedding, query) is independently deployable so the embedding model can be swapped without touching ingestion logic.

I hold a granted Indian patent (No. 565143) from the Indian Patent Office and a published research chapter in an IGI Global handbook on 5G-enabled IoT applications.

---

## Tech Stack

**Languages:** Java · Python · SQL · JavaScript · TypeScript  
**Backend:** Spring Boot · Spring MVC · Spring Security · Hibernate · JPA · FastAPI · REST APIs · Microservices · Kafka · LangChain  
**Databases:** PostgreSQL · MySQL · MongoDB · Redis · Pinecone  
**DevOps & Cloud:** Docker · Kubernetes · Jenkins · GitHub Actions · AWS (EC2, S3) · Linux  
**Concepts:** Distributed Systems · System Design · Event-Driven Architecture · RAG · LLM Integration · CI/CD · Agile

---

## Projects

### [CodeCollab — Real-Time Collaborative Code Editor](https://github.com/venkatesh-reddy-prog/CodeCollab-Real-Time-Collaborative-Code-Editor)

Real-time collaborative code editor built for multi-node scalability.

`Java` `Spring Boot` `WebSocket` `Redis Pub/Sub` `PostgreSQL` `React.js` `Docker` `AWS EC2` `JWT`

- Redis Pub/Sub for cross-node sync — each server subscribes to a shared channel so users on different instances see edits within sub-100ms
- Diff-based broadcasting instead of full document state — kept sync smooth at 50+ concurrent users per room
- Immutable PostgreSQL snapshot schema — makes rollback and session replay trivially correct
- Live demo: [code-collab-real-time-collaborative.vercel.app](https://code-collab-real-time-collaborative.vercel.app)

---

### [Enterprise Knowledge Assistant — AI Semantic Search (RAG)](https://github.com/venkatesh-reddy-prog/enterprise-knowledge-assistant)

Enterprise RAG platform for semantic search across internal documents.

`Java` `Spring Boot` `FastAPI` `LangChain` `OpenAI API` `Pinecone` `PostgreSQL` `React.js` `Docker`

- Recursive character chunking after fixed-size splits degraded retrieval at sentence boundaries
- Async ingestion pipeline — large uploads return a job ID immediately, processing happens in background
- Each service independently deployable — already used this to swap embedding models without touching ingestion logic

---

## Experience

**Software Engineer Intern — Backend & DevOps** · SAP Labs India · Aug 2024 – Jun 2025

Worked in a 6-person backend team on production Java/Spring Boot microservices. Key work:
- Identified Redis caching gap as the bottleneck in a high-traffic service, cut response time ~30%
- Replaced manual deployment process with Jenkins + Docker pipelines, shipped 3+ production releases with zero deployment rollbacks
- Traced a recurring Kubernetes pod memory leak to an unclosed connection pool, eliminated the class of incident
- Raised test coverage on two microservices from near-zero to 85%+ with JUnit/Mockito; wired JaCoCo into CI so failing coverage blocks merges

---

## Achievements

- 🏅 **Patent Granted** — No. 565143, Indian Patent Office — *Performance Analysis of Image Retrieval Using Quantized Color Histogram Bins*
- 📖 **Research Publication** — *5G-Enabled Secure IoT Applications in Smart Cities* — IGI Global Handbook
- ☁️ **AWS Certified Cloud Practitioner** (2025)

---

## Contact

[LinkedIn](https://www.linkedin.com/in/venkateshy-reddy) · [Email](mailto:bvenkateshreddy87@gmail.com) · Bengaluru, India · Open to relocation
