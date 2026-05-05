# Vault Audit — 2026-05-05

#audit #meta

> **Generated:** May 5, 2026 (second run — post-cleanup pass)
> **Method:** Full read of every .md file (38 files); Python wikilink analysis; cross-reference of all pattern and open-question references
> **Scope:** Read-only. Zero files modified.
> **Context:** A first audit was run earlier today (commit 472c694), "Updates based on the audit" were applied (commit 38e10ee), and this report audits the current state.

---

## 1. File Map

Columns: outgoing links | incoming links | ORPHAN flag if 0 incoming

### 00-Home

| File | Description | Out | In |
|---|---|---|---|
| `Home.md` | Dashboard with navigation links and project timeline | 33 | 0 — orphan (expected: entry point) |

### 01-Strategy

| File | Description | Out | In |
|---|---|---|---|
| `Business Model.md` | Four revenue model options (break-even+upsell, B2B2B broker, due-diligence premium, subscription) and three-phase GTM strategy | 11 | 6 |
| `Council Verdict.md` | LLM Council session summary: 5 advisors, verdicts, clashes, blind spots | 6 | 18 |
| `Four Sub-Problems.md` | Framework: succession as four distinct problems (matching, readiness, emotional, deal-structuring) | 4 | 18 |
| `Market Data.md` | Country-level succession statistics with sources: EU, Germany, Italy, Poland, Hungary, Romania | 4 | 5 |
| `Origin Story.md` | History from the 5H bootcamp at ESMT through the Vali Hub phase | 12 | 8 |
| `Problem Statement.md` | Current thesis v3, evolution (v1–v3), 3 key assumptions, 3 deal-breaker hypotheses | 6 | 32 |
| `Product Methodology.md` | Three-pillar extraction framework, Neutral Mirror philosophy, Organizational Report spec | 8 | 11 |
| `Upstream vs Downstream.md` | The timing question: serve founders at succession (65-75) vs 10-15 years earlier | 4 | 18 |

**Missing from 01-Strategy:**
- `ICP Definition.md` — MISSING. Called for explicitly in Interview 006 action items and Standup 2026-05-04. No file exists.

### 02-Research

| File | Description | Out | In |
|---|---|---|---|
| `Competitors.md` | Competitive landscape: Celonis, Clonable, process mining tools, Omnivisor; unresearched flag list | 13 | 16 |
| `Gemini Export — Bootcamp (5H).md` | Full archival Gemini conversation from the 5H bootcamp (3,534 lines / ~49K words) | 0 | 1 — near-orphan |
| `Interview 001 — Successor.md` | Successor in industrial SME: knowledge trap, growth ambitions blocked, customer shift to successor | 5 | 25 |
| `Interview 002 - Ex-Banker, BoD of Deutsche Bank, SMEs view.md` | Written feedback from Carl: problem validated, 6 enterprise competitor names, documentation-first recommendation | 12 | 10 |
| `Interview 003 - Merih (Finance Professor).md` | Finance professor: Clonable/decision replication introduced, KKR Frankfurt and Berkeley intro offered | 21 | 13 |
| `Interview 004 - Prisma Founder (Digital Agency, Romania).md` | Romanian agency founder (200+ SME clients): "digital due diligence" label, internal champion requirement, parallel delivery | 9 | 15 |
| `Interview 005 — Real Estate Agency (Italy).md` | Italian real estate owner: positive outlier with delegation structure, but decision-making still tacit | 13 | 10 |
| `Interview 006 - John Lynch (Lynka).md` | €40-50M Polish textile CEO: challenges 2-week timeline, ERP ceiling, Omnivisor as live competitor, implementation gap | 23 | 18 |
| `Interview 007 — Vetreria Rachello (Italy).md` | Glass manufacturer: catastrophic 2007 overnight succession lived; failed sale blocked by family emotion; Lisa's decision-confidence gap | 15 | 11 |
| `Interview 008 — Antonio Rizza (M&A).md` | M&A professional: 100-item checklist, documentation completeness maps to deal price, consulting-agreement bridge described | 15 | 11 |
| `Interview 009 — Colusso Hardware (Italy).md` | Hardware store owner: 80% succession failure rate estimate, advice-not-products shift, 65K-article knowledge asset | 14 | 7 |
| `Interview 010 — Newton Campos (Search Fund).md` | Search fund GP: direct challenge to retroactive decision replication; prospective vs retroactive divide | 11 | 6 |
| `Interview 011 — Dairy Chemicals Commercial (Italy).md` | Post-acquisition micro-business: "chiavi di lettura" reframe for judgment framework capture; self-preservation dynamic | 13 | 2 — low connectivity (newest) |
| `Interview Guide.md` | Mom Test methodology: 4 prep questions, 6 live trigger questions with triggers, post-interview protocol | 22 | 8 |
| `Patterns From Fieldwork.md` | Living document: 24 confirmed patterns (1–8, 12–27; **patterns 9–11 missing**), emerging hypotheses | 28 | 45 — most linked-to file in vault |

### 03-Outreach

| File | Description | Out | In |
|---|---|---|---|
| `Email Templates.md` | Three Italian outreach templates: commercialista, warm intro, cold founder | 2 | 6 |
| `Outreach Strategy.md` | Six channels ranked by effectiveness, with conversion math | 5 | 9 |

### 04-Deliverables

| File | Description | Out | In |
|---|---|---|---|
| `Council Report.md` | Pointer to HTML/PDF council report files; key output summary | 8 | 1 — near-orphan |
| `One-Pager — German (v3).md` | German translation of One-Pager content v3 | 4 | 2 |
| `One-Pager.md` | All content versions (v1–v3) plus design iteration history | 3 | 11 |
| `Pitch Deck Content.md` | 6-slide cohort deck, Q&A prep table, messaging principles | 6 | 4 |

### 05-Open-Questions

| File | Description | Out | In |
|---|---|---|---|
| `Open Questions.md` | Living document: 50+ open questions across 5 categories | 5 | 13 |

### 06 - 1 to 1s

| File | Description | Out | In |
|---|---|---|---|
| `1 to 1s — Week 3.md` | Mentor check-in: validation status, US competitor signal, ICP entry-point thinking | 9 | 9 |

### 07-Daily-Standup

| File | Description | Out | In |
|---|---|---|---|
| `Standup — 2026-05-04.md` | First standup: ICP sizing debate, M&A angle, knowledge mining framing, interview debriefs 005/007/008 | 10 | 2 |
| `Standup — 2026-05-05.md` | Second standup: role split, vault audit decision, product anchor description, ICP calibration | 13 | 0 — **ORPHAN** (missing from Home.md) |

### Root

| File | Description | Out | In |
|---|---|---|---|
| `CLAUDE.md` | Instructions for Claude Code: vault structure, conventions, how-to protocols | 2 | 0 — orphan (expected: config file) |

### Templates

| File | Description | Out | In |
|---|---|---|---|
| `1 to 1s — Week {{number}}.md` | Template for weekly mentor check-ins | 3 | 0 — orphan (expected: template) |
| `Daily Standup Template.md` | Template for daily standup notes | 0 | 1 |
| `Meeting Notes Template.md` | Template for interview and meeting notes | 4 | 0 — orphan (path-linked from Interview Guide, not wikilinked) |

---

## 2. Strategy Docs — Staleness Check

### `01-Strategy/Problem Statement.md`

**EXISTS.** Latest interview referenced in content: Interview 001 (v3 is "post-first-interview"). The document has not been updated in 10 subsequent interviews.

**Findings from later interviews not reflected:**
- **Interview 006 (John Lynch):** "within weeks" framing explicitly wrong — realistic timeline is 3–6 months; insight without implementation gets sidelined (pure documentation fails); ICP digitalization cutoff missing
- **Interview 007 (Vetreria Rachello):** value erosion is quantifiable (€550K → ~€0 in 3 years); "protect the value of what you built" may be a stronger pitch than "document processes"; family emotion as non-separable factor
- **Interview 008 (Antonio Rizza):** M&A buyer is a potentially stronger paying customer than the founder; documentation completeness directly determines deal price
- **Interview 010 (Newton Campos):** "but the data doesn't exist" objection not addressed in deal-breaker hypotheses; prospective vs retroactive distinction missing
- **Interview 011 (Dairy Chemicals):** "judgment framework capture" reframe not in thesis; self-preservation dynamic (founders resist documentation to maintain leverage) not identified as a risk

**Verdict: STALE** — v3 is 10 interviews out of date. Direction is correct but deal-breaker hypotheses, value proposition framing, and ICP bounds all need a v4.

---

### `01-Strategy/Council Verdict.md`

**EXISTS.** Functions as an archival record of a session — not expected to be updated. The "buyer side missing" blind spot it flagged has since been addressed by Interview 008.

**Verdict: CURRENT** (archival document, no update needed)

---

### `01-Strategy/Four Sub-Problems.md`

**EXISTS.** Latest interview referenced: Interview 001. "Current hypothesis" section still says "we are investigating Problem 2 — Readiness as the primary wedge."

**Findings not reflected:**
- Interview 007 proved Sub-Problem 3 (Emotional) is non-separable from Sub-Problem 2 — the failed sale and Lisa's fear are one conversation
- Interview 008 gave the first concrete buyer-side data on Sub-Problem 4 (Deal Structuring)
- Interview 011 shows all four sub-problems simultaneously present in a post-acquisition case

**Verdict: STALE** — framework is still sound but "current hypothesis" section needs updating

---

### `01-Strategy/Upstream vs Downstream.md`

**EXISTS.** Latest interview referenced: Interview 001.

**Findings not reflected:**
- Interview 006 (John Lynch) is the strongest "downstream is too late" data point: digitally mature, CFO hired, ERP in place, competitor already engaged — the product has no clean wedge here
- Interview 010 (Newton Campos) reinforced: prospective capture (upstream) is uncontroversial; retroactive extraction (downstream) faces the feasibility objection
- Interview 008: M&A-preparation timeline (3–5 years before sale) is a middle ground between upstream and downstream that doesn't fit the current binary framing

**Verdict: STALE** — Interview 006 alone is reason enough for an update; it's the most important data point for this document and it's missing

---

### `01-Strategy/Competitive Landscape.md`

**MISSING.** Interview 002 action items created an explicit task to build this file. The content exists in `02-Research/Competitors.md` but the file and wikilink target do not match. There are no broken links pointing to `[[Competitive Landscape]]` remaining (they were fixed in the post-audit updates), but the conceptual gap remains: Competitors.md lives in 02-Research, not 01-Strategy.

**Verdict: MISSING** — recommend either moving Competitors.md to 01-Strategy or creating a stub

---

### `01-Strategy/ICP Definition.md`

**MISSING.** No file exists. Interview 006 action items: *"Consider creating `01-Strategy/ICP Definition.md` — explicit 'who this is for' and 'who this is NOT for' criteria, with Lynka as the canonical 'too far along' example."* Also called for explicitly in Standup 2026-05-04 and referenced in both standups' open threads. The ICP is scattered across Problem Statement, multiple interview notes, and standup discussions with no single authoritative document.

**Verdict: NEEDS CREATION** — this is the most critical missing document after Problem Statement v4

---

### `01-Strategy/Business Model.md`

**EXISTS.** Latest interview referenced: Interview 004 (Prisma, pricing signal).

**Findings not reflected:**
- Interview 006 (John Lynch): pricing reality check — "fairly humble amounts of money in the beginning" with a 3-month proof window; success-fee model tried and failed (cost savings consultants found €500K savings at Lynka, never adopted)
- Interview 008 (Antonio Rizza): sell-side advisory revenue model (retainer €20K–€100K+ plus 2–3% success fee) validated as a distinct track

**Verdict: STALE** — pricing section needs updating

---

### `01-Strategy/Product Methodology.md`

**EXISTS.** Status says "Working definition — not finalized." Latest referenced finding: Interview 003 (decision replication/Clonable).

**Findings not reflected:**
- Interview 006 (John Lynch): "insight without implementation gets sidelined" — pure blueprint deliverable fails; an implementation mechanism is required
- Interview 010 (Newton Campos): prospective vs retroactive distinction — methodology should explicitly differentiate
- Interview 011 (Dairy Chemicals): "judgment framework capture" is a better framing than "decision replication" for the Conversational Extraction pillar

**Verdict: STALE** — the Neutral Mirror philosophy and three pillars are still sound, but the deliverable spec and the decision-replication framing need revision

---

## 3. Patterns & Open Questions Sync Check

### Patterns From Fieldwork

Total patterns in file: **24** (numbered 1–8, then 12–27 — **patterns 9, 10, 11 are absent**).

**Pattern gap analysis:**

| Expected | In file | Referenced in interviews | Note |
|---|---|---|---|
| Pattern 9 | ❌ Missing | Interview Guide line 127 references "Pattern 9 — the neutral mirror" | Numbering conflict: this appears as Pattern 8 in the Patterns file |
| Pattern 10 | ❌ Missing | Interview 005 line 105 and Interview 009 line 98 reference "Pattern 10 — The gestionale/ERP ceiling" | Content added later as Pattern 22 (from Interview 006), creating a duplicate |
| Pattern 11 | ❌ Missing | Interview 009 line 99 references "Pattern 11 — 'Under-advised' as the felt problem" | Content added later as Pattern 25 (from Interview 006), creating a duplicate |

**Root cause:** Interview 004 proposed patterns labeled "7, 8, 9" in its text, but they were filed as "6, 7, 8" in the Patterns doc (one number off). Interview 005 then referenced the next expected number (10) for a new pattern (ERP ceiling) which was never added. Interview 009 referenced Pattern 10 and coined Pattern 11 — also never added. When Interview 006 arrived later, the ERP ceiling and under-advised concepts were re-added with new numbers (22 and 25). Result: cross-references in Interviews 005 and 009 point to non-existent pattern numbers.

**Pattern sources verified:**
All 24 existing patterns have source interviews listed; all those source interview files exist. No pattern references a missing file.

**Patterns mentioned in interview notes but NOT in the Patterns file by their cited number:**
- Pattern 9 (neutral mirror) — text exists as Pattern 8
- Pattern 10 (ERP ceiling) — text exists as Pattern 22
- Pattern 11 (under-advised) — text exists as Pattern 25

---

### Open Questions

**Total open questions:** ~50 across 5 categories (Customer & Buyer, Knowledge Extraction, Market & Economics, Strategic, Team & Execution).

**Answered questions section:** Empty. The doc says "Move questions here once fieldwork answers them" — none have been moved.

**Questions from later interviews NOT yet added:**

From **Interview 011 (Dairy Chemicals)**, three questions were listed in that note but are absent from Open Questions:
- "Is 'judgment framework capture' a better product name than 'decision replication' or 'knowledge management'?"
- "How do we handle the 'self-preservation' objection — founders who resist documentation because it reduces their leverage in a sale?"
- "Can our product address both knowledge AND cultural transition, or only knowledge?"

All questions from Interviews 007, 008, 009, 010 appear to have been added correctly.

---

## 4. Broken Wikilinks

The first audit (commit 472c694) found numerous broken links; the "Updates based on the audit" commit (38e10ee) fixed most of them. **Current state:**

### Confirmed still-broken (verified by grep):

**None found in source files.** All specific broken links identified in the first audit (`[[Interview 003 — Mary]]`, `[[Competitive Landscape]]`, `[[Feedback 001 — Carl]]`, `[[Interview 004 — John Lynch (Linka)]]`, `[[Interview 005 - John Lynch (Lynka)]]`) have been fixed.

### Path-syntax links (work in Obsidian but non-standard):

| Source | Link | Issue |
|---|---|---|
| `Interview 005 — Real Estate Agency` | `[[05-Open-Questions/Open Questions]]` | Path-prefixed; standard is `[[Open Questions]]` |
| `Interview Guide` | `[[Templates/Meeting Notes Template]]` | Path-prefixed; standard is `[[Meeting Notes Template]]` |

### Structural gaps (not broken links, but related):

- `[[Standup — 2026-05-05]]` is NOT linked from `Home.md` — the file exists but has 0 incoming links
- `[[ICP Definition]]` — no file exists; no links point to it yet (because no one has tried to link to it)
- Pattern numbers 9, 10, 11 in Interview 005, Interview 009, and Interview Guide are phantom references that won't navigate anywhere meaningful (see Section 3)

---

## 5. Home.md Assessment

### What's linked correctly ✅
- All strategy docs (Problem Statement, Council Verdict, Four Sub-Problems, Upstream vs Downstream, Market Data, Business Model, Product Methodology, Origin Story)
- Interviews 001, 004, 005, 007, 008, 009, 010, 011
- Interview Guide, Patterns From Fieldwork
- Outreach Strategy, Email Templates, One-Pager
- Pitch Deck Content, One-Pager German, Council Report
- Standup 2026-05-04, Daily Standup Template
- Open Questions
- Vault Audit 2026-05-05
- 1 to 1s — Week 3

### Still missing from Home.md ❌
1. **`[[Standup — 2026-05-05]]`** — not linked anywhere; 0 incoming links
2. **Interview 002 (Carl)** — listed in navigation but **description is blank** ("—"); should have at least a one-line summary
3. **Interview 003 (Merih)** — listed but **description is blank** ("—")
4. **Interview 006 (John Lynch)** — listed but **description is blank** ("—"); most analytically significant interview missing its summary
5. **`[[Competitors]]`** — never linked from Home navigation (though linked from many other files)

### Timeline errors still present ❌
- Row: `| 5 | Interview 006: Vetreria Rachello — strongest validation, 4 new patterns | ✅ Done |` — **wrong interview number.** Vetreria Rachello is Interview **007**, not 006. This was in the first audit's findings and has not been corrected.

### Timeline missing entries
- No row for Interview 006 (John Lynch) despite it being one of the most analytically important interviews

### Sections referencing non-existent content
None. All linked files exist.

---

## 6. CLAUDE.md Assessment

### Does the folder structure match disk? 
**Mostly yes, with one error:**
- CLAUDE.md documents folder `01-Strategy/` — file exists ✅
- CLAUDE.md documents `02-Research/` — exists ✅  
- All folders listed exist ✅
- **Missing:** `99-Audit/` folder is not mentioned anywhere in CLAUDE.md

### Are the conventions still accurate?
**Mostly yes, with two inconsistencies:**
1. CLAUDE.md says check-ins follow convention `1-1 — Week [N].md` — but the actual file is `1 to 1s — Week 3.md` (different separator style). Template file is also `1 to 1s — Week {{number}}.md`. **Naming convention in CLAUDE.md doesn't match actual files.**
2. CLAUDE.md lists "Competitive Landscape" as a key note at `01-Strategy/Competitive Landscape.md` — **this file doesn't exist.** The actual file is `02-Research/Competitors.md`.

### Interview index in CLAUDE.md: severely outdated
The interview table in CLAUDE.md only goes to Interview 007 and says "Next interview: `Interview 008 —`." We are now at Interview 012 next. This table requires manual updates after every interview and is consistently out of date. The information is redundant (Home.md has the same table, updated more reliably). Recommend removing the table from CLAUDE.md entirely and pointing Claude Code to read `00-Home/Home.md` or list `02-Research/` instead.

### What's unnecessary in CLAUDE.md
- Interview index table (lines ~60-80): outdated, duplicates Home.md, adds maintenance burden
- The "How to Add" sections are currently 4 detailed how-to blocks — could be 4 bullet points without losing operational value for Claude Code

### What's missing that Claude Code needs
- Mention of `99-Audit/` folder
- Clarification that `[[Competitors]]` (not `[[Competitive Landscape]]`) is the correct wikilink for the competitor file
- Note about the naming inconsistency between check-in filenames in templates vs convention
- Note that ICP Definition is a planned-but-not-yet-created file

---

## 7. Graph Structure Analysis

### Link flows by folder (approximate, based on content reading and link counts)

| From | To | Volume | Notes |
|---|---|---|---|
| `02-Research` | `01-Strategy` | Very heavy (≈140+ links) | Every interview links back to Problem Statement, Four Sub-Problems, Upstream vs Downstream, Council Verdict, Competitors, Business Model, Product Methodology |
| `02-Research` | `02-Research` (intra) | Heavy (≈60+ links) | Interviews cross-reference each other and Patterns From Fieldwork |
| `02-Research` | `05-Open-Questions` | Moderate (≈25 links) | Each interview adds questions |
| `01-Strategy` | `02-Research` | Moderate (≈20 links) | Strategy docs cite specific interviews |
| `02-Research` | `04-Deliverables` | Light (≈15 links) | Interviews reference One-Pager and Pitch Deck |
| `01-Strategy` | `01-Strategy` (intra) | Light (≈15 links) | Core strategy docs cite each other |
| `07-Daily-Standup` | `02-Research` | Light (≈10 links) | Standups debrief interviews |
| `01-Strategy` | `03-Outreach` | Very light (≈5 links) | Business Model references Outreach Strategy |
| `04-Deliverables` | `01-Strategy` | Very light (≈5 links) | Pitch Deck references Problem Statement, Council Verdict |

### CLUSTERS (groups of heavily interconnected notes)

**Cluster A — Core Thesis** (tightly interconnected):
`Problem Statement` ↔ `Four Sub-Problems` ↔ `Upstream vs Downstream` ↔ `Council Verdict` ↔ `Interview 001 — Successor`
- Every node in this cluster links to every other node; forms the conceptual backbone

**Cluster B — Research Accumulation** (interview-to-synthesis flow):
`Interviews 001–011` → `Patterns From Fieldwork` ← `Interview Guide` ← `Open Questions`
- Interviews flow INTO Patterns and Open Questions; Interview Guide sits between research and methodology

**Cluster C — Delivery** (loosely connected output layer):
`One-Pager` ↔ `Email Templates` ↔ `Outreach Strategy` ↔ `Pitch Deck Content`
- Minimal internal links; connects to research and strategy but weakly

**Cluster D — Project History** (archival, weakly connected):
`Origin Story` ↔ `Market Data` ↔ `Gemini Export` → `Council Report`
- Origin Story is the hub; Gemini Export is nearly isolated (1 incoming link)

### BRIDGES (notes connecting otherwise separate clusters)

1. **`Problem Statement`** (32 incoming): bridges Cluster A → Cluster B → Cluster C. The single most-linked file; almost every note connects to it.
2. **`Patterns From Fieldwork`** (45 incoming): THE most cited file in the vault; bridges Cluster B → Cluster A; is the primary accumulation point for all interview insights
3. **`Competitors`** (16 incoming): bridges Cluster B (research) → Cluster A (strategy); unique in that it straddles 02-Research and 01-Strategy conceptually
4. **`One-Pager`** (11 incoming): bridges Cluster A/B (strategy/research) → Cluster C (delivery)
5. **`Business Model`** (6 incoming, 11 out): bridges Cluster A → Cluster D → Cluster C

### ISLANDS (disconnected notes or groups)

1. **`Standup — 2026-05-05`** (0 incoming): exists, fully written, not linked from anywhere — invisible in Obsidian graph
2. **`Gemini Export — Bootcamp (5H)`** (1 incoming, 0 outgoing): massive archival file (49K words), only linked by Origin Story. No outgoing links.
3. **`Council Report`** (1 incoming): pointer file to HTML/PDF outputs; only linked by Council Verdict
4. **`Interview 011`** (2 incoming): newest interview, not yet integrated into the broader cross-reference network
5. **`One-Pager — German (v3)`** (2 incoming): only linked from One-Pager and Home

---

## 8. Recommended Actions

### CRITICAL

1. **Update `Problem Statement.md` to v4**: incorporate Newton's feasibility objection as Deal-Breaker Hypothesis 4 (prospective vs retroactive); add "judgment framework capture" as the refined thesis framing; add self-preservation dynamic; update ICP bounds to 20–100 employees / €10–25M EV (Newton's anchor); add the documentation→price quantification from Antonio; replace "within weeks" with 3–6 month timeline.

2. **Create `01-Strategy/ICP Definition.md`**: define exactly who this is for (20–100 employees, €2–20M revenue, founder 55–70, Italy or Germany, successor present OR sale horizon of 3–5 years) and who it is NOT for (digitally mature companies at Lynka's level; solo entrepreneurs at Interview 011's scale; founders pre-any-digital-footprint).

3. **Update `Upstream vs Downstream.md`**: add Interview 006 (John Lynch) as the definitive downstream-is-too-late data point; add Newton's prospective vs retroactive framing; acknowledge the M&A preparation timeline as a middle-ground scenario not covered by the current binary.

4. **Fix `Patterns From Fieldwork.md` — add the missing patterns 9, 10, 11**: Pattern 9 is a numbering artifact (neutral mirror exists as #8); Pattern 10 (gestionale/ERP ceiling) is a duplicate of Pattern 22 — resolve by either renumbering or adding a note that Pattern 10 = Pattern 22; same for Pattern 11 = Pattern 25. Alternatively, update Interviews 005, 009, and Interview Guide to use the correct current pattern numbers (22 and 25).

5. **Fix `Home.md` timeline**: change "Interview 006: Vetreria Rachello" to "Interview 007: Vetreria Rachello" — this is a factual error that has persisted through both audit-and-cleanup cycles.

### IMPORTANT

6. **Add `[[Standup — 2026-05-05]]` to Home.md** Daily Standups section — it currently has 0 incoming links and is invisible in Obsidian.

7. **Add descriptions to blank navigation entries in Home.md**: Interview 002 ("—"), Interview 003 ("—"), Interview 006 ("—") all have empty descriptions. Even a 5-word summary would make navigation useful.

8. **Add three open questions from Interview 011 to Open Questions.md**: judgment framework capture framing question; self-preservation objection question; knowledge vs cultural transition question.

9. **Update `Product Methodology.md`**: add "implementation mechanism required" finding from Interview 006 (insight without implementation gets sidelined); update Conversational Extraction section to use "judgment framework capture" framing from Interview 011; add prospective vs retroactive distinction from Interview 010.

10. **Update `Business Model.md`**: add Interview 006's pricing reality check ("humble amounts with a 3-month proof window"); note that success-fee models have been tried and failed in this market (Lynka's cost-savings consultants); add Antonio's sell-side advisory revenue track (retainer + 2–3% success fee).

11. **Update `CLAUDE.md`**: remove the interview index table (stale, duplicates Home.md); fix check-in naming convention to match actual files (`1 to 1s — Week N.md`); fix Competitive Landscape reference to point to `02-Research/Competitors.md`; add `99-Audit/` to folder list; add clarifying note about the correct wikilink name for competitors.

12. **Move `Competitors.md` to `01-Strategy/` or create a redirect stub `01-Strategy/Competitive Landscape.md`**: the file conceptually belongs in strategy and the original action item from Interview 002 placed it there. Currently it lives in 02-Research.

### GRAPH

13. **Link `[[Gemini Export — Bootcamp (5H)]]` from Home.md** under History/Context — currently has 1 incoming link from Origin Story only; a 49K-word primary source should be findable from the dashboard.

14. **Add a description to the `[[Origin Story]]` link in Home.md** — it's in the navigation already but listed under "Strategy & Thesis" without a description; the origin story is the strongest credibility asset for the pitch.

15. **Add at least one link from later interview notes back to `[[Market Data]]`** — the market statistics (80% succession failure, 560K German SMEs, etc.) are confirmed and amplified by fieldwork but Market Data only has 5 incoming links, all from strategy docs, not from the interviews that validate the numbers.

16. **Create a `[[Standup — 2026-05-05]]` link in Standup 2026-05-04's Related section** (and vice versa for previous standup) so the standup log is a navigable chain.

---

## 9. Compact Vault Summary

**What this vault is:** A knowledge base for a two-person incubation project (Giuseppe + Wolf, ESMT Vali Hub) building an AI-powered "digital due diligence" service to extract and document tacit knowledge from SME founders. Pre-product, fieldwork phase. Target: family-owned SMEs in Germany and Italy, €2–20M revenue, aging founders.

**Core thesis:** Organically grown SMEs run on expertise that lives in people's heads. As founders retire faster than they can be replaced, this creates a knowledge gap that AI now makes tractable to address. The primary customer is the **successor** (not the founder), who inherits an undocumented business and needs it systemized to grow or sell it.

**What's been done:** 11 interviews completed — successors (1), SME owners (4: real estate, glass manufacturing, hardware, dairy chemicals), expert advisors (3: ex-banker, finance professor, Prisma founder), buyer-side (2: M&A professional, search fund GP), and one large company owner (Lynka). The research is strong and well-documented.

**Key findings from fieldwork (not yet in strategy docs):**
- The product must include an **implementation mechanism**, not just a diagnostic blueprint — consultants who deliver only insight get sidelined (Interview 006)
- **Value erosion is quantifiable**: €550K offer in 2024, projected €0 in 3 years without a succession plan (Interview 007)
- **Documentation completeness maps linearly to deal price**: M&A buyers use ~100-item checklists; 20% documented = no offer, 100% = premium price (Interview 008)
- Newton's **feasibility objection** must be addressed: retroactive capture of 20–30 years of unrecorded decisions is only partial (~60–70%); prospective capture is uncontroversial (Interview 010)
- **"Judgment framework capture"** — not decision cloning, not process documentation — is the most defensible product framing: transfer the interpretive keys, not the decisions themselves (Interview 011)
- **ICP calibration**: Italian micro-businesses (€1–2M, 4–18 employees) validate the thesis but are too small as paying customers; Lynka (€40–50M, 250 employees) is too far along digitally; Newton's search fund range (20–100 employees, €10–25M EV) is the empirically grounded sweet spot

**Current vault state:**
- **Living documents** (Patterns From Fieldwork, Open Questions) are well-maintained ✅
- **Strategy docs** (Problem Statement, Four Sub-Problems, Upstream vs Downstream, Business Model, Product Methodology) are 7–10 interviews out of date ❌
- **Delivery docs** (Pitch Deck, One-Pager) still describe an Interview 001-era thesis ❌
- **One missing file** (ICP Definition) and **one naming mismatch** (Competitive Landscape vs Competitors) are the main structural gaps
- **Patterns 9, 10, 11** are referenced in interview notes but absent from the Patterns file — phantom numbering that breaks internal navigation
- **Standup 2026-05-05** has no incoming links (invisible in graph)

**Most urgent cleanup:** Write Problem Statement v4 and create ICP Definition.md. Both are blockers for sharpening any investor or partner conversation. Then fix the Patterns numbering and the Home.md timeline error (Vetreria Rachello is Interview 007, not 006).
