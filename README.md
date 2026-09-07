# Forward Deployed Engineer (FDE) — Prep & Build Log

> Repo name on disk: `forward development engineer` → Correct industry title is **Forward Deployed Engineer (FDE)**.

[![GitHub](https://img.shields.io/badge/GitHub-Rythamo8055%2Fforward--deployed--engineer-blue?logo=github)](https://github.com/Rythamo8055/forward-deployed-engineer)
[![Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Tracker-green?logo=github)](https://rythamo8055.github.io/forward-deployed-engineer/)
[![Source](https://img.shields.io/badge/Source-IIT%20FDE%20Guide-orange)](https://www.iit.edu/blog/forward-deployed-engineer)

- **Repo:** https://github.com/Rythamo8055/forward-deployed-engineer
- **Live tracker (GitHub Pages):** https://rythamo8055.github.io/forward-deployed-engineer/

## 1. Source Weblink

**Main reference for this repo:**

- https://www.iit.edu/blog/forward-deployed-engineer
- Title: *What Is a Forward Deployed Engineer? Inside Tech's Hottest New Job—and How to Prepare for It* — By Petra Kelly, Illinois Tech

Additional sources linked inside that blog:
- AWS $1B FDE org: https://www.aboutamazon.com/news/aws/aws-1-billion-forward-deployed-ai-engineers
- Microsoft Frontier Company ($2.5B / ~6,000 experts): https://blogs.microsoft.com/blog/2026/07/02/microsoft-frontier-company-ai-engineering-that-amplifies-and-protects-your-intelligence/
- a16z: Trading Margin for Moat: https://a16z.com/services-led-growth/
- Pragmatic Engineer: What are Forward Deployed Engineers: https://newsletter.pragmaticengineer.com/p/forward-deployed-engineers
- The New Stack - Why FDE is tech's hottest job: https://thenewstack.io/why-the-forward-deployed-engineer-is-techs-hottest-job/
- The New Stack - Tech Hiring 2026: https://thenewstack.io/tech-hiring-in-2026-the-rise-of-the-specialist/

## 2. Blog Analysis (TL;DR)

**What is an FDE?**
Term coined by Palantir (originally called "Deltas"). Military analogy: deployed forward, close to action. In tech: embedded directly with customers to design, build, ship custom software — usually AI — inside customer's real systems, and feed learnings back to core product.
> Regular dev = one capability across many customers. FDE = one customer across many capabilities.

Part Software Engineer + Solutions Architect + Consultant + Startup CTO / Field CTO.

**What does an FDE actually do? (3-part loop)**
1. **Embed with customers:** On-site / alongside team, map domain/processes. Palantir ~25% time with customers, Commure up to 50%.
2. **Build the solution:** Production code in customer's infra, not demo. For AI: fine-tuning, RAG systems, Evals, LLM deployment, data wiring.
3. **Improve core product:** Customer-specific fix becomes platform feature for all. Ex: OpenAI + John Deere work improved Realtime API for everyone.

Examples from blog:
- OpenAI FDE → John Deere (Iowa farm visit, shipped before growing-season deadline)
- Ramp FDE "pods" tied to specific customers
- Matta (industrial-AI) scopes on factory floor
- AWS FDEs → Allen Institute, Cox Automotive, NBA, NFL (NFL Fantasy AI, NFL IQ in weeks), Ricoh, Southwest Airlines

**Why hottest job in 2026?**
> AI is easy to demo, hard to deploy.

- 95% enterprise AI pilots fail (MIT 2025) — siloed data, security, legacy systems.
- a16z analogy: enterprises buying AI are "like your grandma getting an iPhone" — need setup.
- >50% US tech postings now require AI/ML (up from ~29% year before), 84% orgs to increase AI spend.
- Andela CEO: "FDEs, not FTEs". McKinsey: candidate pool for data roles may cover only ~50% demand.

**Salary context:**
Blog cites BLS 2023: Computer/Info Research Scientists ~$145k median, Data Scientists ~$108k median + 36% decade growth. FDE frequently at/above senior SWE levels + variable pay tied to customer outcomes.

**FDE vs similar roles:**
- **Solutions Engineer / Architect:** More advisory, PoC with sample data, rarely production code on customer systems.
- **AI Engineer:** Builds/integrates AI/ML, not necessarily embedded with specific customer.
- **FDE:** Most hands-on — embedded, writes production code in customer env, contributes back to core product.
- Adjacent titles: Agent Engineer, Implementation Engineer, Technical Delivery Engineer, Sales Engineer.

**Key quote:** Scope resembles startup CTO — small teams, high stakes, end-to-end ownership.

## 3. Master Table: Required Skills → Real-World Projects → Certificates

This is our job-readiness tracker. Check off as we build.

| # | Required Skill (from blog) | What to Learn | Real-World Project to Build (for portfolio) | Certificate to Get | Status |
|---|----------------------------|---------------|--------------------------------------------|--------------------|--------|
| 1 | Full-Stack Software Engineering Fundamentals | Python, TypeScript, APIs, Git, testing, system design | Customer Co-Build Starter: Full-stack internal tool (e.g., support ticket triage app) deployed in Docker + CI/CD | Meta Full-Stack / IBM Full Stack (Coursera) OR AWS Certified Developer - Associate | ⬜ Todo |
| 2 | Applied AI/LLM: Fine-tuning | HuggingFace, LoRA/QLoRA, OpenAI fine-tune API | Fine-tune a small model (e.g., Llama 3 / Mistral) on customer-like domain data (e.g., farm manuals à la John Deere example) + eval report | HuggingFace Course Cert / OpenAI + DeepLearning.AI Fine-tuning | ⬜ Todo |
| 3 | RAG Systems | Embeddings, vector DB (pgvector/Pinecone/Chroma), chunking, LangChain/LlamaIndex | RAG over messy PDFs/CSVs (e.g., NFL rulebook + tickets, or factory SOPs) with citations + evals | DeepLearning.AI LangChain / Vector DBs (Short Courses) + AWS Certified ML - Specialty | ⬜ Todo |
| 4 | Evals + LLM Deployment | Prompt evals, RAGAS, guardrails, latency/cost tradeoffs, Realtime API | Add eval harness to Project #3: accuracy, hallucination rate, latency dashboard. Deploy via FastAPI + vLLM/Bedrock | OpenAI Evals / Confident AI DeepEval practice + Azure AI Engineer Associate (AI-102) | ⬜ Todo |
| 5 | Data Engineering (Data is the moat) | SQL, ETL, dbt, Spark, data cleaning for siloed enterprise data | Siloed-Data Unifier: Ingest 3 messy sources (SQL + CSV + API) → clean warehouse + docs. Show before/after data quality | Databricks Certified Data Engineer Associate / Google Professional Data Engineer | ⬜ Todo |
| 6 | Cloud Infra + Security (regulated: finance/health/gov) | AWS/Azure, IAM, VPC, secrets, HIPAA/SOC2 basics | Deploy Project #3 on AWS with IAM, VPC, Secrets Manager, logging. Threat-model doc for healthcare/finance variant | AWS Solutions Architect Associate + AWS Security Specialty OR Microsoft AZ-104 + SC-100 basics | ⬜ Todo |
| 7 | Rapid Prototyping (PoC in days) | v0/Lovable/Replit + Cursor, Streamlit/Gradio, Idea Shop mindset | 48-hour Prototype Sprint: Ship working PoC in front of a "customer" (friend/mock) + demo video + feedback loop | N/A — proof is demo video + GitHub (IPRO-style Innovation Day) | ⬜ Todo |
| 8 | Communication + Writing | Tech specs, PRDs, architecture decision records (ADRs) | Write 1-pager + ADR + demo script for every project above. Publish in `/docs` | N/A — portfolio docs (or Google Technical Writing course) | ⬜ Todo |
| 9 | Listening / Empathy / User-Centric Loops | User interviews, DORA user-centric focus, tight feedback loops | Factory-Floor Simulation (Matta-style): Interview 2-3 real users, map process, iterate 2 versions based on feedback log | N/A — feedback log artifact / IDEO Design Thinking cert (optional) | ⬜ Todo |
| 10 | Systems Thinking + Ambiguity + Business Sense (ROI) | Adoption, retention, ROI modeling, scoping vague needs | Ramp-Pod Simulation: Pick one customer, own KPI (e.g., reduce support time 30%). Track baseline → shipped → measured ROI doc | AWS Cloud Practitioner (business fluency) + Product / Scrum (PSM I or Pragmatic) optional | ⬜ Todo |

### Minimal Certificate Shortlist (if you want jobs fast)
1. **AWS Certified Solutions Architect – Associate** (cloud + deployment credibility)
2. **AWS Certified Machine Learning – Specialty** OR **Azure AI Engineer Associate (AI-102)** (applied AI/RAG/evals)
3. **Databricks Data Engineer Associate** OR **Google Professional Data Engineer** (data = edge)
4. Plus portfolio > certs: recruiters in 2026 say **"doing the job before you get the job"** — 3-4 production-ready projects beat 10 certs.

## 4. Dev Log — What We Are Doing & What Happened in Sessions

> Update this after every study/build session. Newest on top.

| Date | Session # | What We Planned | What We Did | Key Learnings / Links | Next Up |
|------|-----------|-----------------|-------------|-----------------------|---------|
| 2026-09-07 | S01 | Repo setup + analyze IIT FDE blog | Created this README, added weblink, extracted skills/projects/certs table, initialized dev log | FDE = 1 customer x many capabilities; AI easy to demo hard to deploy; 95% pilots fail | Pick Project #1 stack, create `/projects/01-fullstack-starter` + `/docs` |
| YYYY-MM-DD | S02 | _template - copy this row_ | | | |

### How to use this log
- `What We Planned` = goal before session
- `What We Did` = actual work + files changed
- `Key Learnings` = 2-3 bullets + any new links
- Always update Master Table `Status` column when a skill/project moves: `⬜ Todo → 🟨 Doing → 🟩 Done`

## 5. Roadmap (suggested order)

- [ ] Phase 0: Setup — README + `/projects` + `/docs` + `/certs` folders
- [ ] Phase 1: Full-stack + Cloud deploy (Skills 1,6,8)
- [ ] Phase 2: Data pipeline (Skill 5)
- [ ] Phase 3: RAG + Evals + Fine-tune (Skills 2,3,4)
- [ ] Phase 4: 2x Customer simulations with ROI docs (Skills 7,9,10)
- [ ] Phase 5: Cert exam (pick 1 cloud + 1 AI) + resume with metrics

## 6. Folder Plan

```text
forward development engineer/
  README.md          <- you are here
  docs/              <- specs, ADRs, interview notes, ROI docs
  projects/
    01-fullstack-starter/
    02-data-unifier/
    03-rag-with-evals/
    04-finetune-domain/
    05-rapid-prototype-sprint/
  certs/             <- cert notes + exam checklists
  sessions/          <- optional per-session notes (S01.md, S02.md...)
```

---
*Maintained as living doc. Source of truth: IIT blog link in Section 1.*
