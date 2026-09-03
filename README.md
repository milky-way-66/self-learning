# Self-learning

Hold **named goals**. Plan **this week**. Do the work in your own words. **Once a week, sit down and write.**

Question yourself. Keep the goals in view. Reading, essays, and practice exist to serve the goals — they are not the point by themselves.

Why the system is built this way: [design.md](design.md).

---

## Current goals

See [goal.md](goal.md). Fill those sections before you make todos.

1. **Learn DevOps**
2. **Learn English**
3. **NomStamp (iOS)** — 100 returning users

A week does not have to treat every goal equally. It does have to name which goals it is for. A new interest waits in Captures on [now.md](now.md) until a weekly reflection says it is a goal. The **9–5 SWE job** is a practice channel for DevOps/English (learn from work, or shift work to learn more) — not a separate goal. Evidence still goes in `work/`.

---

## The loop

1. **Goals** live in [goal.md](goal.md). Hold them for weeks or months. Change a goal only after a weekly reflection.
2. **This week** lives in [now.md](now.md): short intent, todos, a 3–5 item “next” stash (not a plan), optional captures.
3. **Do the work.** Each todo is notes, essay, or practice. It produces a file under [work/](work/README.md). Check the box only when that file exists.
4. **Once a week, sit down and write.** Copy [reflections/_template.md](reflections/_template.md) to `reflections/YYYY-Www.md`. Think. Answer it. If you skip this, you did not run the system that week.
5. Rewrite [now.md](now.md) for the next week. Pull from the stash. Drop what no longer serves a goal.

Weekdays: open `now.md`. Sunday (or whenever you protect the block): write the reflection, then replan.

---

## What to open

| File | When |
| --- | --- |
| [goal.md](goal.md) | A goal changed (rare) |
| [now.md](now.md) | Any weekday — plan, todos, captures |
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
├── README.md                 # This file — how to run the system
├── design.md                 # Why it is built this way
├── goal.md                   # Current named goals
├── now.md                    # This week only
├── reflections/
│   ├── _template.md
│   └── YYYY-Www.md
└── work/
    ├── _templates/           # notes / essay / practice
    ├── devops/notes|essays|practice/
    ├── english/notes|essays|practice/
    └── nomstamp/notes|essays|practice/
```

Markdown only. No issue backlog, no far-horizon plan.
