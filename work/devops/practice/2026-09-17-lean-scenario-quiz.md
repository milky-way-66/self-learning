# Practice

- **Goal:** DevOps
- **Date:** 2026-09-17
- **Serves this goal by:** Apply Lean (value, waste, flow, bottleneck) to the internal SDLC document tool in real scenarios — not a second Handbook chapter.

## What I tried

Five scenario questions on Lean, all on the document tool I still own (docs in Git, comments/review on the server). Not definitions.

## What happened

I can already use: **value vs waste** (review is not waste), **rework**, **do not pass a known problem downstream**, **hotfix ≠ root cause**, waiting and rework as wastes.

The hole is **flow and bottleneck**: who is waiting, what is allowed to start, and whether the system still needs me after the fix.

| Scene | What I got right | What to keep |
| --- | --- | --- |
| Manager: drop comments, merge faster | Cutting review cuts the job of the tool; less discussion → more coding/testing rework | Customer = whose work breaks if the doc is stale, not “employees who maintain files.” Lean is not “spend more time on docs”; waiting in review can still be waste. Keep the **quality gate** (comment, discuss, approve) even if merge is not instant. |
| Schema change only I can do; they write the old way, then migrate | Waiting; rework after I release; “just ship my change” ignores in-flight docs | Faster pings do not remove the **bottleneck**. Flow move: pause review until the schema is in, or move **schema + that one doc** as one piece. Migration is design; it is not a flow change by itself. |
| Markdown in Git = done; open comment “field does not exist”; coding starts | Known problem passed downstream. Done = reviewed and approved | Done is **this document**, on **this Git version**, with **server approve**. Tomorrow’s habit: coding does not start while that comment is open. A DoD page before the task does not stop work already started. |
| Writers merged, reviewers commented, I closed tickets; coding used a stale doc | Merge/tickets can look green while the feature is wrong | Reviewer **comment count** can be a fake local too. A weekly check I can see: did coding use an **approved current** doc? “Make rework visible” is the idea, not the check. |
| I hotfix; nobody can run it; same ping next week | Hotfix treats the visible break, not the root | The Lean name is **bottleneck** (stream cannot run without me) + **no learning**, not only rework. Smallest experiment: someone else **does one thing** (a health check, or one change they repeat without me). Not an architecture doc + conventions + todos in one week. |

## What I would do next time

Ask “who is waiting?” and “what is allowed to start?” before I write more documents. If I am the only person who can change the model, a hotfix is not DevOps done.
