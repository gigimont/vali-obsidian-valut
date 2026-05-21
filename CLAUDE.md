# CLAUDE.md — SME Succession Vault

## Project
Giuseppe + Wolf building an AI-powered "digital due diligence" service for SME knowledge transfer. Pre-product, fieldwork phase. Target: family-owned SMEs Germany/Italy, €2-20M revenue. The customer is the successor, not the founder. Obsidian vault tracks all research, strategy, and operations.

## Folder Structure
00-Home/              → Home.md dashboard (entry point)
00-Raw/               → Immutable raw transcripts and source documents. READ ONLY — never modify.
01-Strategy/          → Thesis, ICP, business model, product, competitors
02-Research/          → All interviews (001-011+), patterns, interview guide
  Market Intelligence/ → Desk research on second brain landscape, competitors, tech trends. Prefix: "MI —"
03-Outreach/          → Email templates, outreach strategy
04-Deliverables/      → Pitch deck, one-pager, council report
05-Open-Questions/    → Open Questions.md (living document)
06 - 1 to 1s/         → Weekly mentor check-ins (filename: 1 to 1s — Week N.md)
07-Daily-Standup/     → Daily co-founder standups (filename: Standup — YYYY-MM-DD.md)
99-Audit/             → Vault audit reports
Templates/            → Meeting Notes Template.md, Daily Standup Template.md

## Key Conventions
- Wikilinks: always `[[Note Name]]` without folder prefix
- Competitors file: `[[Competitors]]` in 02-Research/ (NOT "Competitive Landscape")
- ICP Definition: `01-Strategy/ICP Definition.md` — v1 created May 2026, covers Interviews 001–011. Needs v2 update.
- Tags: #strategy #research #interview #pattern #standup #check-in #to-validate #confirmed
- Interview files: `Interview NNN — Name.md` in 02-Research/
- Check-in files: `1 to 1s — Week N.md` in 06 - 1 to 1s/
- Every note must have a `## Related` section with wikilinks
- Raw sources: stored in 00-Raw/, immutable, never modified by Claude Code
- Market Intelligence: stored in 02-Research/Market Intelligence/, prefixed "MI —"
- Vault operations: ingest, audit, query — see "Vault Operations" section below
- **Raw file hub link.** Every new file created in 00-Raw/ (except RAW FILES.md and README.md) must include `[[RAW FILES]]` on its last line. This keeps all raw sources clustered in the graph view.
- **No phantom links or empty files.** Never create a wikilink  to a file that does not exist in the vault. Never create an empty or placeholder .md file just to satisfy a link. If a note references a concept that doesn't have its own page yet, mention it in plain text without double brackets. Only use wikilinks when the target file already exists or is being created in the same commit. Before committing, verify that every wikilink in every new or modified file points to an actual existing file. If unsure, use plain text instead of a wikilink.

## Living Documents (update after every interview)
- `02-Research/Patterns From Fieldwork.md` — patterns 1-42 (with documented gaps at 9, 10, 11, 36), add new ones here
- `05-Open-Questions/Open Questions.md` — cross off answered, add new
- `00-Home/Home.md` — timeline table + navigation links
- `01-Strategy/Product Evolution Log.md` — update after any strategic pivot or major reframe

## After Adding a New Interview
1. Create `02-Research/Interview NNN — Name.md`
2. Append new patterns to Patterns From Fieldwork.md
3. Append new open questions to Open Questions.md
4. Add link + one-line description to Home.md under Research & Interviews
5. Add row to Home.md timeline table
6. Run: git add -A && git commit -m "Add Interview NNN" && git push

## Vault Operations

### Ingest (processing a new source)
When told to process a raw file from 00-Raw/:
1. Read the raw file
2. Identify type: interview transcript, standup, meeting notes, market intelligence
3. Create the structured note in the correct folder (02-Research/ for interviews, 07-Daily-Standup/ for standups, etc.)
4. Extract new patterns → append to Patterns From Fieldwork.md
5. Extract new open questions → append to Open Questions.md
6. Add link + one-line description to Home.md
7. Add timeline table row to Home.md
8. Chain to previous note (add to Related section of the preceding note in the series)
9. Commit and push
10. DO NOT modify the raw file in 00-Raw/

### Audit (vault health check)
When asked to audit:
1. Read every .md file in the vault
2. Produce a report at 99-Audit/Vault Audit — YYYY-MM-DD.md
3. Check: broken wikilinks, orphan pages, stale strategy docs, missing patterns, unchained standups
4. DO NOT modify any file except the audit report

### Query (answering questions about the vault)
When asked a question about the project, research, or strategy:
1. Read relevant files (use index in Home.md to find them)
2. Synthesise an answer with wikilinks to sources
3. If the answer is substantial enough to be reusable, suggest creating a new vault page for it
