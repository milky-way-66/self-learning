---
name: review-english-writing
description: >-
  Review English writing in this self-learning repo (notes, essays, practice,
  reflections) for grammar, spelling, word choice, and clarity. Use when the
  user finishes a work file and asks to review writing, check grammar, proofread,
  improve English, or run a writing review on a note/essay. Also use when the
  project rule requires a writing review after finishing work/ or reflections/ prose.
---

# Review English writing

Teachable feedback for learning English as a **work language** (docs, tickets, reviews, teaching notes). Not literary polish. Not native-like perfection.

## When invoked

1. Identify the target file(s):
   - Prefer the file the user named or has open.
   - Else the `work/` note/essay/practice they just wrote.
   - Else `git diff` / recent files under `work/` or `reflections/`.
2. Read the full file before commenting.
3. Review only the user’s prose (skip YAML-ish metadata lines if empty; still check filled fields like “Serves this goal by”).
4. **Do not edit the file** unless the user explicitly asks you to apply fixes. Default = report only so they learn by rewriting.

## What to check

Prioritize what blocks **clear professional English**:

| Priority | Look for |
| --- | --- |
| High | Grammar that changes meaning; wrong tense/aspect; subject–verb agreement; articles (a/an/the) when missing or wrong; broken sentence structure |
| High | Spelling / typos |
| Medium | Word choice (wrong word, awkward collocation, unclear verb); prepositions |
| Medium | Clarity: vague claims, run-ons, missing logical link between sentences |
| Low | Style polish, more “natural” phrasing when meaning is already clear |

Ignore:

- Template headings and empty sections
- Vietnamese content if intentional (e.g. VN seminar delivery notes)
- Demanding native idioms or fancy vocabulary
- Rewriting their ideas or “Serves this goal by” intent

## Learner profile (use this)

- Approx. TOEIC ~750; strong input, weaker production
- Goal: English others can act on at work — not exam English
- Prefer short explanations of *why* a fix works
- Common L1 patterns to watch (only flag when present): missing articles, verb tense slips, “how to” / infinitive mixups, word order calqued from Vietnamese, overlong sentences without connectors

## Output format

Make the review **easy to scan and fix one row at a time**. Prefer tables over long bullet trees. No walls of prose.

Use this structure every time:

```markdown
## Writing review: `<path>`

| | |
| --- | --- |
| **Readable?** | Clear / Mostly clear / Hard to follow |
| **Must fix** | N |
| **Optional** | N |
| **Next focus** | one short skill to practice (e.g. articles) |

### Must fix

| # | Type | Yours | Try instead | Why |
| --- | --- | --- | --- | --- |
| 1 | grammar | `exact quote` | `corrected quote` | short reason |
| 2 | spelling | `...` | `...` | ... |

Types only: `grammar` | `spelling` | `word` | `clarity`

### Optional

Same table shape. Only if useful; omit the section if empty.

### Already good

- one short bullet
- one short bullet

### Fix checklist

Copy for the learner to tick while editing:

- [ ] #1
- [ ] #2
```

Rules for the tables:

- **Yours** / **Try instead** = short exact quotes (one phrase or one sentence), in backticks. Not a paraphrase of the whole paragraph.
- One issue per row. If the same mistake repeats, one row + “also on lines …” in Why.
- Put the worst meaning-breakers first.
- Cap Must fix at 8 rows, Optional at 5.
- Do **not** dump a full rewritten file unless the user asks.

## If they ask to apply fixes

1. Apply only agreed items (or all Must fix if they say “fix all”).
2. Preserve meaning and structure of notes/essay/practice templates.
3. Re-read and confirm no template fields were wiped.

## Examples of triggers

- “Review the English in this note”
- “Check grammar on my essay”
- “Writing review for `work/devops/essays/...`”
- “I finished the notes — proofread please”
