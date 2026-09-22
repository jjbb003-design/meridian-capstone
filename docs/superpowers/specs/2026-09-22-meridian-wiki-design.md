# Meridian Markets research wiki — design specification

Date: September 22, 2026  
Status: Approved by Joseph Barragan in conversation on September 22, 2026.  
Method: Superpowers brainstorming instructions read from the upstream project. The plugin is not installed in this session.

## Purpose and intended result

Prepare for the October 16 stakeholder interview with Dana Okafor by making the fictional client brief and public grocery research easy to find, check, and turn into useful questions. The result is a small, linked Markdown wiki in a public `meridian-capstone` GitHub repository. It supports discovery; it does not determine the next store location or build Meridian's dashboard.

The user requested completion of the assignment while at work. The assignment requires personal review, decisions, and sequential approval of the saved spec and plan. Those actions remain explicitly pending until the student performs them.

## Design choices

Recommended: organize by client, sources, synthesis, and interview questions, with one central index. This fits a small collection and makes each statement traceable.

Alternatives considered by Codex: a single research document would be quicker but harder to maintain; a searchable application would introduce unnecessary setup. Plain Markdown is sufficient and renders directly on GitHub.

Research focus proposed by Codex: how format, local demand, and available real estate should shape expansion criteria, without treating Pasadena as a predetermined answer. Student may change this focus during review.

## Source policy

- Preserve the assigned public fictional brief at `raw/client-brief.md`. Original: https://github.com/LMU-MSBA/bsan-6088-fa26/blob/main/workshops/client-brief.md.
- Read and retain source title, author/publisher, publication date, original URL, retrieval date, and source scope for each public source.
- Include the required ICSC article dated April 24, 2026 and two additional public sources from the course list. Three meets the linked prompt sheet's higher count even though the pasted assignment says two.
- Save concise, clearly labeled source notes and limited excerpts when full redistribution is not authorized. Do not describe a summary as a complete source copy. Stop on inaccessible or incomplete content; never ingest an error page as evidence.
- Distinguish publication year from the year measured. Distinguish visits, revenue, store counts, and square footage. Preserve forecasts as forecasts.
- The brief is fictional client context, not independent public research. Do not search for a real company and attribute its facts to Meridian.

## Organization

```text
AGENTS.md                         Source, ingest, query, and maintenance rules
README.md                         Navigation and project status
raw/client-brief.md               Assigned brief, preserved
raw/<source>.md                   Public-source provenance and source notes
wiki/index.md                     Every wiki page linked with a short description
wiki/log.md                       Append-only record of ingests, queries, and checks
wiki/client/meridian-markets.md   Brief-based profile, needs, assumptions, unknowns
wiki/sources/<source>.md          Source-specific summary with original citations
wiki/synthesis/expansion.md       Cited answer about specialty-grocer expansion
wiki/interview/questions.md       Prioritized questions for Dana and Marcus
docs/superpowers/specs/           This specification
docs/superpowers/plans/           Implementation plan and review record
```

## Ingest, answer, and maintenance behavior

On ingest: screen the source for allowed content, inspect retrieval quality, save provenance, summarize supported facts, link relevant pages, update index, append log. Preserve raw notes once ingested; log corrections or replacement versions.

On a question: read the index, consult relevant pages and originals, cite each factual claim with a direct original-source link and link back to the corresponding source notes. Mark interpretation as inference. State when evidence cannot answer the question. Save useful answers with citations and update index and log.

On maintenance: check missing sources, broken relative links, orphan pages, contradictory numbers, stale facts, uncited claims, and unsupported recommendations. Keep meaningful source disagreements visible rather than silently reconciling them.

## Data boundaries

The brief permits sales totals by store and week and store attributes to be used with AI. It prohibits customer records and employee data in any AI tool, including loyalty information, labor schedules, and excerpts. Removing names is not permission to upload prohibited records.

For mixed files, do not upload the original or ask AI to redact it. Have an authorized person or approved non-AI process create a separate allowlisted extract, then inspect it before AI use. Exclude customer IDs, loyalty purchase history, employee identifiers, schedules, hidden sheets, comments, and other prohibited material. Obtain client clarification for categories not explicitly allowed, including transaction-level or category-level extracts.

Permission to use information with AI is not permission to publish it on GitHub. This public repository contains only the course's public fictional brief and public research. Keep future client extracts outside the public repo even if they are AI-permitted, unless public release is separately authorized.

## Initial build versus subsequent research

The implementation plan's initial tasks cover folders, AGENTS.md, README, index, log, and the page based on the brief. Specific public-source ingestion and the research query happen after the initial build, consistent with the course prompt sheet. Subsequent work and three review entries may be recorded in a distinct section of the same plan.

## Acceptance criteria

1. The saved brief matches the assigned original.
2. The client page accurately states the requested decision, competing goals, allowed data, and unknowns, without presenting Pasadena's suitability as established.
3. The public-source collection includes ICSC plus two usable sources, each with title and original URL.
4. Each factual synthesis claim is traceable to an original source; inferences and missing evidence are labeled.
5. The index reaches every wiki page; relative links resolve; the log records actual changes.
6. The plan contains completion statuses and three honest review entries: request/result, actual check/finding, and decision/reason. At least one checks a research claim against the original source. Codex checks and student checks are identified separately.
7. The spec and plan are reviewed in sequence by the student before build approval. No invented approval or retrospective claim of compliance.
8. Public GitHub accessibility and rendered spec/plan contents are verified after publishing, with URLs recorded.

## Agent's specification review

Checked against the assignment and prompt sheet: includes purpose, sources, organization, boundaries, and useful-result criteria; separates build tasks from later ingestion; uses three sources to resolve the source-count discrepancy. No private client data is available or needed. Publication and personal review are incomplete, not represented as done.

## Student review

Joseph approved the presented direction and linked specification, replying “yes that works bro” on September 22, 2026. He confirmed his name and that he has not started the assignment. This records his expressed approval; it does not claim he independently verified research sources. Plan review and build approval remain separate next steps.

## Workflow references

- [Course prompt sheet](https://github.com/LMU-MSBA/bsan-6088-fa26/blob/main/workshops/workshop-01-prompt-sheet.md)
- [Course source list](https://github.com/LMU-MSBA/bsan-6088-fa26/blob/main/workshops/workshop-01-sources.md)
- [LLM Wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- [Superpowers brainstorming instructions](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md)
