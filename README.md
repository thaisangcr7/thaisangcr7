## Hi 👋, I'm Sang.

**Automation Engineer · Data Engineering · Financial Systems** at Citibank · Tampa, FL

I build production automation infrastructure at the intersection of
financial operations and Data engineering practices. I turn manual,
error-prone workflows into reliable, scalable systems.

---

### What I'm building

**ATLAS** — It started with a simple initiative: a team manually
reconciling payment records every month across spreadsheets, burning
days of work just to catch errors that a machine could find in
seconds. So I built one. ATLAS is a config-driven Python automation
platform I designed and built entirely solo at Citi. It processes
~25M records/month across 52 global payment applications — running 5 different
pipeline including Threshold, Duplicate, Dual Blind Rekey, and GP
GPOC and MCA executive reporting — validating roughly $1.5 trillion in
payment value every cycle. What used to take over 150 hours of manual
effort per cycle now runs in the background.

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

**ThriveKid** ThriveKid is a
full-stack PWA that helps parents like me track and support their child's
development. It took 8 months, two full mentor code reviews with a
senior engineer, and a 13-issue security audit before it went live.
Under the hood: React 19 TypeScript frontend on Vercel, a 3-layer
.NET 8 Clean Architecture backend on Azure, JWT authentication with
refresh token rotation, and Docker + GitHub Actions CI/CD.

---

### Tech I work with

`Python` · `Pandas` · `FastAPI` · `Flask` · `dbt` · `Apache Airflow` · `C#` · `ASP.NET Core` · `Entity Framework Core` · `React` · `TypeScript` · `RESTful APIs` · `PostgreSQL` · `SQLite` · `SQL Server` · `Docker` · `Azure` · `GitHub Actions` · `Git` · `GitHub Copilot` · `Prompt Engineering`

---

### Background

I came from finance — Wells Fargo, then Raymond James, as an IT
Business Analyst doing SQL-heavy pipeline work — before teaching
I had to code and build the tools I needed when none existed.
Currently a candidate for the M.S. in AI & Business Analytics
(Systems Integration) at USF's Muma College of Business while
working full-time at Citi.

---

🌐 [sangthai.dev](https://sangthai.dev) · 💼 [LinkedIn](https://linkedin.com/in/sang-thai) · 📧 thaisangcr7@gmail.com
