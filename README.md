# Self-learning

Hold **named goals**. Plan **this week**. Do the work in your own words. **Once a week, sit down and write.**

Question yourself. Keep the goals in view. Reading, essays, and practice exist to serve the goals — they are not the point by themselves.

Who this is for: [me.md](me.md). Why the system is built this way: [design.md](design.md). How a week produces files: [run.md](run.md).

---

## Current goals

See [goal.md](goal.md) (index). Full text: one file per goal under [goals/](goals/).

1. **Global product company (English, Vietnam)** — [goals/relocate.md](goals/relocate.md)
2. **Learn English** — [goals/english.md](goals/english.md)
3. **Learn DevOps** — [goals/devops.md](goals/devops.md)

A week does not have to treat every goal equally. It does have to name which goals it is for. A new interest waits in Captures on [now.md](now.md) until a weekly reflection says it is a goal. The **9–5 SWE job** is a practice channel for the global product-company job, English, and DevOps (learn from work, or shift work to learn more) — not a separate goal. Evidence still goes in `work/`. A practice todo names which goal that hour serves.

Finished or dropped goals: [goals/finished/](goals/finished/). Each current goal file has a **History** list so you can see what changed since you first defined it.

---

## The loop

1. **Goals** live in [goals/](goals/) (index: [goal.md](goal.md)). Hold them for weeks or months. Change a goal only after a weekly reflection; append **History** when you rewrite. Close into [goals/finished/](goals/finished/).
2. **This week** lives in [now.md](now.md): short intent, todos, a 3–5 item “next” stash (not a plan), optional captures.
3. **Do the work.** Each todo is notes, essay, or practice. It produces a file under [work/](work/README.md). Check the box only when that file exists. How: a timed weekday session — [run.md](run.md).
4. **Once a week, sit down and write.** Copy [reflections/_template.md](reflections/_template.md) to `reflections/YYYY-Www.md`. Think. Answer it. If you skip this, you did not run the system that week.
5. Rewrite [now.md](now.md) for the next week. One must-land file. Pull from the stash. Drop what no longer serves a goal.

Weekdays: run a session ([run.md](run.md)). Sunday (or whenever you protect the block): write the reflection, then replan.

---

## What to open

| File | When |
| --- | --- |
| [me.md](me.md) | A **fact about you** is wrong (name, job, stack, time, English, relocate) — not a weekly rewrite |
| [goal.md](goal.md) / [goals/](goals/) | A goal changed (rare); History shows rewrites since first define |
| [goals/finished/](goals/finished/) | A goal is done or dropped |
| [now.md](now.md) | Any weekday — plan, todos, captures |
| [run.md](run.md) | **Start here** on a weekday — rules for doing |
| [work/README.md](work/README.md) | Starting notes / an essay / practice |
| [reflections/_template.md](reflections/_template.md) | The weekly think-and-write session |
| [design.md](design.md) | You need the why, not the how |

---

## Work: notes, essay, practice

`work/` is the learning, written down. Bookmarks, PDFs, and copied text do not count.

| Kind | What you do |
| --- | --- |
| **Notes** | After you read or watch, explain it in your own words. |
| **Essay** | Write to think. Take a position. |
| **Practice** | Do the thing (lab, drill, config) and record the attempt. |

Path: `work/<goal>/<kind>/YYYY-MM-DD-slug.md`. Copy from `work/_templates/`. Full rules: [work/README.md](work/README.md).

---

## Layout

```text
├── README.md                 # This file — map of the repo
├── me.md                     # Stable facts about you (not a goal)
├── design.md                 # Why it is built this way
├── run.md                    # How a week produces files (rules for doing)
├── goal.md                   # Index of current goals
├── goals/
│   ├── _template.md
│   ├── <slug>.md             # Current goal + History
│   └── finished/             # Done or dropped
├── now.md                    # This week only
├── reflections/
│   ├── _template.md
│   └── YYYY-Www.md
└── work/
    ├── _templates/           # notes / essay / practice
    ├── devops/notes|essays|practice/
    ├── english/notes|essays|practice/
    └── relocate/notes|essays|practice/
```

Markdown only. No issue backlog, no far-horizon plan.
