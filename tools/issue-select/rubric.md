# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
|Maintainer activity |The last 15 default-branch commit dates and the issue comment thread |There is evidence of maintainer/core-contributor activity within the past 12 months, shown by at least 1 recent default-branch commit or a maintainer/core-contributor response in the issue thread|required|
|Repo in use |The last 5 default branch commit dates|At least 2 of the last 5 default-branch commits occurred within the past 180 days |rquired|
|Scope fits |Issue body and comment thread, including the described task and implementation requirements|The issue describes one clearly bounded change that does not require a broad architectural redesign or changes across more than 3 major components or modules|preferred|
|No existing owner|The issue body and complete comment thread, including linked PRs|No contributor has explicitly claimed the issue, said they are working on it, or opened a PR that addresses the issue|required|
|Policy compliant|The issue body and comment thread, plus the policy criteria in references/evidence-guide.md|The issue does not request or require a change that violates the stated repository/project policy| required|
## Verdict rule

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->
Accept only if every required check passes. Preferred checks never change the verdict and are used only to rank accepted issues. Treat unclear as fail for required checks and as neutral for the preferred check.
