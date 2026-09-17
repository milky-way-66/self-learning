# Me

Facts for **search, advice, and a CV**. Not a goal. Not this week’s plan. No phone or email here.

- Goals: [`goal.md`](goal.md) · This week: [`now.md`](now.md) · Evidence: [`work/`](work/README.md)
- Public CV: [`index.html`](index.html). A file under `work/relocate/` is generated **from this file**.

Change a line when a **fact is wrong**. Append **Updated**.

---

## Identity

| | |
| --- | --- |
| **Name** | Long. People call me **Kang**. CV name: **Long**. |
| **Where** | Hanoi, Vietnam. Would move **solo**. |
| **Headline** | **Backend Software Engineer** (mid overseas). Company title is Senior — do not use Senior as the overseas headline. |
| **9–5 language** | Vietnamese. **Not** English. **Not** Japanese. |

---

## Work

**Kaopiz Software** (Japanese outsourcing, Hanoi). Software for Japan companies, from **their requirements**.

| Period | Title |
| --- | --- |
| Aug 2021 – Aug 2022 | Intern |
| Aug 2022 – present | Full-time, junior → **Senior Software Engineer** (title about **2025**) |

About **5 years**. Team usually **2–5**. I sit in architecture + data; others implement with me. I review and explain. That is the *seat* — not “someone else can run it without me.”

**Stack I have used at work:** Python, FastAPI, PostgreSQL, SQLAlchemy, Celery, Docker, REST. Sometimes Vite. LLM features as **application software**, not ML research. Vue.js only on the document tool below (AI-coded; not a Vue headline).

**How I actually work:** known as **highly adaptive** — new problem, still ship. I keep getting **new projects**. I also keep seeking the next new thing. **Cost:** rarely more than about **7 months** on one project. Wide, not yet deep. One employer — not a job-hopper. Do not write “5 years on one product.”

**Honest level:** most of that work **lacks design** (spec was the design; rules in if-statements; hard to change; messy data; I cannot run / roll back / teach it). **Exception — the only system I will defend as designed:** the internal document tool below. Company-Senior is not a general architecture claim.

**Other work (true, delivery only, do not say I designed them well):** e-commerce / orders, LLM-as-software, other internals, legacy I took over.

**First gap to close:** another engineer can **change and run one system for a week without pinging me**. That is DevOps “done.” Domain (who uses it, what job it does, 2–3 rules) is [`goals/business.md`](goals/business.md). Do not add a fifth goal named “learn design.”

---

## The system I still own

**Label (no product name):** Kaopiz **internal SDLC document tool**. Company software documents — not a Japan-client app. About **a few months** old. Mixed roles on a project use it (not QA-only). I **still own** it. Successor **not chosen**. Data-model changes still need me. High debt; lots of bugs.

**Problem:** documents went **outdated**; **hard to manage and update with QA**; **no shared place** for the company.

**Job:** one company place for software documents + review. **“QA” = review the document** (comment, discuss, approve). Not a test-case / bug-tracker product. Do not write ISTQB.

**What shipped:** docs live **locally in Git** (GitLab / Bitbucket). Comments and other features live **on the server**. Vue UI.

**How we got there (tell this, not only the end state):**

1. Everything in the **database** — documents were hard to manage; people already work locally.
2. Everything in **Git**, including comments — **ACID** for comments was hard.
3. **Split.** First design also had **AI generate and AI edit**; that was not production-ready, which also pushed the local hybrid.

Also failed (do not list as shipped): **AI review**, **traceability graph**. Do not call this an AI product. Do not invent a product name or user counts.

**CV bullet (this system only):** Designed and built from scratch an internal SDLC document tool. Tried DB storage first (docs hard to manage); then Git for everything including comments (ACID for comments was hard); now docs live locally in Git, comments and other features on the server. Python / FastAPI / PostgreSQL; Vue UI. Used AI to code faster. First design also had AI generate/edit — not production-ready. High debt; I still own schema changes.

---

## Skills

| Use | |
| --- | --- |
| Languages | Python |
| Backend | FastAPI, REST, Celery |
| Data | PostgreSQL, SQLAlchemy |
| Ship | Docker |
| Sometimes | Vue.js (document tool only); Vite; LLM APIs as app features |

**Do not headline:** AWS / K8s / SRE; Japanese; ML / AI specialist; English as a work language; one industry expert; “architect” in general; this tool as test-case QA or as an AI-doc product.

---

## Education

**B.Sc. Computer Science**, Thang Long University, Hanoi. Cohort about **2018–2022**. Little/no school from **~2022** (working). Degree finished **2026**. A CV may say 2026. Do not imply full-time student 2022–2026. Do not hide the degree.

---

## Languages

| | |
| --- | --- |
| Vietnamese | Native. Work language. |
| English | TOEIC **~750**. Can read and talk daily. **Not** used at Kaopiz. |
| Japanese | Almost none. Do not list. |

**Interviews (1–2 real ones):** I go blank; I start talking and it comes out wrong; later I see I knew it. Stall is **how I talk about what I do**, not “no English.” Path: essay first, then speak ([`goals/english.md`](goals/english.md)). Do not prescribe a mock-interview treadmill unless I ask.

---

## Relocate (not a public CV section)

Live where work is in English. **NZ first** (life in English, not a researched visa plan). **Australia** also OK. First offer: **whichever mid-level backend visa job comes first (NZ or AU)**.

- Role: mid **backend** on a **work visa**. Not company-Senior, not ML.
- Remote-first is OK **if it can lead to a visa**. Not remote-forever / EOR with no visa path.
- Visa knowledge is **thin**. IELTS/PTE later, when asked.
- Old English CV / LinkedIn **overclaims** (senior / AI / design). Rewrite from this file. I am **not applying**. Blocker: **not confident to start** — not missing IELTS, not missing a new portfolio. Do not send applications unless I ask.

Full goal: [`goals/relocate.md`](goals/relocate.md).

---

## Constraints (for advice)

- **Time:** ~**45 minutes**, **late**, often tired. Weeks are **0 or 2–3** sessions, not a weekday habit. Killed by tired and phone. One must-land file per week. Do not plan “most evenings.”
- **Practice default:** the document tool above. Do not switch to e-commerce/LLM for a better story. Do not invent a successor or a product name.
- **Learning counts** only with a `work/` file (or a reflection). A normal 9–5 day does not.
- **NomStamp** (iOS food-map stamps): dropped hobby. Not a current goal. Not a CV project unless we write a real bullet later.
- A seminar I might teach later is a **wish**, not current work. Do not write mentor / tech lead who grows the team.
- Do not invent jobs, metrics, extra skills, or “I design systems well” as a general claim.

---

## Updated

- **2026-09-17** — first write from interview, then rewritten as CV source (Kaopiz, document tool, honest design limit, relocate, time).
- **2026-09-17** — trimmed: keep facts that change a CV or advice; drop repeated agent/CV checklists and goal-index noise.
