# CLAUDE.md — SME Succession Vault

## Project
Giuseppe + Wolf building an AI-powered "digital due diligence" service for SME knowledge transfer. Pre-product, fieldwork phase. Target: family-owned SMEs Germany/Italy, €2-20M revenue. The customer is the successor, not the founder. Obsidian vault tracks all research, strategy, and operations.

## Folder Structure
00-Home/              → Home.md dashboard (entry point)
01-Strategy/          → Thesis, ICP, business model, product, competitors
02-Research/          → All interviews (001-011+), patterns, interview guide
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
- ICP Definition: planned file at 01-Strategy/ICP Definition.md — does not yet exist
- Tags: #strategy #research #interview #pattern #standup #check-in #to-validate #confirmed
- Interview files: `Interview NNN — Name.md` in 02-Research/
- Check-in files: `1 to 1s — Week N.md` in 06 - 1 to 1s/
- Every note must have a `## Related` section with wikilinks

## Living Documents (update after every interview)
- `02-Research/Patterns From Fieldwork.md` — patterns 1-27, add new ones here
- `05-Open-Questions/Open Questions.md` — cross off answered, add new
- `00-Home/Home.md` — timeline table + navigation links

## After Adding a New Interview
1. Create `02-Research/Interview NNN — Name.md`
2. Append new patterns to Patterns From Fieldwork.md
3. Append new open questions to Open Questions.md
4. Add link + one-line description to Home.md under Research & Interviews
5. Add row to Home.md timeline table
6. Run: git add -A && git commit -m "Add Interview NNN" && git push
