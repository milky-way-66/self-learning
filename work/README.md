# Work

This folder is **the learning, written down**. Goals live in `goals/` (index: `goal.md`). The week lives in `now.md`. `work/` is what you produced.

A checked todo with no file here does not count as learning. Saving a link, a PDF, or someone else’s notes also does not count.

Details of the system are in [design.md](../design.md). How to start a piece of work is below.

---

## Three kinds of work

Every file is one of these. Pick before you start. Copy the matching template from `_templates/`.

| Kind | What you do | Not this |
| --- | --- | --- |
| **Notes** | After you read, watch, or listen, write it in your own words. Use 5W1H (what, who, when, where, why, how) as a prompt — skip what does not apply. Free-form, not a form. | Highlights, copied paragraphs, a bookmark list. |
| **Essay** | Write to think. Argue something (introduction → body → conclusion), explain it as if teaching, or connect two ideas. Longer than notes. | A diary of “I studied today,” or a summary that never takes a position. |
| **Practice** | Do the thing. A lab, a config, a command you ran, a speaking or writing drill. Record what you tried, what happened, what you would do next time. | “I should try X” with no attempt. |

Current goals (DevOps, English, Business domain, Relocate) use the same three kinds. The goal changes the material, not the shape. Dropped goals may still have evidence under `work/<slug>/`.

---

## Where a file goes

```text
work/
├── _templates/          # copy these, don’t write in them
│   ├── notes.md
│   ├── essay.md
│   └── practice.md
├── devops/
│   ├── notes/
│   ├── essays/
│   └── practice/
├── english/
│   ├── notes/
│   ├── essays/
│   └── practice/
├── business/
│   ├── notes/
│   ├── essays/
│   └── practice/
└── relocate/
    ├── notes/
    ├── essays/
    └── practice/
```

Name: `YYYY-MM-DD-short-slug.md`

Examples: `devops/notes/2026-09-03-k8s-probes.md`, `english/essays/2026-09-04-why-i-avoid-speaking.md`, `business/practice/2026-09-10-domain-of-one-system.md`

---

## How a weekday task becomes a file

The session itself is in [run.md](../run.md) (start here, timer, must-land, copy the template first). A todo must be small, actionable, and evaluable before you start it. The file steps:

1. The todo in `now.md` names the **goal**, the **kind**, and how it serves the goal.
2. Copy `_templates/<kind>.md` into the matching folder — before you read or practice.
3. Write. In your own words. Fill “serves this goal by.”
4. Link the file on the todo. Then check it off.

If you cannot fill “serves this goal by,” it does not belong in `work/` this week. Park the idea in Captures on `now.md`.
