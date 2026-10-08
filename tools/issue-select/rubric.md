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

## Checks

|Check|Evidence|Pass condition|Weight|
|-|-|-|-|
|Not-claimed|Assignee, “I’m working on this” comments, linked PRs|No assignee, no recent claim, no open PR|Required|
|Expected-actual-behavior|Lines describing what should happen and what does happen|Both can be quoted|Preferred|
|Specific-change|Issue title, body and labels; the opener’s role (MEMBER, COLLABORATOR, OWNER, CONTRIBUTOR, NONE); comment count and linked PRs|Check the Fail rules first. Fail if the issue: (a) is a tracking list or “megaissue” made of links to other issues; (b) asks for changes “across the codebase” or “incrementally”; (c) has 30+ comments of unresolved debate or abandoned PRs; (d) is a feature request that no maintainer has endorsed and that needs a product decision. Otherwise pass if the issue names the concrete thing to change (a command, UI element, behavior or doc page). A bug report (bug label) filed by a MEMBER, COLLABORATOR or OWNER passes even if it’s short, says “several” or “etc.”, or lists possible causes; treat “suggestions” as optional extras, not extra scope|Required|
|Active-maintainer-engagement|maintainer first-response sample” in Repo facts, plus maintainer comments on this issue|A maintainer replied within about 30 days in the sample, or a maintainer commented on the issue|Preferred|
|Fits-time-available|Files or areas named, size words like “refactor”|Looks like ≤3 files, no breaking change|Preferred|
|Technical-specs-requirements|Versions, OS, tools needed|Stated, and no special access needed|Preferred|
|Active-release-cycle|Release or tag dates|A release in about the last 6 months|Preferred|
|Maintainer-recent-commits|last 5 default-branch commits” dates in the Repo facts block|The newest commit is within 90 days of the bundle's captured date, and the repo is not archived|Required|
|Policy-allows-contribution|The "contribution policy" line in the Repo facts block|Pass if the policy is silent("no statement on AI") or allows AI-assisted contributions, even with conditions like "you must review it." fail if it bans AI generated code or docs, or limits contributions to maintainers only|Required|

## Verdict rule

Accept only if every Required check is P 



A ? on a Required check counts as F, and Preferred checks are reported but don’t change the verdict.



I made One-bounded-and-specific-change Required because an issue with no clear finish line is not an advisable pick however good the rest looks. 



If that rejects too many issues in your eval, move it back to Preferred.

