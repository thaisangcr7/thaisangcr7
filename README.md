## Hi 👋, I'm Sang.

**AI / Backend Engineer** · Automation & Data Engineering at Citibank · Tampa, FL

I build retrieval and analysis systems — things that answer from real
documents and data and can show their work. Day to day that means
production automation for financial operations at Citi, turning manual,
error-prone workflows into reliable ones.

---

### What I'm building

**ATLAS** — It started with a simple initiative: a team manually
reconciling payment records every month across spreadsheets, burning
days of work just to catch errors that a machine could find in
seconds. So I built one. ATLAS is a config-driven Python automation
platform I designed and built entirely solo at Citi. It processes
~25M records/month across 52 global payment applications — running 4
pipeline types: Threshold Validation, Duplicate Detection, Dual Blind
Rekey, and GPOC executive reporting — validating roughly $1.5 trillion
in payment value every cycle. What used to take over 150 hours of manual
effort per cycle now runs in the background.

**Avocado** — A team knowledge and analysis copilot, and the largest
thing I've built. Most "chat with your documents" tools retrieve a
paragraph and paraphrase it. Avocado does that — every answer carries
the sources it came from — but when the question is analytical it
writes pandas, runs it in a locked-down container, and returns the
computed number next to the program that produced it. One path is
explainable, the other is verifiable, and the interface tells you which
one you got. The sandbox is the part I'd defend in review: no network,
read-only filesystem, all Linux capabilities dropped, non-root, hard
memory and CPU caps, applied unconditionally rather than per request.
The API never holds the Docker socket — a separate runner does, with no
database and no model access — so compromising the API doesn't mean
owning the host. Tenant isolation is a SQL predicate at the repository
layer, not a filter in application code, because filtering after
loading means the rows already crossed the boundary. FastAPI +
PostgreSQL/pgvector + React, 757 tests, MIT.

**credit-rag** — Reads a 200+ page commercial credit agreement and
returns the key terms as structured data. The hard part isn't getting
an answer out of a language model; it's knowing whether to trust it.
Every value comes back with the page and the sentence it came from, and
each citation is verified in code against the retrieved text, so an
unsupported answer is downgraded to "not found" rather than invented.
Two-stage search — pgvector/HNSW narrowed by a local cross-encoder
re-ranker — with Kafka-queued ingestion and an idempotent worker.
Accuracy is measured rather than assumed: an evaluation harness scored
it against hand-labeled answer keys, lifting accuracy on a real SEC
filing from 57% to 71%, and disproved a change that turned out to make
no difference at all.

**Automated Portfolio Analytics Pipeline** — I wanted to learn how
data actually moves at scale. So I built one from
scratch as an assistant. This pipeline pulls daily stock prices from Yahoo Finance,
lands them in a PostgreSQL data warehouse, runs them through three
transformation layers using dbt (raw → cleaned → business-ready),
schedules everything with Apache Airflow, and surfaces the results in
a live Metabase dashboard — all running locally in Docker. The
architecture follows the medallion pattern (Bronze / Silver / Gold)
and a star schema in the gold layer. It's a portfolio project,
but it's built the way a real data team would build it.

**ThriveKid** — ThriveKid is a
full-stack PWA that helps parents like me track and support their child's
development. It took 8 months, two full mentor code reviews with a
senior engineer, and a 13-issue security audit before it went live.
Under the hood: React 19 TypeScript frontend on Vercel, a 3-layer
.NET 8 Clean Architecture backend on Azure, JWT authentication with
refresh token rotation, and Docker + GitHub Actions CI/CD.

---

### Tech I work with

**Languages** — `Python` · `TypeScript` · `C#` · `SQL` · `JavaScript`

**Backend** — `FastAPI` · `Pydantic` · `SQLAlchemy` · `Alembic` · `Flask` · `ASP.NET Core` · `Entity Framework Core` · `REST` · `WebSockets`

**Frontend** — `React` · `Angular` · `Tailwind CSS` · `Vite`

**Data** — `PostgreSQL` · `pgvector` · `Redis` · `Apache Kafka` · `dbt` · `Apache Airflow` · `Pandas` · `SQL Server` · `SQLite` · `Metabase`

**AI & retrieval** — `Claude API` · `RAG` · `Vector search` · `Cross-encoder re-ranking` · `Sandboxed code execution` · `Deepgram` · `Prompt Engineering`

**Infrastructure** — `Docker` · `Kubernetes` · `Terraform` · `AWS` · `Azure` · `Vercel` · `Nginx` · `GitHub Actions`

**Testing & tooling** — `pytest` · `Vitest` · `Playwright` · `Ruff` · `uv` · `OpenTelemetry` · `Git` · `GitHub Copilot`

---

### Background

I came from finance — Wells Fargo, then Raymond James, as an IT
Business Analyst doing SQL-heavy pipeline work — before teaching
myself to code and building the tools I needed when none existed.
Currently a candidate for the M.S. in Artificial Intelligence in
Business & Enterprise Integration at the University of South Florida
(expected December 2027) while working full-time at Citi.

---

🌐 [sangthai.dev](https://sangthai.dev) · 💼 [LinkedIn](https://linkedin.com/in/sang-thai) · 📧 thaisangcr7@gmail.com
