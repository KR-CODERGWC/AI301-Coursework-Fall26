# **Rubric: is this a good first issue?**

## Checks

| Check | Evidence | Pass condition | Weight |
|-|-|-|-|
| Not-claimed | Assignee, "I'm working on this" comments, linked PRs | No assignee, no recent claim, no open PR | required |
| Expected-actual-behavior | Lines describing what should happen and what does happen | Both can be quoted | preferred |
| Specific-change | Issue title, body and labels; the opener's role (MEMBER, COLLABORATOR, OWNER, CONTRIBUTOR, NONE); comment count and linked PRs | Check the Fail rules first. Fail if the issue: (a) is a tracking list or "megaissue" made of links to other issues; (b) asks for changes "across the codebase" or "incrementally"; (c) has 30+ comments of unresolved debate or abandoned PRs (claim comments and reproduction reports do not count toward the 30); (d) is a feature request that no maintainer has endorsed and that needs a product decision. Otherwise pass if the issue names the concrete thing to change (a command, UI element, behavior or doc page). A bug report (bug label) filed by a MEMBER, COLLABORATOR or OWNER passes even if it's short, says "several" or "etc.", or lists possible causes; treat "suggestions" as optional extras, not extra scope | required |
| Active-maintainer-engagement | "maintainer first-response sample" in Repo facts, plus maintainer comments on this issue | A maintainer replied within about 30 days in the sample, or a maintainer commented on the issue | preferred |
| Fits-time-available | Files or areas named, size words like "refactor" | Looks like 3 files or fewer, no breaking change | preferred |
| Technical-specs-requirements | Versions, OS, tools needed | Stated, and no special access needed | preferred |
| Active-release-cycle | Release or tag dates | A release in about the last 6 months | preferred |
| Maintainer-recent-commits | "last 5 default-branch commits" dates in the Repo facts block | The newest commit is within 90 days of the bundle's captured date, and the repo is not archived | required |
| Policy-allows-contribution | The "contribution policy" line in the Repo facts block | Pass if the policy is silent ("no statement on AI") or allows AI-assisted contributions, even with conditions like "you must review it." Fail if it bans AI-generated code or docs, or limits contributions to maintainers only | required |

## Verdict rule

Accept only if every required check is graded pass; a required check graded unclear counts as fail. Preferred checks are reported and used to rank accepted issues, but never change the verdict.
