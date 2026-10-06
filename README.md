<div align="center">

# Sang Thai — AI Solution and Data Engineer 👋

### **AI Solution and Data Engineer** · M.S. candidate in AI and Digital Transformation @ USF — I build pipelines that hold up in production, and AI systems on top of them.

<p>
  <a href="https://sangthai.dev">
    <img src="https://img.shields.io/badge/Portfolio-sangthai.dev-2ea043?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio"/>
  </a>
  <a href="https://www.linkedin.com/in/sang-thai/">
    <img src="https://img.shields.io/badge/LinkedIn-sang--thai-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:thaisangcr7@gmail.com">
    <img src="https://img.shields.io/badge/Email-thaisangcr7@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

<p>
  <img src="https://img.shields.io/badge/Open_to-Work-blue?style=for-the-badge" alt="Open to work"/>
  <img src="https://img.shields.io/badge/Data_Engineering-2ea043?style=for-the-badge" alt="Data Engineering"/>
  <img src="https://img.shields.io/badge/AI_Engineering-7c3aed?style=for-the-badge" alt="AI Engineering"/>
  <img src="https://img.shields.io/badge/Backend-ff8c00?style=for-the-badge" alt="Backend"/>
</p>

</div>

---

### About me

At **Citi** I was the sole developer behind **ATLAS**, a controls-testing platform architected for **~25M records/month** across 52 payment applications, built in partnership with Operational Risk stakeholders. It validated locally end-to-end before a reorg shifted priorities.

I came up through data — Finance degree from USF, then Wells Fargo and Raymond James doing SQL-heavy operations and pipeline work (schema design, Control-M batch scheduling) — and taught myself software engineering properly along the way: Python → data pipelines → backend APIs → cloud infrastructure → applied AI. Now formalizing it with an **M.S. in AI in Business & Enterprise Integration** (expected Dec 2027).

My edge: I don't just move data, I make it *usable* — RAG pipelines, verifiable document extraction, and analytics layers teams actually query.

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=thaisangcr7&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=thaisangcr7&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages"/>
</div>

---

## 🚀 Featured Projects

### 🎙️ avenotes.ai — [Live site →](https://avenotes.ai)

**Shipped SaaS: AI meeting notes without the bot.**

Browser-based meeting note-taker — no bot joins the call. Live transcription, structured recaps, cross-meeting memory. Designed, built, and launched.

<p align="center">
  <img src="images/avenotes-hero.jpg" width="720" alt="Avenotes — your second mind for every meeting"/>
</p>
<p align="center">
  <img src="images/avenotes-memory.jpg" width="352" alt="Avenotes remembers — you just ask"/>
  <img src="images/avenotes-recap.jpg" width="352" alt="Avenotes recap — walk out knowing exactly what was said"/>
</p>

---

### 📊 [Automated Portfolio Analytics Pipeline](https://github.com/thaisangcr7/Automated-Portfolio-Analytics-Pipeline)

**End-to-end ELT: Yahoo Finance → PostgreSQL → dbt → Metabase, orchestrated by Airflow.**

Daily stock prices flow through a medallion architecture — Bronze (raw, append-only) → Silver (cleaned, enriched) → Gold (marts) — with data quality tests gating every run.

| | |
|---|---|
| ⏰ Orchestration | Airflow DAG, weekdays 6 PM: ingest → seed → dbt run → test |
| 🥉🥈🥇 Modeling | 5 dbt models across three layers · **26 data quality tests** |
| 📈 BI | Metabase dashboard: value, P&L, moving averages |
| 🐳 Infra | Fully containerized in Docker |

<p align="center">
  <img src="https://sangthai.dev/images/portfolio_analysis.png" width="720" alt="Portfolio Analytics Dashboard"/>
</p>

---

### 🥑 [Avocado](https://github.com/thaisangcr7/avocado)

**Grounded AI over your team's data.**

A copilot that answers from documents with cited sources — or writes Python, runs it against your data in a locked-down sandbox, and shows you the code behind the number. Handles **110,000+ row** datasets.

`Python` `FastAPI` `PostgreSQL` `pgvector` `Redis` `Docker` `React` `TypeScript` — **757 tests · CI green**

<p align="center">
  <img src="https://sangthai.dev/images/avocado-cited.jpg" width="720" alt="Avocado answering with cited sources"/>
</p>

---

### 🔎 [credit-rag](https://github.com/thaisangcr7/credit-rag)

**Verifiable RAG for financial documents.**

Extracts structured terms from 200+ page credit agreements — every value traced to its source sentence; unverifiable values return **not found**, never hallucinated. Two-stage retrieval (pgvector + local cross-encoder), Kafka-backed idempotent ingestion, eval harness included (**64 tests · CI green**).

---

### 📡 [SENTINEL](https://github.com/thaisangcr7/SENTINEL)

**Production-grade data pipeline on AWS.**

Economic indicator monitoring (FRED API → PostgreSQL → anomaly alerts via FastAPI). Infrastructure fully defined in Terraform, deploys gated on the test suite, security-audited before launch (**6 vulnerabilities fixed**), ran live on AWS for five months.

---

## 🧰 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,typescript,sql,fastapi,flask,postgres,redis,kafka,docker,kubernetes,terraform,aws,azure,react,angular,cs,dotnet,git,githubactions,vscode" alt="Tech stack"/>
</p>

| Area | |
|---|---|
| **Data** | Airflow · dbt · Kafka · PostgreSQL · pgvector · SQL Server · Pandas · Metabase |
| **AI** | RAG · Vector search · Cross-encoder reranking · Eval harnesses · Sandboxed code execution · Claude API · Deepgram |
| **Backend** | FastAPI · Flask · ASP.NET Core · REST · WebSockets · async Python |
| **Infra** | Docker · Kubernetes · Terraform · AWS · Azure · GitHub Actions · CI/CD |

---

## 📈 By the numbers

| | |
|---|---:|
| Records/month ATLAS was architected for | **~25M** |
| Manual effort it was designed to remove | **~90%** |
| Payment applications covered | **52** |
| dbt models / data quality tests | **5 / 26** |
| Avocado automated tests | **757** |
| Largest dataset computed in full | **110,064 rows** |

---

## 📬 Currently

- 📊 Building data systems that hold up in production
- 🎙️ Growing **avenotes.ai**
- 🎓 M.S. in AI & Digital Transformation @ USF
- 💼 Open to **Data Engineering, AI Engineering, and Frontend/Backend** roles — [let's talk](mailto:thaisangcr7@gmail.com)
- ⚽ Playing soccer whenever I can

---

<div align="center">

🌐 [sangthai.dev](https://sangthai.dev) · 💼 [LinkedIn](https://www.linkedin.com/in/sang-thai/) · 📧 thaisangcr7@gmail.com

</div>
