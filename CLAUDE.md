# CLAUDE.md — SME Succession Obsidian Vault

## What This Is

This is an Obsidian knowledge base for an incubation project at the Vali Entrepreneurship Hub. The team (Giuseppe + Wolf) is building an AI-powered "digital due diligence" service to extract and document tacit knowledge from SME founders and senior employees.

**Stage:** Pre-product, fieldwork phase.

---

## Vault Structure

```
00-Home/              → Dashboard (Home.md)
01-Strategy/          → Thesis, council verdict, competitive landscape, strategic questions
02-Research/          → Interview notes, feedback notes, interview guides, patterns
03-Outreach/          → Outreach strategy, email templates
04-Deliverables/      → Pitch deck content, one-pager, council report
05-Open-Questions/    → Master checklist of what to validate
06 - 1 to 1s/         → Weekly mentor check-in notes
Templates/            → Reusable templates for meetings and check-ins
```

---

## Conventions

### File naming
- Interviews: `Interview 001 — [Name or Company].md`
- Feedback (written advisory): `Feedback 001 — [Name].md`
- Check-ins: `1-1 — Week [N].md`
- Strategy notes: plain descriptive name, e.g., `Problem Statement.md`

### Linking
- Always use `[[wikilinks]]` to connect notes
- Link to related notes at the bottom of every note under a `## Related` section
- Link inline when mentioning another concept (e.g., "see [[Four Sub-Problems]]")

### Tags
Core tags: `#strategy`, `#research`, `#interview`, `#feedback`, `#check-in`, `#weekly`, `#outreach`, `#deliverable`, `#pattern`, `#to-validate`, `#confirmed`, `#to-research`, `#core`, `#living-document`, `#mom-test`

Role tags: `#sme-owner`, `#expert`, `#academic`, `#agency`, `#banking`, `#successor`, `#founder`

### Frontmatter style
Use blockquote metadata at the top of each note (not YAML frontmatter):
```
> **Date:** April 2026
> **Interviewee:** Name — role
> **Sector:** ...
```

---

## Key Notes (update these frequently)

- `00-Home/Home.md` — Dashboard. Update the timeline table and navigation links when adding new notes.
- `02-Research/Patterns From Fieldwork.md` — Living document. Add new patterns after every interview.
- `05-Open-Questions/Open Questions.md` — Living document. Cross off answered questions, add new ones.
- `01-Strategy/Problem Statement.md` — Thesis with version history. Add new versions as thinking evolves.
- `01-Strategy/Competitive Landscape.md` — Competitor research. Update as new companies are discovered.

---

## How to Add a New Interview Note

1. Create file in `02-Research/` named `Interview [NNN] — [Name or Company].md`
2. Use the structure from existing interview notes (see Interview 001–004 for examples)
3. Include: Context, Key Quotes, What We Learned, Patterns confirmed/challenged, Action Items, Open Questions, Related links
4. After creating, update these notes:
   - `02-Research/Patterns From Fieldwork.md` — add or confirm patterns
   - `05-Open-Questions/Open Questions.md` — add new questions, check off answered ones
   - `00-Home/Home.md` — add link under Research & Interviews, update timeline

## How to Add a Feedback Note

Same as interview but file goes in `02-Research/` as `Feedback [NNN] — [Name].md`

## How to Add a Weekly Check-in

1. Create in `06 - 1 to 1s/` as `1-1 — Week [N].md`
2. Use template from `Templates/1-1 Template.md`
3. Update `00-Home/Home.md` timeline

---

## Important Context for AI Assistance

- **The customer is the successor, not the founder.** This is a core positioning choice.
- **"Digital due diligence"** is the current product label (from Interview 002).
- **"Decision replication"** (from Interview 003 / Clonable) is an emerging but uncommitted direction.
- **The Mom Test** guides all interview methodology — no leading questions, no loaded framing.
- The project targets **Germany and Italy**, family-owned SMEs, **€2–20M revenue**.
- **All text in the one-pager is verbatim from the team's approved docx** — do not rephrase it.
- When updating existing notes, **append** new content — never delete existing content unless explicitly asked.
