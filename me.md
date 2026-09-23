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
| **Headline** | **Backend Software Engineer** (mid). Company title is Senior — do not use Senior as the headline on applications. |
| **Pay** | About **32 million VND / month** (stated 2026-09-23). Do not invent gross vs net. |
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

**First gap to close:** another engineer can **change and run one system for a week without pinging me**. That is DevOps “done.” Who uses the document tool, and the rules of that system, belong in the English story and the system-design review for [`goals/relocate.md`](goals/relocate.md). Do not add a separate goal named “learn design” or “architect.”

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

Portal sheet in [`bangdiem.html`](bangdiem.html), pasted **2026-09-23**. Failed attempts and duplicate passes are removed in the markdown. The portal prints credits accumulated **133**, cumulative average **7.51/10**, **3.02/4**. The whole-program line on the same export is **139** credits, **7.19/10**, **2.88/4**. Do not put either average on the public CV unless asked. Full passed rows: [`thang-long-transcript.md`](thang-long-transcript.md).

**Thesis** CS499 (6 credits) **8.7, A**. **Internship** IP401 (2 credits) **8.5, A**.

For advice, not a course list on a CV: high marks are programming, data structures, discrete math, probability (9.0), graphics, software engineering, .NET, testing, and the thesis. Statistics is a **B** (7.6). **D+** on calculus 1, linear algebra, digital engineering, and intro law. DBMS is a **C** (5.8). Networks, formal languages, information theory, and the AI course are **C**. English courses are 18 credits, average about **7.1** (C to B+). Dropped blank courses are not on the list (`CF321`, `SE487`, and blank defense or PE rows).

---

## Languages

| | |
| --- | --- |
| Vietnamese | Native. Work language. |
| English | TOEIC **~750**. Can read and talk daily. **Not** used at Kaopiz. |
| Japanese | Almost none. School only: Japanese 1–2 (7.1 B, 5.5 C). Do not list. |

**Interviews (1–2 real ones):** I go blank; I start talking and it comes out wrong; later I see I knew it. Stall is **how I talk about what I do**, not “no English.” Path: essay first, then speak ([`goals/english.md`](goals/english.md)). Do not prescribe a mock-interview treadmill unless I ask.

---

## Relocate (not a public CV section)

Next job: **mid backend** at a **global product company** in **Hanoi or Ho Chi Minh City**, working language **English**. The New Zealand / Australia visa search is **set aside**. Going abroad is not this goal’s “done.”

- Outsourcing only if product screens produce no interviews.
- CV sending starts **January 2027**, and can stay open through **April 2027**. I am **not applying** before that. Blocker: **not confident to start**. Do not send applications unless I ask.
- Old English CV / LinkedIn **overclaims** (senior / AI / design). Rewrite from this file.

Full goal: [`goals/relocate.md`](goals/relocate.md).

---

## Constraints (for advice)

- **Time:** from **2026-09-24**, at least **1–2 hours a day**, **more on Saturday and Sunday**, for this goal. One must-land file per week. A day counts when a `work/` file moves. Older weeks were often **0 or 2–3** short late sessions, killed by tired and phone.
- **Practice default:** the document tool above. Do not switch to e-commerce/LLM for a better story. Do not invent a successor or a product name.
- **Learning counts** only with a `work/` file (or a reflection). A normal 9–5 day does not.
- **NomStamp** (iOS food-map stamps): dropped hobby. Not a current goal. Not a CV project unless we write a real bullet later.
- A seminar I might teach later is a **wish**, not current work. Do not write mentor / tech lead who grows the team.
- Do not invent jobs, metrics, extra skills, or “I design systems well” as a general claim.

---

## Updated

- **2026-09-17** — first write from interview, then rewritten as CV source (Kaopiz, document tool, honest design limit, relocate, time).
- **2026-09-17** — trimmed: keep facts that change a CV or advice; drop repeated agent/CV checklists and goal-index noise.
- **2026-09-23** — Thang Long portal sheet in `transcript.md`. Education has the computed average, thesis, and the holes. Not an official printed GPA.
- **2026-09-23** — Full portal export. Failed attempts removed. File renamed to `thang-long-transcript.md`. Portal cumulative is 133 credits, 7.51/10, 3.02/4. Probability, statistics, and the AI course are on the pass list.
- **2026-09-23** — Pay stated at about 32 million VND / month. Next job is a global product company in Hanoi or Ho Chi Minh City, English at work. NZ / AU visa search set aside.
- **2026-09-24** — Business-domain goal dropped. Preparation for the job: English, DevOps Handbook plus practice, Python/FastAPI review, system design of the document tool.
- **2026-09-24** — Study time he set: at least 1–2 hours a day, more on the weekend.
