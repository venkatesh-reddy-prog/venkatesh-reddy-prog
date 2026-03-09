<div align="center">

# B. Venkatesh Reddy

**Backend Engineer** — Java · Spring Boot · Distributed Systems · AWS

[![Portfolio](https://img.shields.io/badge/Portfolio-venkatesh--reddy.vercel.app-4fffb0?style=flat-square&logo=vercel&logoColor=black&labelColor=0a0c10)](https://venkatesh-reddy.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-venkateshy--reddy-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/venkateshy-reddy)
[![Email](https://img.shields.io/badge/Email-bvenkateshreddy87@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:bvenkateshreddy87@gmail.com)
[![AWS](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://venkatesh-reddy.vercel.app/)

<br>

> *Ex-SAP Labs India · M.Tech AI & ML (SRM University, 2025) · **Open to full-time SDE / Backend roles***

</div>

---

## About

I spent 10 months at SAP Labs India building backend services that handle real production traffic — optimising a high-load Spring Boot service by **~30%**, owning test coverage from near-zero to **85%+**, and shipping **3+ production releases**. I also traced a Kubernetes pod memory leak to an unclosed connection pool and proposed decomposing an overloaded service into three smaller ones after noticing unrelated deployments blocking each other.

Outside SAP, I built two systems from scratch to explore problems I found interesting:

- **CodeCollab** — a distributed real-time code editor where I chose Redis Pub/Sub over direct WebSocket broadcast specifically because the editor needed to scale across multiple server instances. Sends only diffs between edits rather than full document state, keeping sync smooth at 50+ concurrent users with sub-100ms latency.

- **Enterprise Knowledge Assistant** — a RAG pipeline where documents are chunked, embedded via OpenAI, and stored in Pinecone. Used recursive character splitting after fixed-size splits produced mid-sentence breaks that degraded retrieval quality. Each service (ingestion, embedding, query) is independently deployable so the embedding model can be swapped without touching ingestion logic.

---

## ⚡ Highlights at a Glance

| Metric | Result |
|--------|--------|
| Service latency reduction | **~30%** |
| Test coverage raised to | **85%+** |
| Production releases shipped | **3+** with zero rollbacks |
| Real-time sync latency | **< 100ms** at 50+ users |
| Granted patents | **1** (IPO No. 565143) |

---

## 🛠 Tech Stack

**Languages**
`Java` `Python` `SQL` `JavaScript` `TypeScript`

**Backend**
`Spring Boot` `Spring MVC` `Spring Security` `Hibernate` `JPA` `FastAPI` `REST APIs` `Microservices` `Kafka` `LangChain`

**Databases**
`PostgreSQL` `MySQL` `MongoDB` `Redis` `Pinecone`

**DevOps & Cloud**
`Docker` `Kubernetes` `Jenkins` `GitHub Actions` `AWS (EC2, S3)` `Linux`

**Concepts**
`Distributed Systems` `System Design` `Event-Driven Architecture` `RAG` `LLM Integration` `CI/CD` `Agile`

---

## 🚀 Projects

### [CodeCollab — Real-Time Collaborative Code Editor](https://github.com/venkatesh-reddy-prog/CodeCollab-Real-Time-Collaborative-Code-Editor)
> `Java` `Spring Boot` `WebSocket` `Redis Pub/Sub` `PostgreSQL` `React.js` `Docker` `AWS EC2` `JWT`

Real-time collaborative code editor built for multi-node scalability.

- **Redis Pub/Sub for cross-node sync** — each server subscribes to a shared channel so users on different instances see edits within sub-100ms
- **Diff-based broadcasting** instead of full document state — keeps sync smooth at 50+ concurrent users per room
- **Immutable PostgreSQL snapshot schema** — makes rollback and session replay trivially correct

🔗 [Live Demo →](https://code-collab-real-time-collaborative.vercel.app)

---

### [Enterprise Knowledge Assistant — AI Semantic Search (RAG)](https://github.com/venkatesh-reddy-prog/enterprise-knowledge-assistant)
> `Java` `Spring Boot` `FastAPI` `LangChain` `OpenAI API` `Pinecone` `PostgreSQL` `React.js` `Docker`

Enterprise RAG platform for semantic search across internal documents.

- **Recursive character chunking** after fixed-size splits degraded retrieval at sentence boundaries
- **Async ingestion pipeline** — large uploads return a job ID immediately, processing happens in background
- **Each service independently deployable** — already used this to swap embedding models without touching ingestion logic

---

## 💼 Experience

### Software Engineer Intern — Backend & DevOps · SAP Labs India
**Aug 2024 – Jun 2025** · 6-person backend team · Java / Spring Boot microservices

- Identified Redis caching gap as the bottleneck in a high-traffic service, cut response time **~30%**
- Replaced manual deployment process with Jenkins + Docker pipelines, shipped **3+ production releases** with **zero deployment rollbacks**
- Traced a recurring Kubernetes pod memory leak to an unclosed connection pool, eliminated the class of incident
- Raised test coverage on two microservices from near-zero to **85%+** with JUnit/Mockito; wired JaCoCo into CI so failing coverage blocks merges

---

## 🏆 Achievements

🏅 **Patent Granted** — No. 565143, Indian Patent Office
*Performance Analysis of Image Retrieval Using Quantized Color Histogram Bins*

📖 **Research Publication** — IGI Global Handbook
*5G-Enabled Secure IoT Applications in Smart Cities*

☁️ **AWS Certified Cloud Practitioner** (2025)

🎓 **M.Tech — Artificial Intelligence & Machine Learning** · SRM University (2025)

---

## 📬 Contact

📍 Bengaluru, India · Open to relocation

| | |
|--|--|
| 🌐 Portfolio | [venkatesh-reddy.vercel.app](https://venkatesh-reddy.vercel.app/) |
| 💼 LinkedIn | [linkedin.com/in/venkateshy-reddy](https://www.linkedin.com/in/venkateshy-reddy) |
| 📧 Email | [bvenkateshreddy87@gmail.com](mailto:bvenkateshreddy87@gmail.com) |
| 💻 GitHub | [github.com/venkatesh-reddy-prog](https://github.com/venkatesh-reddy-prog) |

---

<div align="center">
  <sub>Built with care · Bengaluru, India</sub>
</div>
