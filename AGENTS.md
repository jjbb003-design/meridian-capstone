# Meridian wiki instructions

## Purpose and scope

Maintain a research wiki for Joseph Barragan's Meridian Markets capstone. Meridian is fictional. Use the public class brief as the authority for client facts; never substitute a real business with the same name. Read `wiki/index.md` before answering questions.

## Data boundaries

- Allowed for AI under the brief: sales totals by store and week; store attributes.
- Prohibited in any AI: customer records, loyalty membership or purchase history, employee data, labor schedules, and excerpts. Removing names does not make prohibited records allowed.
- For mixed files, keep the original out of AI. Request an allowlisted extract produced by an authorized person or approved non-AI process and inspected for hidden sheets, comments, and prohibited columns. Ask the client about unspecified categories.
- AI permission does not authorize public release. This public repo may contain the published fictional brief and public research only. Do not put real client extracts in it.
- `.gitignore` is only an accident-prevention aid; it cannot protect data already committed or authorize ingestion.

## Organization and provenance

`raw/` holds the preserved brief and clearly labeled source notes; `wiki/` holds derived pages. Specs and plans belong in `docs/superpowers/`. Keep reading-note drafts and submission preparation in `submission/`; keep the tutorial dashboard in a separate repo.

For each source, record its title, author/publisher, original URL, publication date when verified, access date, scope, and retrieval limitations. Do not claim a summary is a full article. Keep excerpts short and cite the original. Preserve source notes after ingestion; append correction notes or save a new version rather than silently rewriting provenance.

## Ingest

1. Screen data against the boundaries before reading it with AI.
2. Open and inspect the original. Stop on a paywall, error, or incomplete retrieval; do not invent missing content.
3. Save provenance and concise source notes in `raw/`.
4. Create a source page with direct original-source citations, precise dates and units, and limitations.
5. Update relevant synthesis/client/question pages without presenting inference as fact.
6. Update `wiki/index.md` and append an actual dated action to `wiki/log.md`.
7. Check a consequential claim against the original, including number, period, geography, and whether it describes actual results or a forecast.

## Answer

Read index and relevant pages, then consult the original for substantive claims. Cite each factual claim directly to its original source and link the local source notes. Identify inference, speculation, and unknowns. Industry trends cannot establish Pasadena's suitability. File useful answers in `wiki/synthesis/`, preserving citations; update index and log.

## Check and maintain

Check relative links, orphan pages, missing citations, inconsistent units, stale dates, and contradictory claims. Keep source disagreements visible. Distinguish visits from revenue, publication year from measurement year, and announced stores from opened stores. Record who performed each check; never invent Joseph's review, reading completion, approval, or decision. Log corrections and unresolved limitations.
