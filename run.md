# How we run

[design.md](design.md) is why this system exists. This file is **how a week produces files**.

---

## Start here

**Weekday** — open [now.md](now.md). Do the **must-land** todo (or the ride-along if that file already exists). Copy the template first. 45 minutes. Stop. Check the box only when the file exists.

**Sunday** — copy [reflections/_template.md](reflections/_template.md), sit and write, then rewrite `now.md`. If you skip this, you did not run the system that week.

**Writing or breaking a todo** — it does not go on `now.md` until it is **small**, **actionable**, and **evaluable** (rule below). If it fails any of the three, break it again. Do not put the unbroken version on the list.

Do not start by opening this chat to redesign the system.

---

## Rules for doing

- **Sunday steers. Weekdays ship.** The weekly reflection calibrates goals and rewrites `now.md`. A weekday is not “open `now.md`.” It is a timed session that leaves a file in `work/`.
- **One must-land file per week.** Name it on `now.md`. That file is the week. Everything else rides along, waits, or is bonus. Three book-chunks in parallel is how nothing finishes.
- **Break every todo until it is small, actionable, and evaluable.** If a task is too big, vague, or you cannot say how you will know it is done, it is not a todo yet — break it. All three must pass:
  - **Small:** fits one 45-minute session. “Read Part I” or “a solid chunk” does not. One chapter, one section, or one dump does.
  - **Actionable:** a verb + a thing you can start without another decision. “Start the handbook” does not. “Read the preface and write what it claims DevOps is for” does.
  - **Evaluable:** a yes/no done-test on the todo itself. Usually: the `work/` file exists **and** it answers a named question. “I studied” / “I feel like I started” is not evaluable.
- **A weekday is 45 minutes, one todo.** Same-ish time when you can. When the timer ends, stop. Do not stretch a session into “I’ll finish the solid chunk.”
- **Copy the template first.** The empty file exists before you feel ready. Read, speak, or practice with that file open. Write in your own words until the timer ends.
- **Ugly short files count.** One chapter (or a few pages) plus 10–15 minutes in your own words is a notes file. A perfect unread chapter is not. Check the box when the done-test is true.
- **Ride-alongs share the session.** English speak (5–10 min) happens the same evening as the notes it is about — not a second evening, not after a “solid chunk” exists.
- **The 9–5 dump is short.** Friday, ~10 minutes: write what already touched ship / run / observe / teach (or one deliberate shift). Do not hunt all week for a special DevOps task. No file → that day did not count.
- **Other goals wait.** A secondary book or notes todo starts only after the must-land file exists — or in one weekend slot. Do not give every goal an equal book-chunk.
- **Dates in filenames are names, not deadlines.** Missing Monday is not a reason to skip the week.
- **Empty `- [ ]` lines invite more todos.** Delete them. Do not leave placeholders under a goal.
- **Do not redesign mid-week.** A thought about the framework, a new interest, a doubt: Captures on `now.md`. Decide on Sunday. Another chat that only refines the system is usually fake progress.
- **The agent starts and closes sessions.** It does not replace the session. Starting: you name the todo; the agent copies the template; you write. Done: English review, then you check the box. Sunday: you write the reflection; the agent helps rewrite `now.md`.

---

## A todo on `now.md`

Kind (`notes` / `essay` / `practice`) · action · **Done when:** · path.

Example:

```text
- [ ] notes Read Handbook preface. Write: what it says DevOps is for, and whether that matches my goal.
  Done when: file exists and those two answers are filled
  → work/devops/notes/YYYY-MM-DD-slug.md
```

If you cannot write **Done when** in one line, break the task.

---

## A weekday session

1. Open [now.md](now.md). Pick the must-land todo, or the next one that is unblocked (ride-along, then Friday dump).
2. Copy `work/_templates/<kind>.md` into the path on the todo.
3. Do the work with the file open (read, speak, dump the workday).
4. Fill it in your own words. Fill “serves this goal by.” Hit the **Done when** on the todo.
5. Stop when the timer ends. Link the file. Check the box only if the done-test is true. If not, leave the box open and continue next session — do not enlarge the todo.

If you cannot fill “serves this goal by,” it does not belong this week. Park it in Captures.

How a file is shaped: [work/README.md](work/README.md).

---

## Sunday

Protect a block. Think first, then write. Copy [reflections/_template.md](reflections/_template.md) to `reflections/YYYY-Www.md`. If you skip this, you did not run the system that week.

The questions live in the template and in [design.md](design.md) (weekly session). After the write-up: rewrite `now.md` — one must-land, every todo small / actionable / evaluable, ride-alongs named, stash at most 5, delete the rest.

---

## What to open

| When | File |
| --- | --- |
| Starting a weekday session | [now.md](now.md), then the template |
| File finished | that `work/` file — then check the todo |
| Sunday | [reflections/_template.md](reflections/_template.md), then `now.md` |
| A goal feels wrong | wait for Sunday; then `goals/` |
| You want the why | [design.md](design.md) |
