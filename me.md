# Me

Source of truth for **search, analytics, advice, and a CV**. Not a goal. Not this week’s plan. No phone or email in this file.

- Goals: [`goal.md`](goal.md) / [`goals/`](goals/)
- This week: [`now.md`](now.md)
- Evidence of learning: [`work/`](work/README.md)
- A real CV (when it exists) belongs under `work/relocate/` — generate it **from this file**, do not invent extra jobs, titles, or metrics.
- Public HTML CV: [`index.html`](index.html) at the repo root (GitHub Pages).

Change this file when a **fact is wrong**. Append **Updated**.

---

## CV headline

**Backend Software Engineer** — Hanoi, Vietnam.  
Overseas aim: **mid / intermediate** backend SWE on a work visa (NZ first). Company title is Senior; do not use Senior as the overseas headline.

| | |
| --- | --- |
| **Name** | Long. People call me **Kang**. CV name: **Long**. |
| **Location** | Hanoi, Vietnam |
| **Would move** | Solo |
| **Work language at 9–5** | Vietnamese. **Not** English. **Not** Japanese. |

---

## Summary (CV-ready)

Backend engineer at **Kaopiz Software** (Japanese outsourcing, Hanoi). Intern from **Aug 2021**, full-time from **Aug 2022**, now **Senior Software Engineer** (company title). About **5 years** building software for Japan-based companies from **their requirements**.

Main stack: **Python, FastAPI, PostgreSQL, SQLAlchemy, Celery, Docker, REST**. Sometimes Vite frontend and LLM features **as software** (not ML research). Client domains are **mixed** (e-commerce, AI, internal tools, and others) — there is no single industry headline.

**Honest level:** I have sat in the **design seat** (architecture + data) on a small team (about 2–5). **Most** of that work I do not consider good design. **Exception:** the internal **SDLC document tool** — I designed it **from scratch** and it is good enough to talk about on a CV (I will defend “designed” for **this system only**). AI helped me code faster; the design decisions were still mine. It still has **too much technical debt**, and I have not handed it off. Overseas mid-level is still the headline; company-Senior is not a blanket architecture claim.

### How I work (Kaopiz pattern)

I am known as **highly adaptive**: give me a problem I have never seen, I still find a way to ship a solution. I **keep getting assigned to new projects**. Everything is new; I have to learn a lot.

**Cost:** I have **rarely stayed on a project more than about 7 months**. Breadth is real. Depth is hard. I also **keep seeking the next new thing**. That matches mixed client domains and “spec was the design” on most systems.

**Now:** the internal document tool is the one I still own — that is the depth bet (handoff, domain, design I would defend). Do not write “5 years on one product.” Do not write “job hopper” (one employer). Do not hide the rotation.

---

---

## Experience

### Kaopiz Software — Hanoi

Japanese outsourcing: software for Japan companies, from their specs/requirements.

| Period | Title |
| --- | --- |
| Aug 2021 – Aug 2022 | Intern |
| Aug 2022 – present | Full-time engineer, junior → **Senior Software Engineer** (title about **2025**; current HR title) |

**Scope (typical project):** I am the person who shapes architecture + data; others implement with me. Team is usually 2–5. I **review and explain** to the team. That is the *seat*. It is **not** “I left a system someone else can run.”

**How I judge that work (17 Sep 2026):** The same weaknesses showed up on **several** systems (e-commerce, LLM-as-software, other internals, legacy) — not one bad project. Those are **real**, but they **lack design**. **Exception:** the internal **SDLC document** tool (below) — designed from scratch, quite good, **allowed on a CV**. Do not extend that claim to the other systems. Do not polish the others into “designed and led production systems.”

**What “lack of design” meant in practice:**

- The **spec was the design** — tables and APIs copied from it
- Domain rules lived in my head or in if-statements, not as a clear model
- **Hard to change** — one change broke several places
- **No module boundaries** — everything talked to everything
- **Database was messy** — unclear keys, duplicated data, no obvious source of truth
- I could **not** really run / observe / roll it back myself
- I could **not teach someone else to keep it going** without me
- I shipped fast with **AI / copied patterns**, then did not go back and design

**First gap to close (ranked):** leave a system **someone else can run**. Evaluable test: **one system at work** — another engineer can **change and run it for a week without pinging me**. That is already inside DevOps “done” ([`goals/devops.md`](goals/devops.md)). Business domain ([`goals/business.md`](goals/business.md)) is the spec-vs-rules half. Do not add a fifth goal named “learn design.”

### One system (handoff target + CV story)

**Label (generic, no product name):** Kaopiz **internal SDLC document tool**. Software documents for the company’s own work (not a Japan-client e-commerce app). About **a few months** old.

**Who uses it:** mixed roles, **most of the people on a project** (not QA-only).

**The problem it was for:** documents **went outdated over time**; **hard to manage and update with QA**; **no shared place for the company**.

**Job of the tool:** one company place for software documents + review (QA here = review/update docs, not a test-case product).

**How it actually works (now):**

- **Git is storage** (GitLab / Bitbucket). Users **create and update docs locally**. The **web app is for view + discuss**.
- Users **comment and talk about the document** (live view on the web).
- **“QA” here = review the document** (comment, discuss, approve) — **not** a test-case / bug-tracker product. Do not write ISTQB / test management on a CV.

**Core record:** a **document** (in git / local). Comments and other features **live on the server**, around that document.

**How the design actually moved (interview story — do not skip the failed steps):**

1. **Everything in the database first.** Documents were **hard to manage** that way. People already **work locally**.
2. **Everything in Git next** — documents, **even comments**, and some other data. Then **ACID** for comments and similar features was **hard** (Git is not a good place for that).
3. **Split (what shipped):** **docs live locally** (Git). **Features live on the server** (comments and the rest).
4. **First design also included AI generate and AI edit.** That was **not good enough for production**, so we moved to this **local hybrid** — users can work on documents locally instead of depending on those AI flows.

Do not write the story as “we always knew Git + server.” The split came **after** DB-first and Git-everything. Do not list AI generate/edit as a shipped product feature.

**The design I will defend in an interview (one sentence):**  
Docs in Git/local, features on the server — we landed there after DB-everything and Git-everything both failed in different ways (docs hard to manage in the DB; ACID for comments hard in Git; AI generate/edit not production-ready).

**Stack (this system):** FastAPI, PostgreSQL, SQLAlchemy, REST; Docker / Celery as in my usual stack. **Frontend: Vue.js**, vibe-coded with AI (I still own the design). Do not headline “Vue expert.”

**Why this one first (handoff):** I **still own it**. If I disappeared, people would ping me. **Successor:** not chosen yet.

**What would fail on a handoff this week:** the pieces fit **only in my head**; **data model changes still need me**.

**Technical debt (honest):** we **pulled in a lot of features; most failed; lots of bugs**. **AI generate and AI edit** were in the **first design**, not later extras — they were **not good enough for production** (that is one reason for the local hybrid). Also failed: **AI review**, **graph view for document traceability**. Do not list those as shipped product features. Do not call this an AI product.

**If I write notes:** domain = a document in Git/local vs a comment on the server, why DB-everything and Git-everything each failed, what a comment is allowed to mean. DevOps = debt + one teachable change. English essay/interview: **this is the system** (tell the three storage steps, not only the end state).

**CV (this system only — allowed):** I **designed and built it from scratch**. I will defend **designed** here. AI helped me **implement faster** (including the Vue UI). The design to talk about is the **storage split** (DB → Git-everything → docs local / features on server), not “we always used Git.” High debt; AI generate/edit was first-design and failed; I still own schema changes. No product name, no fake metrics.

Allowed bullet shape:

- Designed and built from scratch an internal SDLC document tool. Tried DB storage first (docs hard to manage); then Git for everything including comments (ACID for comments was hard); now docs live locally in Git, comments and other features on the server. Python / FastAPI / PostgreSQL; Vue UI. Used AI to code faster. First design also had AI generate/edit — not production-ready, which is one reason for the local hybrid. High bug/debt load; I still own schema changes.

**Handoff today (company-wide, not only this tool):** important knowledge stays in my head (I explain once, they still need me); no runbook (start, healthy, break); often only my machine / my access; juniors can take tickets I split, they cannot change the model without me.

**Teaching today:** not a real 9–5 practice. A **seminar / course** is something I want later (Vietnamese audience, from the handbook — stash, not current teaching). Do not write “mentor” or “tech lead who grows the team” on a CV.

**What I do not own as a headline:** production infra / AWS (touched, not strong). Japanese client meetings. English at work. “Strong system design.” “I mentor so the system survives me.”

#### Work that existed (kinds)

**CV design highlight — this one only:**

- Internal **SDLC document** tool — docs local/Git, features on the server (after DB then Git-everything); designed **from scratch** (generic label)

**Other work — true, weak design, no “I designed X well”:**

- E-commerce / shop / order-style systems (API + data)
- LLM features as product software (not research)
- Other internal tools
- Legacy systems I took over

#### Named systems (CV bullets)

**Allowed:** the SDLC document tool (bullet shape above). Do not invent user counts. Do not list failed AI/graph extras as successes.

**Still blocked as design highlights:** e-commerce, LLM features, other internals, legacy. Mid-level delivery lines only if a CV needs more than one job bullet.

---

## Skills

**Use on a CV (have used at work):**

| Area | |
| --- | --- |
| Languages | Python |
| Backend | FastAPI, REST APIs, Celery |
| Data | PostgreSQL, SQLAlchemy (schema work — **not** a design strength yet) |
| Ship-ish | Docker |
| Sometimes | Vue.js on the SDLC tool (AI vibe-coded — not a Vue headline); Vite on other work; LLM APIs as application features |

**Do not headline / do not fake on a CV:**

- AWS, Kubernetes, SRE, DevOps job title
- Japanese language
- ML Engineer / AI specialist / research
- English as a work language at Kaopiz
- A single industry expert (domains are mixed; spec often *is* the domain — that gap is [`goals/business.md`](goals/business.md))
- “System designer” / “architect” as a **general** headline — only the SDLC document tool may use **designed** (from scratch: storage path DB → Git-everything → docs local / features on server). Other Kaopiz work still lacks design.
- This tool as a **test-case QA product** or as an **AI document product** (AI generate/edit was first-design and failed; graph extras also failed)
- That Git was the **first** storage idea (path: DB → Git-everything including comments → split)

---

## Education

**Bachelor of Computer Science** — Thang Long University, Hanoi.

| | |
| --- | --- |
| **Cohort** | About **2018–2022** (normal years) |
| **What happened** | I skipped / barely attended from about **2022** to focus on work at Kaopiz |
| **Degree** | Finished in **2026** |

A CV may say B.Sc. CS, Thang Long University, **2026**. Do not imply I was a full-time student 2022–2026. Do not hide the degree.

---

## Languages

| | |
| --- | --- |
| Vietnamese | Native. Work language. |
| English | About **TOEIC 750**. Can **read** and **talk daily**. **Not** used at Kaopiz. |
| Japanese | Almost none. Do not list as a skill. |

**Interviews (tested, 1–2 real ones):** I go **blank**. I cannot answer the way I would at work. I **start talking**, but it comes out **bad and wrong**. After I go home I see that I **could have done better** — the knowledge was there; the interview was not. This is a **performance / how I talk about what I do** stall, not “I do not know English at all.” Path still: essay first, then speak from it ([`goals/english.md`](goals/english.md)). Do not prescribe a mock-interview treadmill unless Kang asks.

---

## Relocate (targeting — not a public CV section)

**Aim:** live and work where the job is in English. **NZ** is the country I picked first (life in English, not a researched visa plan). **Australia** is also OK. For a first offer: **whichever mid-level backend visa job comes first (NZ or AU)**. Other countries are not the current backup list.

**Role:** mid-level **backend** SWE on a **work visa**. Company-Senior / ML / AI specialist are not the headline.

**How I get there:** **remote first is OK if it can lead to a visa later.** Still not the plan: remote-forever contractor / EOR with no visa path ([`goals/relocate.md`](goals/relocate.md)).

**Visa knowledge:** **thin**. I have not really studied AEWV / accredited employers. NZ-first is an aim, not a researched plan. Do not fake visa expertise. Do not block a CV rewrite on studying the whole immigration manual.

**English tests:** TOEIC ~750 only. **IELTS/PTE later**, when a visa or employer asks — not now.

**Search today:** I have an **English CV / LinkedIn**, but the CV is **old and overclaims** (senior / AI / design). I am **not applying**. I would rather **rewrite from this file** than reuse the old CV. LinkedIn must not stay as a senior/AI headline if we touch it.

**Blocker:** I am **not confident to start** (apply). That is the stall — not missing IELTS, not missing a new portfolio project.

**What to produce anyway (relocate files, not applications):** an honest CV under `work/relocate/` generated from this file. Interview reps stay in `work/english/`. Do not mass-apply. Do not wait for confidence before **writing** the CV; do wait for Kang before sending applications he did not ask to send.

**“Next few months”** still means a real search window, not a 6-month fail cliff. A week with zero study sessions can still hold a relocate todo only if it is small (e.g. CV draft from `me.md`).

---

## Time that is real (not a CV section)

About **45 minutes**, **late** (after dinner), often already tired. Some weeks **0** sessions, some weeks **2–3**. Do **not** plan as if this is steady.

What usually kills it: **tired from 9–5** (open the file and stop), and **phone / chat / YouTube** instead of the timer.

For `now.md`: one must-land file that still works if the week is a zero. No four equal book-chunks. Do not add todos that need “most weekdays.”

---

## Side (not a named goal; optional CV “projects” only if we write a real bullet later)

**NomStamp** — iOS app: stamp food photos on a map. Dropped as a learning goal (2026-W36). Hobby. Do not treat as current `now.md` work.

---

## Current named goals (index only)

1. Learn DevOps
2. Learn English
3. Learn business domain
4. Move (NZ or other)

---

## For agents

**Be accurate and coach.** This file is also a **CV source**: a generated CV may only use facts here. If a bullet needs a named system or a number that is not here, ask — do not invent.

Do **not** assume or invent:

- Senior / staff **overseas**, ML Engineer, “AI specialist”
- Japanese as a work language
- English used at Kaopiz
- Frontend, LLM, or AWS as the center of the job
- One client industry as my identity, or 5 years on one product
- That I job-hop companies (one employer; projects often under ~7 months)
- That I already work deeply by default (I seek new; depth is the current bet)
- Daily weekday study sessions, or a steady “few evenings” (some weeks are zero)
- A partner/family move
- Founder / MBA / canvas / LTV-CAC as the business-domain goal
- NomStamp as a current goal
- That a 9–5 day counted as learning with no `work/` file
- Metrics, awards, or project names not written above
- That **all** Kaopiz systems are strong design work (only the SDLC tool is CV-designable)
- That the SDLC tool is a test-case QA product, an AI-doc product, or already handed off / low-debt
- That Git + web discuss was the first design (it was DB, then Git-everything, then the split)
- That “used AI to code faster” means ML Engineer
- That I can already hand a system off (first gap: someone else can run it)
- That I currently teach / mentor as a real part of the job (seminar is a wish; handoff fails)
- A named successor on the SDLC tool (person is **not chosen yet**)
- That visa/AEWV is already researched
- That I am ready to apply (I am not confident to start)
- That the old English CV is usable (it overclaims; rewrite from this file)
- Remote-forever / EOR as the whole plan (remote-first is OK only with a visa path)

When suggesting DevOps or business-domain work, default to the **internal SDLC document tool** (docs in Git/local, features on the server). Do not switch to e-commerce/LLM for “a better story.” Do not tell the design as if Git was the first idea.

### How to draft a CV from this

1. **Rewrite from this file.** Do not reuse the old English CV (it overclaims senior / AI / design).
2. Headline: Backend Software Engineer (mid), Hanoi. Target: NZ or AU work-visa role.
3. One employer: Kaopiz Software, intern Aug 2021 / full-time Aug 2022–present, company title Senior from ~2025.
4. Summary + skills. No ML headline. **Designed** only for the SDLC document tool (storage path: DB → Git-everything → docs local / features on server).
5. Experience: that SDLC bullet. Do not sell failed AI/graph features. Other systems = delivery only.
6. Education: B.Sc. CS, Thang Long University, **2026** (cohort ~2018; work-first from ~2022).
7. Languages: Vietnamese; English TOEIC ~750 (do not imply interviews are fine). No Japanese.
8. English interview / essay: talk about **this** system. Put the CV file under `work/relocate/` when Kang asks. No phone/email in `me.md`. Do not send applications unless he asks.

---

## Updated

- **2026-09-17** — first write from interview (identity, 9–5, English, relocate, time).
- **2026-09-17** — named goal #3 is **Learn business domain** (not generic business / MBA).
- **2026-09-17** — rewritten as resume source: Kaopiz, dates, title path, Thang Long CS, FastAPI stack, mixed domains. Named CV project bullets still empty.
- **2026-09-17** — design gaps (several systems): spec-as-design, rules in ifs, hard to change, no boundaries, messy DB, no run/rollback, cannot hand off, AI-fast then no redesign. Cause = lack of knowledge + outsourcing shape. First to close = teach-to-leave (DevOps done).
- **2026-09-17** — handoff fails in several ways (head, no runbook, env, juniors-on-tickets). Teaching at work is not real yet; seminar is later. Done-test for first gap: one work system, another engineer changes+runs a week without pinging me.
- **2026-09-17** — English interviews (1–2): blank, talk that is wrong, regret after. Degree: Thang Long CS, cohort ~2018–2022, finished **2026** (low/no school from ~2022 while working).
- **2026-09-17** — Senior title ~**2025**. Time: late + tired; weeks spike 0 or 2–3; killed by tired and phone.
- **2026-09-17** — Relocate: English life, NZ picked first; **NZ or AU** whichever visa job first. Remote-first OK if it leads to a visa. Visa knowledge thin. IELTS later. Old EN CV overclaims — rewrite from `me.md`. Not applying; blocker = not confident to start.
- **2026-09-17** — One handoff system: Kaopiz internal **SDLC document/QA** tool (generic label). Still mine. Successor not named. This week’s fail: in my head + data model needs me.
- **2026-09-17** — SDLC tool interview: git = document storage (local edit); web = view + comment/review. Mixed project roles. Vue + AI. New (~months). Design to defend: features around the git doc. Debt = extra features mostly failed (AI generate/review, traceability graph) + lots of bugs. “QA” = document review, not test cases.
- **2026-09-17** — Work pattern: highly adaptive; always new projects; rarely > ~7 months on one; depth is hard; keeps seeking new. Document tool = depth bet.
- **2026-09-17** — Document-tool problem (corrected): docs go stale; hard to manage/update with QA; no company-wide shared place.
- **2026-09-17** — Document-tool design path: DB-everything first (docs hard to manage; people work locally) → Git-everything including comments (ACID for comments hard) → split: docs local/Git, features on the server. AI generate/edit was in the first design, not production-ready — that also pushed the local hybrid.
