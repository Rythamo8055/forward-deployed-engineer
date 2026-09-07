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

> **GitHub audit 2026-09-07 via `gh` (80 repos scanned): 5x DONE, 2x DOING, 3x TODO. Evidence links below. Source of truth = this table. Pages dashboard mirrors it.**

| # | Required Skill (from blog) | What to Learn | Real-World Project — Plan vs YOUR Evidence | Certificate to Get (free-first for students) | Status |
|---|----------------------------|---------------|--------------------------------------------|--------------------|--------|
| 1 | Full-Stack Software Engineering Fundamentals | Python, TypeScript, APIs, Git, testing, system design | Plan: ticket-triage app + Docker + CI/CD<br>**✅ DONE: [aegis-support-copilot](https://github.com/Rythamo8055/aegis-support-copilot) (LangGraph+Streamlit+SQLite, 12 commits) + [docuqa-rag](https://github.com/Rythamo8055/docuqa-rag) (FastAPI+Next.js, 33 commits, live demo) + [cognodb-graphlink](https://github.com/Rythamo8055/cognodb-graphlink) (FastAPI+Cypher) + snip-url-shortener/shipgraph/cafe** | FREE: freeCodeCamp Full-Stack, Full Stack Open (free cert) / Paid later: Meta/IBM Coursera ($59/mo) OR AWS Developer Assoc $150 | 🟩 Done |
| 2 | Applied AI/LLM: Fine-tuning | HuggingFace, LoRA/QLoRA, OpenAI fine-tune API | Plan: Fine-tune Llama/Mistral on domain docs + eval report<br>**⚠️ GAP: [needle](https://github.com/Rythamo8055/needle) uses pretrained 45M tiny model (no training run). Need 1x Colab LoRA + eval report** | FREE: HuggingFace LLM Course + Agents Course (free cert) / DeepLearning.AI shorts free | ⬜ Todo |
| 3 | RAG Systems | Embeddings, vector DB (pgvector/Pinecone/Chroma), chunking, LangChain/LlamaIndex | Plan: RAG over PDFs/CSVs + citations + evals<br>**✅ DONE: [docuqa-rag](https://github.com/Rythamo8055/docuqa-rag) (parent-child 800/300, MiniLM, Chroma, Hybrid BM25+vector RRF + rerank, 54 tests, 27/28 stress 96%) + [aegis](https://github.com/Rythamo8055/aegis-support-copilot) (Chroma 12-doc + citation filter) + [breachkit](https://github.com/Rythamo8055/breachkit-redteam-lab) (48-doc corpus) + GraphRAG in cognodb** | FREE: DeepLearning.AI LangChain/RAG shorts free / Paid later: AWS ML Engineer Assoc $150 | 🟩 Done |
| 4 | Evals + LLM Deployment | Prompt evals, RAGAS, guardrails, latency/cost tradeoffs, Realtime API | Plan: eval harness + FastAPI deploy<br>**✅ DONE: [aegis](https://github.com/Rythamo8055/aegis-support-copilot) (60 golden tickets: triage 86.7%, escalation 81.7%, 0 grounding viol, CI blocks >2pts, 36 tests) + [breachkit](https://github.com/Rythamo8055/breachkit-redteam-lab) (14 probes 100%→0% stub, 23%→0% live gpt-oss-20b, CI gate) + [docuqa](https://github.com/Rythamo8055/docuqa-rag) (10/10 eval) + [genar-ai-safety-reporting](https://github.com/Rythamo8055/genar-ai-safety-reporting) (LLM-as-Judge + verifier)** | FREE: DeepEval practice + MS Learn AI-102 path free / Paid later: Azure AI-102 $165 (or free voucher via Skills Fest) | 🟩 Done |
| 5 | Data Engineering (Data is the moat) | SQL, ETL, dbt, Spark, data cleaning for siloed enterprise data | Plan: 3 sources → warehouse + quality docs<br>**🟨 DOING: [genar-ai-safety-reporting](https://github.com/Rythamo8055/genar-ai-safety-reporting) (Pandas 1068→1024 dedup + evidence packets) + [cognodb-graphlink](https://github.com/Rythamo8055/cognodb-graphlink) (3-domain graph modeling). Missing: SQL+dbt/Spark warehouse** | FREE: Databricks Academy Fundamentals badges free + Kaggle SQL free / Paid later: Databricks Assoc $200 | 🟨 Doing |
| 6 | Cloud Infra + Security (regulated: finance/health/gov) | AWS/Azure, IAM, VPC, secrets, HIPAA/SOC2 basics | Plan: AWS IAM/VPC/Secrets/logging + threat model<br>**🟨 DOING: [breachkit](https://github.com/Rythamo8055/breachkit-redteam-lab) (OWASP LLM Top10, guardrails, live Streamlit+Cloudflare demo) + [lolak-solutions-security-audit](https://github.com/Rythamo8055/lolak-solutions-security-audit). Missing: AWS IAM/VPC prod deploy** | FREE: AWS Skill Builder free + Student Rewards (21 badges = free $100 voucher) + Azure for Students $100 credit / Paid later: AWS SAA $150, Security $300 | 🟨 Doing |
| 7 | Rapid Prototyping (PoC in days) | v0/Lovable/Replit + Cursor, Streamlit/Gradio, Idea Shop mindset | Plan: 48h PoC + demo video<br>**✅ DONE: [needle](https://github.com/Rythamo8055/needle) (Tauri Rust 17 tools, 25 commits) + [GEMINI-3-HACKATHON](https://github.com/Rythamo8055/GEMINI-3-HACKATHON) (interview platform, 7 commits) + live Streamlit demos** | N/A — demo video + GitHub = proof | 🟩 Done |
| 8 | Communication + Writing | Tech specs, PRDs, architecture decision records (ADRs) | Plan: 1-pager + ADR per project in `/docs`<br>**✅ DONE: aegis `PLAN.md`+`DEVLOG.md`, breachkit `RED_TEAM_REPORT.md`+JSON scorecards, genar PADER/PSUR regulatory reports** | FREE: Google Technical Writing free | 🟩 Done |
| 9 | Listening / Empathy / User-Centric Loops | User interviews, DORA user-centric focus, tight feedback loops | Plan: 2-3 interviews, 2 iterations + log<br>**⚠️ GAP: no interview/feedback logs yet. Add `docs/feedback-log.md` to aegis** | FREE: IDEO acumen free articles / feedback log artifact | ⬜ Todo |
| 10 | Systems Thinking + Ambiguity + Business Sense (ROI) | Adoption, retention, ROI modeling, scoping vague needs | Plan: own KPI (↓support 30%) + ROI doc<br>**⚠️ GAP: no KPI/ROI doc yet. Add `docs/ROI.md` to aegis (baseline→shipped→measured)** | FREE: AWS Cloud Practitioner Learn path free / Paid later: PSM I $200 opt | ⬜ Todo |

### Minimal Certificate Shortlist (free-first — you are broke final-year, $0 now)
1. **$0 now:** HuggingFace Agents (free cert) + DeepLearning.AI shorts free + AWS Skill Builder free + MS Learn AI-102 path free + Databricks Fundamentals badges free + freeCodeCamp
2. **Free voucher hunt:** AWS Builder Student Rewards (21 badges = free $100 Foundational voucher) + Microsoft Skills Fest / Ignite challenge (100% off AI-102) + GitHub Student Pack (Azure $100, MongoDB free cert)
3. **Pay later only:** **AWS SAA $150** + **Azure AI-102 $165** + **Databricks Assoc $200** = ~$515 total. Portfolio > certs.
4. Plus portfolio > certs: recruiters in 2026 say **"doing the job before you get the job"** — you already have 5 DONE projects, that beats 10 certs.

## 4. Dev Log — What We Are Doing & What Happened in Sessions

> Update this after every study/build session. Newest on top.

| Date | Session # | What We Planned | What We Did | Key Learnings / Links | Next Up |
|------|-----------|-----------------|-------------|-----------------------|---------|
| 2026-09-07 | S03 | Audit GitHub via gh, mark DONE | Scanned 80 repos, mapped aegis/breachkit/docuqa/needle/cognodb/genar to 10 skills: 5 Done, 2 Doing, 3 Todo. Updated README + Pages with evidence links | Strongest: eval-gated CI (60 golden, 14 probes, Ragas 0.982). Gaps: LoRA fine-tune, AWS IAM/VPC, ROI/feedback logs | 1x free LoRA Colab + add docs/ROI.md + docs/feedback-log.md to aegis, claim 2 free badges |
| 2026-09-07 | S02 | Push to GitHub + Pages tracker | Created public repo, pushed 5 files, enabled Pages (legacy/main-root), set homepage, verified 200 live | Pages build `built` in ~1min; live dashboard persists ticks via localStorage | Pick Project #1 stack, scaffold `/projects/01-fullstack-starter` |
| 2026-09-07 | S01 | Repo setup + analyze IIT FDE blog | Created this README, added weblink, extracted skills/projects/certs table, initialized dev log | FDE = 1 customer x many capabilities; AI easy to demo hard to deploy; 95% pilots fail | Pick Project #1 stack, create `/projects/01-fullstack-starter` + `/docs` |
| YYYY-MM-DD | S04 | _template - copy this row_ | | | |

### How to use this log
- `What We Planned` = goal before session
- `What We Did` = actual work + files changed
- `Key Learnings` = 2-3 bullets + any new links
- Always update Master Table `Status` column when a skill/project moves: `⬜ Todo → 🟨 Doing → 🟩 Done`

## 5. Roadmap (suggested order)

- [x] Phase 0: Setup — README + `/projects` + `/docs` + `/certs` folders + Pages live
- [x] Phase 1a: Full-stack + RAG + Evals (Skills 1,3,4,7,8) — DONE via aegis/breachkit/docuqa/genar
- [ ] Phase 1b: Cloud prod deploy — AWS IAM/VPC/Secrets for docuqa (Skill 6 gap)
- [ ] Phase 2: Data warehouse ETL (Skill 5 gap) + LoRA fine-tune + eval report (Skill 2 gap)
- [ ] Phase 3: Customer sims — add `docs/feedback-log.md` + `docs/ROI.md` to aegis (Skills 9,10 gaps)
- [ ] Phase 4: Free badges (2x) + voucher hunt + resume with metrics (triage 86.7%, probes 100%→0%, Ragas 0.982)

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
