# Technical Review: Measuring Transformation Change

## Pass: 2026-11-14

| Field | Value |
| :--- | :--- |
| Reviewer model | Gemini 3.1 Pro |
| Session | Fresh (yes) |
| Web / CLI verification | Available (Google Search) |
| Labs in scope | No lab files (group-activity course) |
| Lab tester reports | None |
| Scope | Slides (`course/00-introduction.md` through `course/04-evaluating-training-impact.md` and `course/images/*.svg`) |

### Corrections

| ID | Location | What was wrong | Change made | Source |
| :--- | :--- | :--- | :--- | :--- |
| T-1 | `course/01-defining-success.md` / The New AI Enablement Landscape | Wrote `Microsoft 365 Copilot chat` with lowercase `chat`, inconsistent with `course/03-designing-training.md` and official Microsoft product naming | Standardized to `Microsoft 365 Copilot Chat` to match `03-designing-training.md` and official naming | Microsoft Learn (`https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-chat-overview`), 2026-11-14 |
| T-2 | `course/02-measuring-change-management.md` / Three Tiers of AI Rollout Data | Listed `Claude or Gemini admin logs` as tracking active days, feature surfaces used, and cohort retention; in Claude Enterprise, standard admin audit logs only record security and workspace events (sign-ins, role updates, project/file actions) rather than active usage telemetry | Updated to `Claude analytics, and Gemini admin reports` to reflect the surfaces that report active usage and adoption | Anthropic Help Center (`https://support.anthropic.com`) and Google Workspace Admin Help (`https://support.google.com/a/answer/15239892`), 2026-11-14 |
| T-3 | `course/03-designing-training.md` / Role-Based Curriculum Matrix Across Functions | Listed `copilot-instructions.md` without the required `.github/` directory path alongside `CLAUDE.md`; GitHub Copilot requires repository-wide custom instructions at `.github/copilot-instructions.md` | Updated `copilot-instructions.md` to `.github/copilot-instructions.md` | GitHub Docs (`https://docs.github.com/en/copilot/customizing-copilot/adding-repository-custom-instructions-for-github-copilot`), 2026-11-14 |

### Verification log

| Location | Claim | Result | Source | Date |
| :--- | :--- | :--- | :--- | :--- |
| `course/01-defining-success.md` / The New AI Enablement Landscape | Product names: Claude, Gemini, Microsoft 365 Copilot Chat, GitHub Copilot, Claude Code | Corrected (`T-1`) | https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-chat-overview | 2026-11-14 |
| `course/01-defining-success.md` / Quiz 1 and Quiz 2 | Quiz 1 answer key (`B`) and Quiz 2 answer key (`C`) match slide facts and distractors are false | Confirmed | Internal cross-check against Chapter 1 slides | 2026-11-14 |
| `course/02-measuring-change-management.md` / Three Tiers of AI Rollout Data | Microsoft 365 Copilot Dashboard, GitHub Copilot metrics, Claude analytics, and Gemini admin reports track adoption and active usage | Corrected (`T-2`) | https://learn.microsoft.com/en-us/viva/insights/org-team-insights/copilot-dashboard ; https://docs.github.com/en/copilot/managing-copilot/managing-github-copilot-in-your-organization/reviewing-activity-related-to-github-copilot-in-your-organization ; https://support.google.com/a/answer/15239892 | 2026-11-14 |
| `course/02-measuring-change-management.md` / Example: A Plain-Language Measurement Charter | Cohort aggregation floor of 10+ employees aligns with standard enterprise privacy thresholds (default minimum group size in Microsoft Viva Insights Copilot Dashboard is 10 employees) | Confirmed | https://learn.microsoft.com/en-us/viva/insights/org-team-insights/copilot-dashboard | 2026-11-14 |
| `course/02-measuring-change-management.md` / Why Drafting Speed Alone Misleads | Cycle-time and rework figures (`6.0h + 2.0h = 8.0h` manual baseline; `1.5h + 6.0h = 7.5h` speed-only; `2.5h + 1.5h = 4.0h` balanced) match `images/ch02-cycle-time-rework-bars.svg` | Confirmed | Cross-check of `course/02-measuring-change-management.md` and `course/images/ch02-cycle-time-rework-bars.svg` | 2026-11-14 |
| `course/02-measuring-change-management.md` / Quiz 1, Quiz 2, and Quiz 3 | Quiz 1 answer key (`C`), Quiz 2 answer key (`B`), and Quiz 3 math (`500 * 4.2 = 2,100 hours/week`) are accurate | Confirmed | Internal cross-check against Chapter 2 slides | 2026-11-14 |
| `course/03-designing-training.md` / Training Solves Skill Gaps, Not Will or System Gaps | Prosci ADKAR model sequential milestones: Awareness, Desire, Knowledge, Ability, Reinforcement | Confirmed | https://www.prosci.com/methodology/adkar | 2026-11-14 |
| `course/03-designing-training.md` / Matching Enablement Design to AI Modality | Product names: Microsoft 365 Copilot in Office apps, Gemini in Google Workspace, GitHub Copilot, Claude Code | Confirmed | https://workspace.google.com/solutions/ai/ ; https://docs.anthropic.com/en/docs/claude-code/overview | 2026-11-14 |
| `course/03-designing-training.md` / Role-Based Curriculum Matrix Across Functions | Repository custom instructions filenames: `CLAUDE.md` for Claude Code and `.github/copilot-instructions.md` for GitHub Copilot | Corrected (`T-3`) | https://docs.anthropic.com/en/docs/claude-code/memory ; https://docs.github.com/en/copilot/customizing-copilot/adding-repository-custom-instructions-for-github-copilot | 2026-11-14 |
| `course/03-designing-training.md` / Quiz 1, Quiz 2, and Quiz 3 | Quiz 1 answer key (`B`), Quiz 2 answer key (`C`), and Quiz 3 labor math (`150 * 0.5h = 75 hours`) are accurate | Confirmed | Internal cross-check against Chapter 3 slides | 2026-11-14 |
| `course/04-evaluating-training-impact.md` / Adapting Kirkpatrick’s Four Levels for AI Enablement | Kirkpatrick Four Levels (Level 1: Reaction, Level 2: Learning, Level 3: Behavior, Level 4: Results) and backward design principle | Confirmed | https://www.kirkpatrickpartners.com/the-kirkpatrick-model/ | 2026-11-14 |
| `course/04-evaluating-training-impact.md` / Stopping at Level 4 vs. Calculating Monetary ROI & Defensible Renewal Math When Finance Asks for ROI | Jack Phillips Level 5 ROI methodology and formula (`($180k isolated benefit - $90k cost) / $90k cost * 100 = 100% ROI`) | Confirmed | https://roiinstitute.net/ | 2026-11-14 |
| `course/04-evaluating-training-impact.md` / Three Low-Lift Ways to Capture Level 3 Behavior | Robert Brinkerhoff's Success Case Method (SCM) comparing high-adopting success cases and stalled/non-adopting cases via structured interviews | Confirmed | Brinkerhoff, *The Success Case Method* (Berrett-Koehler, 2003) | 2026-11-14 |
| `course/04-evaluating-training-impact.md` / Building an End-to-End Impact Chain & Isolating Enablement Value from Tool Access Alone | Handle-time and cycle-time reductions (`4.2d -> 2.8d = -33%`, `48m -> 33m = -31%`, `48m -> 35m = -27%`) match `course/02-measuring-change-management.md` and `images/ch04-staggered-wave-attribution.svg` | Confirmed | Cross-check across Chapters 2 and 4 and SVG charts | 2026-11-14 |
| `course/04-evaluating-training-impact.md` / Quiz 1 and Quiz 2 | Quiz 1 answer key (`B`) and Quiz 2 answer key (`C`) match slide facts and distractors are false | Confirmed | Internal cross-check against Chapter 4 slides | 2026-11-14 |

### Left unchanged

- Teaching gaps, demos, Do Nows, and discussions stay with Instructor Review
- Spelling and typography stay with the Copy Editor
- Layout and new graphics stay with the Course Graphics Designer
- A choice between two valid approaches stays as written
- A volatile claim marked unverified stays as written
