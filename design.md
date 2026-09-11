# Goal-centric learning

The center of this system is **your current goals**. Everything else exists to serve them.

You can hold more than one. Right now that means **learn DevOps**, **learn English**, **learn business**, and **relocate** (NZ first, or another English-working country). Keep the list small and named. A pile of themes is not a set of goals.

The core practice is to **keep questioning yourself** and **keep the goals in view**. Reading, essays, experiments, and other tasks are how you learn — they are not the point by themselves. If a task does not serve a named goal, it does not belong in the week.

---

## The loop

1. Hold your **current goals** as one file each under `goals/` (index in `goal.md`). Keep them for weeks or months. Add, drop, or rewrite a goal only when a weekly reflection says it is clearly wrong — or clearly missing. When you rewrite, append one line to that file’s **History**.
2. Plan **this week only** in `now.md`: a short intent per goal you will touch, a todo list tagged to a goal, and a small “next” stash (3–5 bullets, not a plan).
3. **Do the work.** Each todo produces a file in `work/`: **notes**, **essay**, or **practice**. Check it off only when that file exists. How a weekday actually does this: `run.md`.
4. **Once a week, sit down and write.** Copy `reflections/_template.md` into a dated file. Think. Answer the questions honestly. This session is required. If you skip it, you did not run the system that week.
5. After the session: rewrite `now.md` for the next week. Pull from the stash, drop what no longer serves a goal, and add at most 3–5 new stash items. If a goal finished or dropped: move it to `goals/finished/` and update `goal.md`.

Weekdays you run a session (`run.md`), not only open `now.md`. Optional mid-week captures live there if something hits you. They are never required.

A week does not have to treat every goal equally. It does have to name which goals it is for, and it must not invent an unofficial goal as “just this once.”

---

## Layout

```text
├── README.md                 # How to use this repo
├── design.md                 # This file — why the system works this way
├── run.md                    # How a week produces files (rules for doing)
├── goal.md                   # Index of current goals (links only)
├── goals/
│   ├── _template.md          # New current goal
│   ├── <slug>.md             # One file per current goal (+ History)
│   └── finished/             # Done or dropped goals
│       ├── _template.md
│       └── YYYY-MM-<slug>.md
├── now.md                    # This week’s plan, todos, next stash, captures
├── reflections/
│   ├── _template.md          # Copy this for the weekly session
│   └── YYYY-Www.md           # One write-up per week
└── work/                     # Learning output — see work/README.md
    ├── _templates/           # notes / essay / practice
    ├── devops/notes|essays|practice/
    ├── english/notes|essays|practice/
    ├── business/notes|essays|practice/
    └── relocate/notes|essays|practice/
```

Dropped-goal evidence may still live under `work/<slug>/`.

Markdown only. No GitHub issues, no quarterly OKRs, no second-brain wiki, no daily logs.

---

## Rules

- **Named goals only.** Each current goal is `goals/<slug>.md`, listed in `goal.md`. Do not let a new interest become a goal mid-week. Park it in Captures and decide on Sunday.
- **This week is the plan.** The stash is a reminder so Sunday is not empty. It is not a backlog. Cap it at 3–5 items. Delete freely.
- **Every todo is tagged to one goal** and says how it serves that goal. If you cannot say it in one line, it does not go on the list.
- **Every todo is small, actionable, and evaluable** before it goes on `now.md`. If not, break it. Details: `run.md`.
- **The day job is a channel, not a goal.** 9–5 SWE work can serve DevOps, English, Business, or Relocate when you either (a) learn from what you already did and write notes/practice, or (b) deliberately shift a task toward ship / run / observe / teach / work English / value-cost-metric talk / real search (CV, applications). A practice todo names which goal that hour serves. A normal day with no file in `work/` does not count.
- **The weekly session is the calibration.** You question yourself, you question the week, you question each goal. Default is to keep a goal. You change it only when the answer is clearly no. Rewrites go in the goal file; append **History**.
- **Finished goals leave the current list.** Move to `goals/finished/` with Status / Closed on / How I know. Keep `work/<slug>/` as evidence.
- **Output in `work/` is the evidence.** A checked box without a notes, essay, or practice file does not count. Bookmarks and copied text do not count.
- **Weekdays follow `run.md`.** One must-land file, a timed session, ride-alongs on the same evening. Do not add a fourth planning layer.

---

## Files

### `goal.md` and `goals/`

`goal.md` is only the **index** of current goals. The real text lives in `goals/<slug>.md` (slug matches `work/<slug>/`).

Each goal file includes why it matters, what “done” looks like, what you will not chase, and an append-only **History**: first line = defined; later lines = what changed after a reflection. The top of the file is always the current wording — not a stack of old full drafts. Git still has full diffs if you need them.

When a reflection closes a goal, copy it to `goals/finished/YYYY-MM-<slug>.md` (keep History), remove `goals/<slug>.md`, and drop the row from `goal.md`.

### `now.md`

The only file you need on a weekday.

- **This week** — which goals you will touch, and how, in a few sentences.
- **Todos** — grouped by goal. Each names a kind (`notes` / `essay` / `practice`) and links the file when it exists.
- **Next** — 3–5 bullets of likely next work, each tagged to a goal. No dates, no fake schedule.
- **Captures** — optional. A thought, a question, a doubt, a possible new goal. Dump it here so it survives until Sunday.

At the start of each week, replace last week’s todos. Do not let `now.md` become a history file. History of *learning* belongs in `reflections/` and `work/`. History of *goal wording* belongs in each goal’s History list (and git).

### `reflections/`

One file per week, named `YYYY-Www.md` (example: `2026-W36.md`). Write in full sentences. The template is a set of questions, not a status report. Stay in the chair until you have actually thought. Walk each named goal; also ask one question about *you*.

### `work/`

This is the learning, written down — not a dump of links.

Three kinds only:

- **Notes** — after input, explain it in your own words.
- **Essay** — write to think; take a position.
- **Practice** — do the thing and record the attempt.

Path: `work/<goal>/<kind>/YYYY-MM-DD-slug.md`. Copy from `work/_templates/`. How to use it is in `work/README.md`.

---

## The weekly session

Protect a block of time. Think first, then write. Do not fill this in as a chore at midnight.

1. Restate each current goal in your own words, without looking. Then look at `goal.md` / `goals/`. If they do not match, that is the first finding.
2. What did you actually do this week? Facts, not mood. Sort it by goal.
3. What moved each goal? Point at files in `work/`, or admit that a goal did not move.
4. What looked like work but was not (interesting, busy, unrelated to any named goal)?
5. What question should you be asking yourself right now — about you, not about the task list?
6. What did you learn that you can explain in your own words? (Per goal if needed.)
7. For each goal: still the right one? Yes or no. If no: why, and what replaces it? If rewriting: update `goals/<slug>.md` and append History. If finished/dropped: move to `goals/finished/`. If a new goal wants in: why, and which existing one (if any) loses a seat? Update `goal.md` before you plan the next week.
8. Given that, what is next week *for*? Which goals get time? Then rewrite `now.md`.

---

## Looking back (e.g. six months)

1. Open `goal.md` + each `goals/<slug>.md` **History** — how the aim changed since first define.
2. Skim `goals/finished/` — what you closed and why.
3. List files under `work/<slug>/` and read the weekly `reflections/` for that window.
4. Judge each “done” against evidence. Then rewrite or close goals as above.

---

## What we dropped on purpose

The previous design mixed OKRs, GitHub sprint issues, a work-learning matrix, daily logs, and a knowledge wiki. That buried the goals and invited planning too far ahead.

This version is the loop only: hold named goals, plan a week, do learning work, question yourself in writing, repeat.
