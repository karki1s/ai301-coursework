# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

[issue/67](https://github.com/codepath/pathreview-ai301-fa26-s1/issues/67)

**Verdict output**

Accept

[Your skill's live-mode output for this issue, pasted verbatim and ending with the
fenced JSON verdict block. A summary does not satisfy this field.]

**The verdict must record `accept` for this issue.** Choose an issue your own skill
accepts. If your skill rejects every candidate you try, that is a signal about your
rubric rather than about the issues: revise it and re-run — retries are unlimited and a
partial re-run costs about $0.20 — or run the skill on different candidates. Output
recording `reject` for the issue you chose earns no credit for this field.

```
┌────────────────────┬───────────┬───────┬─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │       Check        │  Weight   │ Grade │                                                                              Evidence                                                                               │
  ├────────────────────┼───────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Maintainer         │ required  │ pass  │ Newest main commit 2026-09-16 by Aburke225 (5 days ago) — well inside 12 months                                                                                     │
  │ activity           │           │       │                                                                                                                                                                     │
  ├────────────────────┼───────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Repo in use        │ required  │ pass  │ Last 5 main commits: 3× 2026-09-16, 2× 2026-08-24 — 5 of 5 within 180 days                                                                                          │
  ├────────────────────┼───────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Scope fits         │ preferred │ pass  │ One function: create_review() in core/services/review_service.py ignores its user_id arg; fix mirrors the existing Profile.user_id join in get_review(). Single     │
  │                    │           │       │ module                                                                                                                                                              │
  ├────────────────────┼───────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ No existing owner  │ required  │ pass  │ 0 comments, 0 assignees, no linked PRs, no cross-references; the repo's only open PR (#74) targets #60                                                              │
  ├────────────────────┼───────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Policy compliant   │ required  │ pass  │ docs/CONTRIBUTING.md says nothing about AI or tooling; no AI policy file; PR template has no disclosure box — silence passes                                        │
  └────────────────────┴───────────┴───────┴─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
  
  Every required check passes → accept. The preferred check also passes, so it ranks well against other accepted candidates: the bug is stated precisely, the correct pattern already exists two functions down in
  the same file, and tier-2 plus the xfail contract in the PR template tell you exactly what "done" looks like.
  
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s1/issues/67",
    "checks": [
      {"name": "Maintainer activity", "grade": "pass",
       "evidence": "Newest main commit 2026-09-16 by Aburke225, 5 days before the 2026-09-21 grading date."},
      {"name": "Repo in use", "grade": "pass",
       "evidence": "Last 5 main commits (3x 2026-09-16, 2x 2026-08-24) are all within 180 days."},
      {"name": "Scope fits", "grade": "pass",
       "evidence": "Body scopes the fix to create_review() in core/services/review_service.py; one module, no redesign."},
      {"name": "No existing owner", "grade": "pass",
       "evidence": "assignees: none; 0 comments; no linked PRs or cross-references; only open PR #74 targets issue #60."},
      {"name": "Policy compliant", "grade": "pass",
       "evidence": "docs/CONTRIBUTING.md and the PR template state nothing about AI-assisted contribution."}
    ],
    "verdict": "accept"
  }   
      
```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

[The agreement score of each run you did, in order. A single run is a complete answer if
only one run occurred. **The last score in your list must match the agreement line in the
`eval-run.txt` you committed** — that file is the record of your final run.]

**Issue analysis**

[One scored issue, identified by id (`issue-01` through `issue-20`; the `calib-`
issues are not scored). State your rubric's decision, the gold label, and the
reasoning that produced your rubric's result.]

**Check rationale**

[One check from the `rubric.md` uploaded to `tools/issue-select/`, quoted as it is
currently written, with the reasoning behind its current form.]

**Trade-offs**

[What the quoted check gives up. Any one of these is a complete answer: an issue whose
result it changes, a canary you re-ran with `--only`, a case you accept it will miss, or a
stated reason nothing changed elsewhere. "Nothing changed, and here is how I know" earns
the point in full when the reason follows.]

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

[Answer all three:

1. The issue's fit to your interests and to the time available.
2. What the verdict identified correctly, and what you weighed that the rubric could
   not.
3. The anticipated difficulty in claiming it.]

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
