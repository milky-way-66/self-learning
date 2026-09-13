# Review: what is Lean

- **Target:** [2026-09-14-what-is-lean.md](./2026-09-14-what-is-lean.md)
- **Round:** 2 (2026-09-13)
- **How to use:** Tick a box when that item is fixed in the essay. Ask for round 3 after a pass.

| | |
| --- | --- |
| **Readable?** | Mostly clear |
| **Content** | Better (Three Ways are named). Two claims still fight the Handbook. |
| **Presentation** | Same spoken lecture shape. Intro and close still weak. |
| **English** | Same spelling/grammar load. One new broken sentence in the Third Way. |
| **Next focus** | Reconcile one-way flow with feedback. Then a spelling sweep (*performance, individual, stream, definition, achieve, continuously*). |

---

## Round 2 — what changed

| Previous issue | Now |
| --- | --- |
| Promised three Ways, wrote only flow | **Fixed.** Second Way (feedback) and Third Way (learn from failure) are in the essay. |
| System performance = sum of people | **Partial.** You now include workflow, not only individuals. Still sounds like “add the parts.” Lean: optimize the **flow**; individual speed can make the stream worse. |
| `it necessery` (missing verb) | **Partial.** Now `it's necessery` — verb is there; spelling is still *necessary*. |
| Dev vs QA “couldn’t be solved” | **Open.** Unchanged. |
| Flow only one direction | **Open.** Worse now: the First Way still says one direction only, then the Second Way sends feedback back. |
| Weak why / no waste examples / pep-talk close | **Open.** Unchanged. |

---

## 1. Content — still open

Tick when the essay itself is fixed, not when you agree in chat.

- [ ] **C1 — Flow vs feedback (highest).** First Way: work should only go one way. Second Way: feedback should reach the system. Both can be true if you split them: **work/value flows forward; feedback flows back.** One sentence in the First Way bullet is enough. Right now the two Ways contradict.
- [ ] **C2 — Dev vs QA is not unsolvable.** Keep: local goals can clash. Change: Lean/DevOps **reduce** that clash with one shared goal (customer-usable value, no hidden defects). “Natural conflict that couldn’t be solved” is the opposite of the point.
- [ ] **C3 — System / flow.** Don’t say flow performance is “created by” individual performance. Say: the stream’s performance is the **flow between steps**; we improve people *and* the path, but a local win that slows the next step is not a win.
- [ ] **C4 — Why Lean.** Replace “we want to be good and better.” Use: faster value, less waiting/rework, quality at the source.
- [ ] **C5 — Thesis up front.** One or two sentences: Lean is how we run a system so work flows toward customer value with less waste — and that is the base of DevOps. Then the five questions + Three Ways.
- [ ] **C6 — Close.** Drop “stay alive / stay awake.” End with what to reuse: (1) value then stream, (2) problems stop at the source, (3) local speed that hurts the stream is not improvement, (4) feedback + safe learning. Optionally: one real loop from your job.

**Thin but OK for now (no tick required):** Second and Third Ways are short. Content is roughly right. Later: Second Way = fast right-to-left signal (test, prod, customer). Third Way = experiment, learn from failure, don’t punish honest misses — that is not the same as shipping a **known** defect (First Way).

**Already good (content):**

- Lean = deliver value with less waste; five questions; IT stream = idea → running service → operate.
- You named all Three Ways. Don’t un-name them.

---

## 2. Presentation — still open

- [ ] **P1 — Cut throat-clearing.** Delete or rewrite `So` / `Oke` / `well` / `this essay will explain` / `And that is Lean`. First sentence of each paragraph = the point.
- [ ] **P2 — Number the five questions** `1–5`. You already have First / Next / Then / Other / Last; numbers scan at work.
- [ ] **P3 — Shorten the four flow bullets.** Pattern: **name → one sentence what → one sentence why.** Each bullet is a paragraph now.
- [ ] **P4 — Label the First Way** the same way as the others (`First Way: flow`, `Second Way: feedback`, `Third Way: learning`). The last two are named; the first is still “optimize performance.”
- [ ] **P5 — Intro / body / close jobs.** Intro = thesis + preview. Body = five questions, then IT stream, then Three Ways. Close = what to reuse, not a pep talk.

**Already good (presentation):**

- Order of ideas is still the right spine.
- “The second way” / “the third way” is clearer than the old “three ways (for now)” with only one way written.

---

## 3. Grammar and vocab

| | |
| --- | --- |
| **Must fix** | 8 |
| **Optional** | 5 |

### Must fix

| # | Type | Yours | Try instead | Why |
| --- | --- | --- | --- | --- |
| 1 | grammar | `how we it effect the software development` | `how it affects software development` | Broken word order. *Affect* = verb; *effect* = usually a noun. Also: `idea that effect the devops`. |
| 2 | grammar | `Thing of lean is way we continus practicing` | `Think of Lean as a way we continuously practice` | *Thing* vs *Think*. Need *as a way*. *Continuously* = adverb. |
| 3 | word | `local optimization to defect the gloabl perfomance` | `local optimization to hurt global performance` | *Defect* = a flaw, not “damage.” Also *global* / *performance*. |
| 4 | word | `then thought the development` | `then through development` | *Thought* = past of *think*. *Through* = along the path. |
| 5 | grammar | `we having three ways` | `we have three ways` | Use *have*. Same pattern: `we practicing`, `This happend`, `between the, by optimize`. |
| 6 | spelling | `devliver` / `resouce` / `indivitual` / `defination` | `deliver` / `resource` / `individual` / `definition` | Same extra/missing-letter pattern also: *necessery, helpfull, undertand, genaral, achive, continus, pravtices, requrire, attection, responsiple, downsteam, wheter, happend, bettwen, practive, insteed, steam, provice, possiple, environement, failture*. |
| 7 | grammar | `what problem we are trying to solved` | `what problem we are trying to solve` | After *to*, use the base verb. Also `couldn't be solve` → `could not be solved`. |
| 8 | grammar | `Failure is bad it it necessery for learning` | `Failure is costly, but it is necessary for learning` | Double *it*; need *but*; *necessary*. New in the Third Way paragraph. |

### Optional

| # | Type | Yours | Try instead | Why |
| --- | --- | --- | --- | --- |
| 1 | word | `zero wasted` / `lowest wasted` | `zero waste` / `the least waste` | *Waste* = noun. *Wasted* = adjective. |
| 2 | grammar | `5 question` | `five questions` | Plural. Also `these work` → `this work`. |
| 3 | word | `why we should lean it` | `why we should learn it` | *Lean* = the method. *Learn* = study. |
| 4 | grammar | `the the nearest place where it occur` | `the nearest place where it occurs` | Double *the*. *It occurs*. |
| 5 | clarity | `Stay alive and stay a wake, me and my friend as we continue this.` | Delete. | Spoken close. *Awake* is one word. |

### Already good (English)

- `it's necessery` is closer than `it necessery` — you added the verb.
- Core line is still the right definition: deliver value with less waste (then fix *deliver* / *resource* / *the customer*).
- New Third Way words (*failure, experiment, resilient*) are the right vocabulary once spelling is clean.

### Fix checklist (English)

- [ ] #1 affect / `how we it`
- [ ] #2 *Think of Lean as… continuously practice*
- [ ] #3 *defect* → *hurt* (or *damage*)
- [ ] #4 *through* development
- [ ] #5 *have* / *happened* / *them* / *by optimizing*
- [ ] #6 spelling sweep
- [ ] #7 *to solve* / *be solved*
- [ ] #8 Third Way: *costly, but necessary*

---

## Suggested order for the next pass

1. Content **C1** (flow vs feedback) and **C2** (Dev/QA).
2. Intro thesis **C5** + close **C6**.
3. English checklist #1–#8 (one row at a time).
4. Presentation P1–P4 if energy left.

Do not rewrite the whole file in one shot. Round 3 = this file with more ticks, then another review.
