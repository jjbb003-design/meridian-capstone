# Meridian Research Wiki Implementation Plan

> **For agentic workers:** Use superpowers:executing-plans to implement this plan task-by-task, inline as requested by the course. Steps use checkbox syntax for tracking. Do not delegate.

**Goal:** Build a traceable research wiki for Joseph Barragan's October 16 Meridian stakeholder interview.

**Architecture:** Plain Markdown separates preserved source material from cited wiki pages. An index provides navigation and an append-only log records changes. The initial build uses only the client brief; public research follows afterward.

**Tech Stack:** Markdown, Git, GitHub, PowerShell for file and link checks.

**Spec:** [Approved specification](../specs/2026-09-22-meridian-wiki-design.md).

**Status:** Joseph approved the saved plan in conversation ("the other thing is chill") after the explicit plan-review request. Inline execution began September 22, 2026.

## Global constraints

- Public repository name: `meridian-capstone`.
- The brief is fictional client context, not independent public research.
- Include the required ICSC article dated April 24, 2026 and two additional public sources from the course list.
- Customer records and employee data must never enter AI, including excerpts. Removing names does not change this rule.
- Permission for AI use is not permission for public GitHub publication.
- Label source notes as summaries when they are not complete copies. Preserve dates, units, geographic scope, and qualifications.
- Record Joseph's decisions only when he actually supplies them. Identify Codex checks separately.
- Keep the dashboard tutorial in its own repository.

## Review focus

1. Mixed confidential files: reject the original for AI ingestion; request an independently prepared allowed extract.
2. Pasadena confirmation bias: treat it as a proposed site, not an evidence-backed conclusion.
3. Numerical ambiguity: distinguish store openings, visits, revenue, and forecasts; preserve measurement year.
4. Unavailable sources: do not summarize an error page or claim to have read inaccessible content.
5. Broken navigation: verify every relative Markdown link and every wiki page's index entry.

## Initial wiki build

### Task 1: Project instructions and navigation

**Files:** Create `AGENTS.md`, `README.md`, `.gitignore`, `wiki/index.md`, and `wiki/log.md`.

**Consumes:** Approved spec and preserved `raw/client-brief.md`.

**Produces:** Source-handling rules, ingest/query/maintenance procedures, a wiki entry point, and dated change history.

- [x] Write AGENTS.md with explicit allowed/prohibited data examples, provenance fields, direct citations, inference labels, and index/log update rules.
- [x] Write README with project purpose, fictional-client label, links to the brief, index, spec, and plan; accurately state publication status.
- [x] Add `.gitignore` exclusions for `.env`, virtual environments, caches, and a `private/` folder. Explain that ignore rules do not remove previously committed files or authorize confidential ingestion.
- [x] Create index and log, linking only files that exist at this stage.
- [x] Check the instructions against two scenarios: a loyalty CSV remains prohibited after names are removed; store-week sales totals may be AI-permitted but not automatically public. Record the actual finding below.
- [x] Show changed files for review, then commit when Git identity is available.

**Done:** Instructions implement all four workflows and both data scenarios correctly; navigation opens real files.

### Task 2: Client brief page

**Files:** Create `wiki/client/meridian-markets.md`; update `wiki/index.md` and `wiki/log.md`.

**Consumes:** `raw/client-brief.md` and Task 1 instructions.

**Produces:** Cited client profile, decision context, assumptions, constraints, and unanswered questions.

- [x] Compare the saved brief with the assigned original and record whether the contents match.
- [x] Summarize the 14-store footprint, business model, dashboard request, uneven growth, and proposed Pasadena expansion, citing the original brief.
- [x] Explain that revenue, costs, and customer experience are distinct goals with no agreed priority or metric definitions yet.
- [x] Flag POS migration comparability, the board preview versus eight-week engagement, and data permissions for clarification.
- [x] Check every client fact against the brief. Ensure Pasadena is labeled a stakeholder preference rather than a validated recommendation.
- [x] Update index/log, show changed files, and commit when identity is available.

**Done:** Every client fact is supported, assumptions are explicit, and the page adds no invented store performance.

### Task 3: Initial wiki acceptance check

**Files:** Review all Task 1–2 files; update this plan and `wiki/log.md`.

- [x] Read AGENTS.md, index, log, and client page against the spec.
- [x] Check all relative Markdown link targets exist and every wiki page is linked from the index.
- [x] Inspect repository contents for accidental secrets, private client data, and unsupported claims.
- [x] Record real findings and corrections; mark the initial build complete only when checks pass.
- [x] Show the initial wiki for review before starting public-source ingestion.

**Done:** A usable, checked wiki based solely on the brief. Specific public-source ingestion is not part of these initial build tasks.

## Subsequent workshop activities — after initial build

These record later workshop work in the same plan, not additional initial-build tasks.

- [x] Ingest the assigned ICSC article into `raw/icsc-grocery-formats-2026.md` and `wiki/sources/icsc-grocery-formats-2026.md`. Preserve title, date, original URL, and limited supporting excerpts. Update index/log.
- [x] Check one ICSC claim against the original article, preserving whether a location is open or under development. Record the check and decision below.
- [x] Ingest JLL's Grocery Report 2025 into corresponding raw/source pages, checking that 2024 openings are not mislabeled 2025 openings.
- [x] Select a third accessible source from the class list, based on expansion criteria. If retrieval fails, use another accessible listed source and record why.
- [x] Save `wiki/synthesis/expansion.md`, answering where specialty grocers are opening with direct citations and explicit inferences.
- [x] Save `wiki/interview/questions.md` with prioritized questions for Dana and a separate data-clarification list for Marcus. Include alternatives to Pasadena, success criteria, POS migration, and allowed extracts.
- [x] Update index/log and repeat link, citation, and confidentiality checks.
- [x] Record Joseph's overall acceptance of the reviewed work.
- [x] Record Joseph’s reported review, original-source check confirmation, and accepted reasons below. Agent checks remain identified separately.
- [x] Commit and push to Joseph's public `meridian-capstone` repository after account access is established.
- [x] Open the GitHub spec and plan and check their contents; verify anonymous repository access. Record actual URLs in the submission checklist.

## Review record

### Review 1 — Design and data boundaries

- **Request and result:** Joseph asked for assignment completion and approved the proposed wiki direction and linked spec. Codex produced the saved spec and this implementation plan.
- **Check performed by Codex:** Read the assigned brief's Terms of engagement and compared the spec's rules. The spec prohibits customer/employee records and distinguishes AI use from public publication.
- **Joseph’s reported review and finding:** Reported reviewing the work and accepted the data-boundary explanation: restricted customer and employee information stays out of AI, while approved sales totals may be used.
- **Joseph’s decision and reason:** Accept without changes because the rules protect customer and employee information while allowing approved sales totals. Joseph explicitly endorsed this proposed wording in conversation. He also reports submitting the confidentiality paragraph.

### Review 2 — Original-source research claim

- **Request:** Summarize a public grocery source with citations and verify a numerical or location claim against the original.
- **Result:** Source pages and a cited synthesis were saved. A key JLL claim is that Sprouts opened 35 stores in 2024.
- **Check by Codex:** Opened JLL's original Grocery Report 2025 and read the Fastest-growing grocers in 2024 section. The number is supported; 2025 is publication year, not the opening year. Also checked ICSC: Redlands is described as under development, not already open.
- **Agent decision:** Accept the qualified claims and preserve their dates/status. 
- **Joseph’s reported check and decision:** When asked whether he verified the JLL claim himself, Joseph answered affirmatively. The claim under review was 35 Sprouts openings in 2024. He accepted the reviewed summary without changes after that confirmation. This records his reported check; Codex did not observe his browsing. No separate detailed account of his checking process was supplied.

### Review 3 — Cited answer and interview usefulness

- **Request:** Answer where specialty grocers are opening and identify a useful question for Dana.
- **Result:** Saved wiki/synthesis/expansion.md and wiki/interview/questions.md.
- **Check by Codex:** Followed the synthesis citations to ICSC and JLL. Their location examples are supported, but neither compares Meridian's Pasadena option with alternatives. All relative links resolve; all eight wiki pages appear in the index.
- **Agent decision:** Accept the examples as interview context; do not recommend Pasadena on this evidence. Proposed question: what would make Dana reject Pasadena? 
- **Joseph’s reported review, finding, and decision:** Reported reviewing the work and accepted the question without changes. He endorsed the reason that asking what would make Dana reject Pasadena helps test her preference instead of assuming it is the best location. This reason was proposed by Codex and explicitly adopted by Joseph.

## Plan self-review

Codex checked this plan against the approved spec: initial build remains separate from public ingestion; all required files have an owner; data boundaries, citation checks, navigation, and publication verification are covered. No dashboard code is included because it belongs in a separate project. Pending statuses describe work not yet performed, not claims of completion.

## Execution approval

Joseph approved the saved plan in conversation on September 22, 2026. Execution is inline. This records expressed approval, not an independent student source check.


## Execution evidence

Initial build complete: brief matched original; all relative links resolved; client facts and data scenarios checked by Codex. Local commit a62b016. Inline execution uses this plan as the work ledger, as the assignment requires. The approved course plan does not delegate or add automated tests for Markdown; direct source and link checks are the verification method.



Publishing check: pushed commit 661060e to public main. Anonymous HTTP retrieval of spec, plan, and wiki/index returned 200 and matched local contents. Browser navigation opened the plan URL; full signed-out browser-window check is still distinct from the successful anonymous HTTP check.


## Student completion update

On September 22, 2026, Joseph reported submitting the six links and confidentiality paragraph and sharing the Google Doc. He then said, “yea i reviewed all good do what oyu have to do to finish.” This records his overall review and acceptance without inventing specific source checks or reasons. Joseph subsequently confirmed the JLL check and explicitly adopted the data-boundary and interview-question reasons recorded above. Brightspace submission and the document recipient/access role are student-reported, not independently verified.
