<h1 align="center">Yusuf Candır</h1>

<p align="center">
  <b>Software Engineer · Backend · AI/LLM · Cloud</b><br/>
  I build backend systems that stay correct when things fail, and AI systems that show their evidence.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/yusufcandir"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  &nbsp;
  <a href="mailto:yusufcandir30@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## About me

I'm a software engineer working across **backend engineering** and **applied AI**. On the backend I design microservices and serverless APIs with NestJS, Spring Boot and AWS. On the AI side I build LLM and retrieval-augmented generation (RAG) pipelines with explainable machine learning, and I measure how well they ground their answers.

- **Now:** building LLM and RAG systems for cybersecurity at KMUTNB, Thailand
- **Research:** presented TreeSHAP-guided RAG at the SCIN 2026 international conference
- **Cloud:** built serverless backends on AWS at Kuark Dijital
- **Open to:** software engineering roles in backend, full-stack and AI/LLM engineering

## 💼 Experience

**AI Research · LLMs & RAG for Cybersecurity**, King Mongkut's University of Technology North Bangkok (KMUTNB), Thailand
- Designed an explainable pipeline that turns Suricata IDS alerts into evidence-grounded threat reports in Thai and English
- Trained an XGBoost risk classifier (97.5% accuracy, 0.960 macro F1) and used TreeSHAP to rerank retrieved evidence
- Built a FAISS knowledge base of 885,273 chunks from NVD, CVE, CWE and MITRE ATT&CK, served a local LLM (Typhoon2) with Ollama, and added claim-level citation guardrails
- Ran a controlled evaluation of 1,000 generated reports; retrieval cut attributional hallucination from 86% to 0%

**Backend Development · AWS Serverless**, Kuark Dijital
- Built backend services and APIs for web and mobile apps on AWS Lambda, API Gateway, AppSync, Cognito and S3

## 🚀 Featured projects

### 🛡️ [TreeSHAP-Guided RAG for Thai–English IDS Alert Reporting](https://github.com/Yusufcandir/LLM-based-Threat-and-Vulnerability)
Converts raw Suricata IDS alerts into structured, evidence-grounded security reports in Thai and English. It explains each decision as a chain: what the model decided (XGBoost risk class), which features drove it (TreeSHAP), and why they matter (RAG evidence reranked by SHAP importance).
- Hierarchical retrieval: exact CVE → CWE → ATT&CK lookup, then signature search, then semantic FAISS search, with abstention when there is no evidence
- Three-level citation guardrail that checks each claim against valid, supporting sources
- Fully local stack with no cloud LLM API; evaluated with BERTScore, a hallucination taxonomy (H1–H5) and significance tests

`Python` `XGBoost` `SHAP` `FAISS` `sentence-transformers` `Ollama` `Typhoon2`

### 🔁 [Takasla: Trust-Enhanced C2C Exchange Platform](https://github.com/Yusufcandir/takasla)
A peer-to-peer exchange platform for high-value goods, with risk-based escrow, fraud detection and blockchain-anchored trade certificates.
- 12 NestJS microservices behind an API gateway, with one PostgreSQL database per service and RabbitMQ events using the outbox pattern
- Trade state machine with 19 states, saga orchestration with compensating steps, Redis distributed locks, idempotency keys and optimistic locking
- Risk scoring that sets verification level, dispute window and shipping flow; trade certificates anchored on Ethereum Sepolia with Merkle trees
- AI-generated image detection for listings, multi-carrier shipping webhooks, and KVKK (Turkish data protection) compliance
- Next.js user and admin apps; deployed with Docker Compose behind Caddy with automatic TLS

`TypeScript` `NestJS` `PostgreSQL` `RabbitMQ` `Redis` `Next.js` `Docker` `Solidity`

### 🤖 [backend-dev-kit](https://github.com/Yusufcandir/backend-dev-kit-claude) · [Codex edition](https://github.com/Yusufcandir/backend-dev-kit-codex)
A plugin for **Claude Code** and the **OpenAI Codex CLI** that takes a backend task end to end: analysis and roadmap, implementation, then review. It ships skills for each stage plus four agents (researcher, OWASP-based security auditor, test engineer and backend coder) that run the review checks in parallel.

`AI agents` `Claude Code` `Codex CLI` `Developer tooling`

### 📸 [FotoFocus](https://github.com/Yusufcandir/FotoFocus-App)
A mobile app for learning photography, with structured lessons, photo challenges, star ratings and a community feed.
- Flutter client using Provider; REST API built with Node.js, Express, Prisma and PostgreSQL
- JWT authentication with email verification, Cloudinary image uploads, follows, and account deletion that cascades through the backend

`Flutter` `Dart` `Node.js` `Express` `Prisma` `PostgreSQL`

### 🚗 [Crashlytics](https://github.com/Yusufcandir/Crashlytics)
A road-safety platform that predicts accident severity and computes road safety scores from historical accident records, with an interactive accident map and filters.

`Python` `scikit-learn` `Pandas` `Flask` `Node.js` `Express`

## 🛠️ Tech stack

| Area | Tools |
|---|---|
| **Languages** | <img src="https://skillicons.dev/icons?i=java,python,ts,js,dart&theme=dark" alt="Java, Python, TypeScript, JavaScript, Dart"/> |
| **Backend** | <img src="https://skillicons.dev/icons?i=spring,hibernate,nodejs,nestjs,express,flask,graphql&theme=dark" alt="Spring Boot, Hibernate, Node.js, NestJS, Express, Flask, GraphQL"/> |
| **Data & messaging** | <img src="https://skillicons.dev/icons?i=postgres,mysql,redis,rabbitmq,prisma&theme=dark" alt="PostgreSQL, MySQL, Redis, RabbitMQ, Prisma"/> |
| **AI / ML** | <img src="https://skillicons.dev/icons?i=python,sklearn&theme=dark" alt="Python, scikit-learn"/><br/>XGBoost · SHAP · FAISS · RAG · Ollama · sentence-transformers · Whisper · Pandas |
| **Frontend & mobile** | <img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,flutter&theme=dark" alt="React, Next.js, Tailwind CSS, Flutter"/> |
| **Cloud & DevOps** | <img src="https://skillicons.dev/icons?i=aws,docker,githubactions,jenkins,linux,git&theme=dark" alt="AWS, Docker, GitHub Actions, Jenkins, Linux, Git"/><br/>Lambda · API Gateway · AppSync · Cognito · S3 · Caddy |

## 📫 Get in touch

I'm happy to talk about backend architecture, LLM/RAG systems or new opportunities. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/yusufcandir) or [email](mailto:yusufcandir30@gmail.com).
