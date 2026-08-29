<h1 align="center">Hey, I'm Ootso 👋</h1>
<h3 align="center">Backend + AI infrastructure · CSE @ B.P. Poddar Institute, Kolkata</h3>

<p align="center">
  <a href="mailto:ootsodhar@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://leetcode.com/u/Ootsoooooooooo/"><img src="https://img.shields.io/badge/LeetCode-ffa116?style=for-the-badge&logo=leetcode&logoColor=black" /></a>
  <a href="https://github.com/Ben160804"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

### Where I'm headed

I'm a backend engineer crossing over into AI infrastructure. I've spent the last year building automation pipelines — moving data between APIs, orchestrating workflows, shipping features that serve real users. Now I'm going deeper: understanding the math behind ML, building systems that wrap and serve models, and learning how production AI actually works.

I don't just want to *use* AI tools. I want to understand them, build with them, and eventually design the infrastructure that makes them reliable.

---

### What I've done

**[Bluebeaks Solutions](https://bluebeaks.com) — AI Engineer Intern** *(May 2026 - Aug 2026)*

Built the AI layer of a resume tailoring platform. My work sat at the intersection of backend engineering and ML operations:

- Designed an **n8n pipeline** that ingests job descriptions, scores resumes against them using **Gemini LLM prompts**, and outputs tailored PDFs — processing 200+ resumes/week at 95%+ formatting accuracy
- Built a **multi-persona drip email system** with five user segments and cron scheduling, cutting manual outreach by ~70%
- Scaled lead generation to **400+ companies across 5 countries**, enriching **10,000+ contacts** via Tomba and Cleanlist APIs — 3x prospecting efficiency
- Wrote a **Python transformation layer** handling 50+ API payloads/day at 99.9% data integrity, supporting multi-step workflow orchestration
- Integrated **Gemini with guardrail prompts** to generate structured outputs for 100+ job descriptions/month, reducing human review by 40%
- Built automated job-application workflows using **Zerowork**, saving ~6 hours/week of manual work

**Key realization from this role:** shipping AI features isn't about the model — it's about the pipeline around it. Data integrity, prompt guardrails, fallback logic, and observability matter more than the LLM itself.

---

### Projects

**[Journald-Sniffer](https://github.com/Ben160804/Journald-Sniffer)** *(2025 - Present)*

Linux auth event ingestion and threat detection pipeline. Reads systemd journal (facility 10 — `authpriv`), parses sudo/su/sshd sessions, classifies outcomes, escalates ambiguous ones to Groq LLM, and alerts on suspicious patterns. Exposed via FastAPI and containerized with Docker.

- **Pipeline:** `ingestor.py` → `parser.py` → `llm.py` → `watchdogv2.py`
- **API:** FastAPI with 6 endpoints — `/health`, `/ingest`, `/parse`, `/alerts`, `/sessions`, `/raw`
- **Classification:** success / failure / suspicious / unknown via keyword matching + Groq LLM fallback for ambiguous sessions
- **Threat detection:** brute-force (5+ failures from same IP), port scan (12+ neutral events, 0 successes), success-after-failure
- **Storage:** PostgreSQL with three tables — `raw_logs`, `auth_logs`, `ingest_state`
- **LLM:** Groq `llama-3.1-8b-instant` — only called for ambiguous sessions to minimize API costs
- **Deployment:** Dockerfile + docker-compose, uvicorn ASGI server

**[RepoRecon](https://github.com/Ben160804/RepoRecon)** *(2026)*

Automated repo structure analysis and code intelligence. Currently rebuilding it with:

- AST parsing for Python codebases
- Embedding-based code search (moving from keyword to semantic)
- This is my playground for learning how vector search actually works

**[skill_sYnc](https://github.com/Ben160804/skill_sYnc)** *(2026)*

Flutter app connecting users based on shared skills. Firebase backend, production-deployed. My reminder that shipping matters more than perfection.

**[MediScribe](https://github.com/Ben160804/MediScribe)** *(2026)*

Medical documentation assistant built with Dart + Flutter. Explored how LLMs can be constrained to produce reliable clinical text — mostly learned what *doesn't* work.

---

### Numbers

- **400+** LeetCode problems solved (max rating 1616)
- **200+** resumes/week automated at Bluebeaks
- **10,000+** contacts enriched across 5 countries
- **6** REST endpoints in Fac-10Sniffer, 98% detection accuracy
- **SIH 2025 Grand Finalist** — ISRO problem statement
- **GDG On Campus** Core Technical Team

---

### Tech Stack

```yaml
Languages:        Python, SQL
Backend / APIs:    FastAPI, Django REST Framework, REST APIs
Automation / AI:   n8n, Google Gemini API, Groq API, RenderCV
Databases:         PostgreSQL, MongoDB
Networking:        TCP/IP, DNS, DHCP, HTTP/HTTPS, SSH, IPv4/IPv6, Routing, Subnetting
Core CS:           Data Structures & Algorithms, Operating Systems, DBMS,
                   Computer Networks, OOP, Software Development
Tools:             Git, GitHub, Docker
```

---



### LeetCode

<p align="center">
  <img src="https://leetcard.jacoblin.cool/Ootsoooooooooo?theme=dark&font=Noto%20Sans&ext=heatmap" />
</p>

---

> **Currently seeking:** 2027 SWE internships in **AI infrastructure** or **backend engineering** at companies that take ML seriously.
> Open to relocating. Let's talk: ootsodhar@gmail.com
