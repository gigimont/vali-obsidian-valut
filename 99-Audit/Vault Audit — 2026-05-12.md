# Vault Audit — 2026-05-12

#audit #meta

> **Generated:** May 12, 2026
> **Method:** Full read of every .md file (53 files); cross-reference of all pattern, open-question, and wikilink references
> **Scope:** Read-only. Zero files modified.
> **Context:** Second full audit. The prior audit (2026-05-05) covered 38 files. Since then: 15 new files added (Interviews 012–019, Standups May 06/09/11, 1 to 1s Week 4/5, ICP Definition.md, Vault Audit May 05). The May 05 audit's critical recommendations were partially implemented. This audit assesses the current state against 19 completed interviews.

---

## 1. Complete File Map

**Total: 53 .md files** (up from 38 in prior audit; 15 new)

### 00-Home (1)
| File | Description | Out | In |
|---|---|---|---|
| `Home.md` | Dashboard: navigation + project timeline | 45+ | 0 — orphan (expected: entry point) |

### 01-Strategy (9)
| File | Description | Status |
|---|---|---|
| `Business Model.md` | Four revenue models; three-phase GTM | Stale — post-Interview 004 |
| `Council Verdict.md` | LLM Council: verdicts, clashes, blind spots | Current — archival |
| `Four Sub-Problems.md` | Matching / readiness / emotional / deal-structuring | Stale — post-Interview 001 |
| `ICP Definition.md` | Who this is for / not for; triggers; evidence table | Partial — v1, post-Interviews 001–011 |
| `Market Data.md` | Country-level succession statistics | Current (unchanged) |
| `Origin Story.md` | History from 5H bootcamp through Vali Hub | Current (archival) |
| `Problem Statement.md` | Thesis v4, deal-breaker hypotheses, assumptions | Stale — v4 frozen post-Interviews 002–011 |
| `Product Methodology.md` | Neutral Mirror, three pillars, Organizational Report | Stale — pre-Pattern 28 |
| `Upstream vs Downstream.md` | Timing question; unresolved | Stale — post-Interview 001 |

**Note from prior audit implemented:** ICP Definition.md created ✅. Remaining: the file is still at v1 (post-Interviews 001–011); 8 more interviews since then.

### 02-Research (23)
| File | Notes |
|---|---|
| `Competitors.md` | Updated with Life Book (May 12). Contains Celonis, Clonable, Omnivisor, Life Book, pending stubs. |
| `Gemini Export — Bootcamp (5H).md` | 49K-word archival file. 0 outgoing links, 1 incoming (Origin Story). Near-island. |
| `Interview 001 — Successor.md` | Foundational; 25+ incoming links |
| `Interview 002 - Ex-Banker...` | Feedback from Carl; written format, no transcript |
| `Interview 003 - Merih (Finance Professor).md` | Decision replication framing; Clonable reference |
| `Interview 004 - Prisma Founder...` | Patterns 6–8; "digital due diligence" label |
| `Interview 005 — Real Estate Agency (Italy).md` | Contains broken pattern refs (Pattern 10) |
| `Interview 006 - John Lynch (Lynka).md` | ERP ceiling; Patterns 22–27; most analytically dense pre-012 |
| `Interview 007 — Vetreria Rachello (Italy).md` | Catastrophic succession; Lisa's gap; Patterns 13–16 |
| `Interview 008 — Antonio Rizza (M&A).md` | Documentation → price; Patterns 17–18 |
| `Interview 009 — Colusso Hardware (Italy).md` | Contains broken pattern ref (Pattern 11); 80% failure rate |
| `Interview 010 — Newton Campos (Search Fund).md` | Feasibility challenge; Pattern 21 |
| `Interview 011 — Dairy Chemicals Commercial (Italy).md` | "Chiavi di lettura"; self-preservation; low connectivity (2 incoming) |
| `Interview 012 — Stefan Weiler (Filigran, Germany).md` | Origin story; zero knowledge transfer; YPO channel |
| `Interview 013 — David (Textile Manufacturing, Germany).md` | Campfire method (Pattern 28); tech fatigue (Pattern 29); ghost pattern (Pattern 30) |
| `Interview 014 — Ulrich Bauermeister (Filigran, Germany).md` | Failed self-build; €20K experiments (Pattern 31); Fachvereinigung channel (Pattern 33) |
| `Interview 015 — Joerg von Weiler (Filigran Poland).md` | Wolf's father; origin story; YPO pipeline; Pattern 28 third confirmation |
| `Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany).md` | Pattern 22 sharpened; Patterns 34–35; ICP role-vs-size question |
| `Interview 017 — Armin Struckmeier (NUK Novatex, Germany).md` | Olive tree framework; Life Book lead; strongest M&A validation |
| `Interview 018 — Hubertus von Huelsen (AWW, Germany).md` | "Reading our document"; Pattern 34 confirmed; pre-transformation GTM; CTO lead |
| `Interview 019 — Lorenz Essing (EMH Partners, Germany).md` | Always-on GTM challenge; vulnerability mapping; soft vs hard knowledge |
| `Interview Guide.md` | Mom Test methodology; 6 live questions; contains phantom Pattern 9 reference |
| `Patterns From Fieldwork.md` | 35 confirmed patterns; 3 emerging hypotheses; most-linked file |

### 03-Outreach (2)
| File | Notes |
|---|---|
| `Email Templates.md` | Three Italian templates (commercialista, warm intro, cold) |
| `Outreach Strategy.md` | Six channels ranked; German channels underdeveloped given pivot to DACH |

### 04-Deliverables (4)
| File | Notes |
|---|---|
| `Council Report.md` | Pointer to HTML/PDF; archival; 1 incoming link (near-orphan) |
| `One-Pager — German (v3).md` | Translation of v3 English content; same staleness issues |
| `One-Pager.md` | Content v1–v3 + design history; v3 pre-fieldwork framing |
| `Pitch Deck Content.md` | 6-slide deck + Q&A prep; Q&A factually outdated |

### 05-Open-Questions (1)
| File | Notes |
|---|---|
| `Open Questions.md` | ~60+ questions; 7 categories; Answered section still empty |

### 06 - 1 to 1s (3)
| File | Notes |
|---|---|
| `1 to 1s — Week 3.md` | Mentor check-in |
| `1 to 1s — Week 4.md` | Poland fieldwork, M&A angle, ICP parameters |
| `1 to 1s — Week 5.md` | Three-interview trifecta (017/018/019), Life Book, product demo transition |

### 07-Daily-Standup (5)
| File | Notes |
|---|---|
| `Standup — 2026-05-04.md` | First standup; ICP sizing; M&A angle |
| `Standup — 2026-05-05.md` | Role split; audit decision; vault architecture |
| `Standup — 2026-05-06.md` | Outreach coordination; Nora Fehlbaum strategy |
| `Standup — 2026-05-09.md` | Pitch deck; CTO search; 5 new contacts |
| `Standup — 2026-05-11.md` | Week recap; Monday schedule; demo hypothesis |

### 99-Audit (1)
| File | Notes |
|---|---|
| `Vault Audit — 2026-05-05.md` | Prior audit; 38 files; critical recommendations partially implemented |

### Root (1)
| File | Notes |
|---|---|
| `CLAUDE.md` | Contains one stale convention (ICP Definition note) |

### Templates (3)
| File | Notes |
|---|---|
| `1 to 1s — Week {{number}}.md` | Check-in template |
| `Daily Standup Template.md` | Standup template |
| `Meeting Notes Template.md` | Interview note template |

---

## 2. Strategy Staleness Check

### `Problem Statement.md` — v4, frozen post-Interviews 002–011

**Findings from Interviews 012–019 not reflected:**

- **Pattern 28 (campfire / storytelling)** — three independent sources (David, Joerg, Armin) confirm stories surface tacit knowledge better than structured questioning. Not in thesis or methodology assumptions.
- **Three-pillar crystallization** (Week 5 / Interview 019) — extraction now articulated as: (1) interview methodology, (2) computer-use tracking, (3) document scanning. Interview methodology confirmed as most uncertain pillar. Not in Problem Statement.
- **Olive tree framework** (Interview 017) — reframes "replaceability" entirely: don't replace 1:1, split the role into pieces. Has direct implications for the irreplaceability myth (Pattern 5) and for the product deliverable concept.
- **Always-on vs event-driven** (Interview 019) — Lorenz's challenge to M&A-only framing is a strategic reframe that potentially alters the GTM entry point and the recurring revenue model. Not addressed anywhere in strategy docs.
- **Pre-transformation documentation** as third GTM angle (Interviews 016, 018) — two independent sources arrived at "do your homework before McKinsey arrives." Product has value beyond succession/M&A. Not in Problem Statement.
- **Soft vs hard knowledge distinction** (Interview 019) — hard knowledge is recoverable; soft knowledge (relationships, gut feel, judgment) is the real moat. This sharpens the "judgment framework capture" thesis from Interview 011 but is absent from v4.
- **Information vulnerability mapping** as deliverable concept (Interview 019) — a specific, nameable output that a PE board member immediately understood. Not in thesis.
- **Life Book as methodology benchmark** (Interview 017) — professional story-harvesting company is the external validation of the interview extraction approach. Sets a quality bar and a potential methodology source.
- **Digitalization paradox confirmed across industries** (Interviews 014, 016, 018) — Pattern 22 sharpened: full digital maturity does not eliminate the tacit knowledge bottleneck. Current ICP exclusion of "digitally mature" companies needs qualification.

**Verdict: STALE.** v5 needed. Direction remains sound; the pillar architecture, GTM angles, and deliverable concepts have all evolved significantly in 8 interviews.

---

### `ICP Definition.md` — v1, frozen post-Interviews 001–011

**Findings from Interviews 012–019 not reflected:**

- **Role-based vs size-based ICP question** (Interviews 016, 018) — both BWB-Gruppe and AWW are above ICP size on revenue/employees but match perfectly on pain profile. The strategic to-do raised in Interview 016 is unresolved: should ICP be "motivated technical insider with documentation pain" rather than "20–100 employees"?
- **AWW as above-ICP size but perfect pain match** — 170M revenue, 560 employees. Tool-making expert retiring in 2–3 years. CEO building the same thing. Hubi confirmed as potential pilot customer despite size. No ICP row for Interview 018.
- **Lorenz's add-on acquisition framing** (Interview 019) — EMH's €5–20M add-on acquisitions with less formal DD is exactly the ICP entry point for buyer-side. Not reflected in Secondary ICP section.
- **"Motivated technical insider"** as a distinct ICP persona (Interviews 014, 016, 018) — Bauermeister, Bergerhoff, and Hubi are all the same profile: technically capable insider who sees the problem, has internal approval to solve it, but fails at the last 10% of implementation. This persona is missing from ICP Definition entirely.
- **Evidence table only covers Interviews 001–011** — 8 more interviews with ICP-relevant data not in the table.

**Verdict: STALE.** v2 needed. The role-vs-size ICP question is the single most strategically important open question in the vault and it has no home in the ICP Definition file.

---

### `Product Methodology.md` — Working definition, pre-Pattern 28

**Findings not reflected:**

- **Campfire method not named** — Pattern 28 (from three independent sources) establishes storytelling as the primary extraction mechanism for Conversational Extraction (Pillar 3). Product Methodology still describes Pillar 3 as "structured interviews." The "why it works" rationale is entirely missing.
- **Standardgrundlage-first sequencing** (Pattern 34) — for technical-domain SMEs, the normative document layer must be ingested before storytelling adds value. Current methodology is campfire-first in all cases. Two independent sources (Bergerhoff, Hubi) explicitly confirmed this sequencing requirement.
- **"Information vulnerability mapping"** (Interview 019) — Lorenz immediately engaged with this framing as a concrete deliverable. Could replace or supplement "Organizational Report" for investor-side customers.
- **Olive tree mapping** as a potential deliverable (Interview 017) — split irreplaceable roles rather than attempting 1:1 replacement. Not yet in the deliverable spec.
- **"Judgment framework capture" framing** — referenced in Problem Statement v4 but not integrated into the methodology description. Pillar 3 still uses old "decision replication" language.

**Verdict: STALE.** The three pillars are structurally sound but the content of each pillar has been significantly refined by fieldwork. The deliverable spec needs an update.

---

### `Business Model.md` — Exploratory, post-Interview 004

**Findings not reflected:**

- **AWW as pilot candidate** — 170M revenue CEO who is already building what we're building, offered a three-way partnership conversation. Relevant to early revenue model.
- **Filigran LOI option** — Wolf's father interested in putting Baris on payroll. Team decided to maintain independence but LOI from Filigran could provide credibility. Not documented.
- **Always-on SaaS implication** (Interview 019) — Lorenz's "event-driven not M&A-only" challenge directly implies a recurring revenue model if the product becomes continuous vulnerability monitoring. Not in Business Model.
- **Pre-transformation documentation** as a distinct revenue stream — selling knowledge extraction as "homework before McKinsey" is a different buyer (CTO/operations, not founder) with different budget source (OPEX, not succession budget).

**Verdict: STALE.** The four revenue models are still valid options, but the GTM implications of three new application angles (succession, M&A, pre-transformation) and an always-on monitoring option are not captured.

---

### `Upstream vs Downstream.md` — Unresolved, post-Interview 001

**Nine high-signal interviews since last update.** Interviews 006, 010, 012, 013, 014, 016, 018 all add directly to this question. Interview 019's "always-on" framing introduces a third option beyond the binary (not upstream OR downstream, but continuous). Still marked "UNRESOLVED" with no new content.

**Verdict: CRITICALLY STALE.** This is the most neglected strategy document.

---

### `Four Sub-Problems.md` — Framework, post-Interview 001

"Current hypothesis" section still says "we are investigating Problem 2 — Readiness as the primary wedge." Interviews 007, 008, 011, 013, 017, 019 all add data: the emotional sub-problem is non-separable, the deal-structuring sub-problem has real buyer-side validation, and the matching problem (olive tree framework) has a new potential deliverable. No updates since Interview 001.

**Verdict: STALE.** Framework remains valid; the "current hypothesis" section is 18 interviews out of date.

---

### `Pitch Deck Content.md` — 6-slide, Interview 001 era

- **Slide 5 header**: "What the First Interview Told Us" — appropriate when there was one interview; now at 19. The slide may need renaming.
- **Q&A table**: "What's your N? | 1 interview done, 15+ planned" — factually wrong. Should read 19 interviews done, validation saturating.
- **Council Verdict slide references**: still directionally valid but the market data and pattern count are outdated.

**Verdict: OUTDATED.** Core narrative still holds but key statistics are wrong. Update before next external pitch.

---

### `One-Pager.md` + `One-Pager — German (v3).md` — Content v3, pre-fieldwork

- "Within weeks, we crystallize your company's intuition into a concrete output" — Interview 006 (John Lynch) explicitly challenged this: realistic timeline is 3–6 months. The one-pager is still making this claim.
- Content v3 was written to test our thesis with founders — it worked. But the thesis has moved considerably.
- German version has identical issues.

**Verdict: MESSAGING RISK.** The "within weeks" framing undermines credibility with experienced buyers. Update the timeline claim before the next round of outreach.

---

## 3. Patterns Integrity Check

**Total patterns in file: 35** (up from 24 in prior audit; 11 added: Patterns 28–35 + 3 emerging hypotheses)

### Numbering gaps — still present from prior audit (not fixed)

| Pattern # | Status | Where referenced | Resolution needed |
|---|---|---|---|
| Pattern 9 | Missing as standalone entry | `Interview Guide.md` line 127 | Notes in Patterns file say "Pattern 9 = Pattern 8 (neutral mirror)" — add explicit note to Interview Guide referencing correct number |
| Pattern 10 | Missing as standalone entry | `Interview 005` (line 105), `Interview 009` (line 98) | Content added later as Pattern 22; add a note to Pattern 22: "also referenced as Pattern 10 in older interview notes" |
| Pattern 11 | Missing as standalone entry | `Interview 009` line 99 | Content added later as Pattern 25; same fix as Pattern 10 |

**Root cause unchanged from prior audit:** Numbering shift in Interview 004 propagated forward. Interviews 005 and 009 reference pattern numbers that no longer exist as standalone entries.

### New patterns added since prior audit: all correctly numbered and sourced

Patterns 28–35 each have a source interview, and all those interviews exist in the vault. No orphaned pattern sources.

### Emerging hypotheses — three new entries

All three (olive tree mapping deliverable, Life Book investigation, boomerang successors sub-segment) are attributed to Interview 017 with the correct wikilink.

### Cross-reference: patterns referenced in interview notes vs. patterns in file

Spot-checked: Interviews 017, 018, 019 all reference patterns by number (2, 5, 17, 18, 22, 25, 26, 27, 34, 35). All these patterns exist in Patterns From Fieldwork with matching numbers. ✅

---

## 4. Interview Coverage Matrix

**19 interviews completed.** Type and geography distribution:

| Category | Interviews | Count |
|---|---|---|
| Successors (internal perspective) | 001, 013 (David) | 2 |
| SME founders — Italy | 005, 007, 009, 011, 015 (Joerg) | 5 |
| SME founders — Germany | 012, 013, 016, 017, 018 | 5 |
| Expert / advisor (non-buyer) | 002 (ex-banker), 003 (finance professor), 004 (Prisma) | 3 |
| M&A / investor buyer-side | 008 (Antonio), 010 (Newton), 019 (Lorenz) | 3 |
| Technical operations leader | 014 (Bauermeister), 016 (Bergerhoff), 018 (Hubi) | 3 |

**Note:** Interviews 014/016/018 overlap with "SME founder" category — counted as technical ops leaders because that's their primary contribution to the dataset.

### Coverage gaps

- **Female founder**: 0 interviews. All 19 interviewees are male. Whether this reflects the target market or an outreach bias is unknown.
- **Completed transitions**: 0 interviews with a founder who successfully completed a transition and can speak retrospectively. Interview 011 (dairy chemicals) is a partial case — post-acquisition but not fully resolved.
- **Successor post-acquisition** (young CEO who bought a family business): Newton (010) is the closest but speaks from an investor lens, not an operational one. The search fund searcher persona (young CEO learning a business fast) is entirely unvalidated.
- **Pre-55 founder**: All founders interviewed are 55+. The "upstream" thesis (catch founders earlier) has no firsthand validation.
- **Legal / notary / commercialista**: 0 direct interviews. The commercialista channel was the #1 rated outreach strategy but has not produced an interview yet.

---

## 5. Open Questions Sync

**Total open questions: ~65+** across 7 categories (Customer & Buyer, Knowledge Extraction, Market & Economics, Strategic, Team & Execution, Product & GTM, Competitors & Market).

### Answered Questions section

**Still empty.** No questions have been moved to the Answered section despite 8+ interviews since the living-document convention was established. Suggested migration:

| Question | Evidence for answer | Suggested status |
|---|---|---|
| "Is storytelling extraction better than structured documentation?" | Patterns 28 (three independent sources). David, Joerg, Armin all independently confirm. | ✅ Move to Answered: "Yes — campfire stories surface tacit knowledge better than process mapping (Pattern 28, 3 sources)" |
| "Can the 'campfire storytelling' method scale, or is it artisanal?" | Still open — Life Book contact is the next data point | Keep open |
| "Is 'judgment framework capture' a better product name?" | Pattern 011 confirmed, used in v4 thesis. Reasonably answered. | ✅ Move to Answered: "Adopted as primary framing in Problem Statement v4" |

### Open questions from Interviews 012–018 missing from Open Questions.md

**Interview 018 (Hubi)** — 3 open questions listed in the interview file that are absent from the living document:
1. Should "pre-transformation documentation" become a third application on the product slide alongside "Preserve & Scale" and "Acquire & Exit"?
2. Is Hubi's AI consulting colleague a potential CTO, advisor, or competitor?
3. Does the "Celonis for analog companies" framing resonate with non-technical audiences?

All three are unresolved and strategically significant. Need to be added.

**Interview 013 (David)**: Open questions appear to be in the Knowledge Extraction section ✅ (campfire scalability, AI training from stories, company story archive).

**Interview 014 (Bauermeister)**: Questions appear in Customer & Buyer and Strategic sections ✅.

**Interview 015 (Joerg)**: No distinct open questions listed in the interview file — questions are rolled into Interview 013 and 017 context. No gap.

**Interview 016 (Bergerhoff)**: Questions appear in Strategic and Customer & Buyer sections ✅.

**Interview 017 (Armin)**: Questions appear in Competitors & Market section (Life Book classification, olive tree mapping) ✅.

---

## 6. Home.md Assessment

### What's correctly linked ✅
- All 19 interviews with one-line descriptions ✅
- All 5 standups ✅ (prior audit's orphan — Standup May 05 — is now linked)
- Weeks 3, 4, 5 check-ins ✅
- All strategy docs: Problem Statement, Council Verdict, Four Sub-Problems, Upstream vs Downstream, Market Data, Business Model, Product Methodology, Origin Story ✅
- Competitors ✅
- All delivery docs: Pitch Deck, One-Pager, One-Pager German, Council Report ✅
- Outreach docs ✅
- Open Questions ✅
- Vault Audit May 05 ✅

### Missing from Home.md ❌

1. **`[[ICP Definition]]`** — NOT in the Strategy & Thesis navigation section. ICP Definition is one of the 9 files in `01-Strategy/` but is not linked from the dashboard. All other strategy files appear; this is the only one missing.

### Name inconsistency (not a broken link, but worth flagging)

- **Timeline row 103** description text reads: *"Interview 017: Armin Stuttmeyer — olive tree framework..."*
- **Navigation section** correctly uses: `[[Interview 017 — Armin Struckmeier (NUK Novatex, Germany)]]`
- **Actual filename**: `Interview 017 — Armin Struckmeier (NUK Novatex, Germany).md`

The wikilink is correct and will navigate correctly. The description text in the timeline uses a different spelling ("Stuttmeyer"). Minor, but will cause confusion when the interviewee is searched.

### Timeline accuracy

All 19 interviews appear in the timeline. All statuses are marked ✅ Done through Interview 019. The next planned milestones (one manual transformation, sharpened problem statement + MVP wedge) are correctly marked as ⬜ Planned.

The timeline error from the May 05 audit (Interview 006/007 numbering swap) has been **fixed** ✅ — Vetreria Rachello correctly appears as Interview 007 in the current file.

---

## 7. CLAUDE.md Assessment

### Accurate ✅
- Folder structure: all folders listed including `99-Audit/` ✅
- Check-in naming convention: `1 to 1s — Week N.md` matches actual files ✅
- Competitors file: correctly documented as `[[Competitors]]` in 02-Research/ ✅
- After-interview protocol: 6-step process is still correct and followed ✅

### Inaccurate ❌

**`ICP Definition` note**: CLAUDE.md currently states:
> `ICP Definition: planned file at 01-Strategy/ICP Definition.md — does not yet exist`

This is **wrong**. The file was created after the May 05 audit and exists at `01-Strategy/ICP Definition.md`. CLAUDE.md needs to be updated to: *"ICP Definition: `01-Strategy/ICP Definition.md` — v1 created May 2026, currently stale post-Interview 011."*

### Outdated ⚠️
- `02-Research/` description says "All interviews (001-011+)" — imprecise but not wrong since the "+" covers 012–019. Acceptable as written.

---

## 8. Broken Wikilinks

### Confirmed broken or phantom references

| Source file | Reference | Issue |
|---|---|---|
| `Interview Guide.md` | "Pattern 9 — the neutral mirror" | Phantom — Pattern 9 doesn't exist as a standalone entry; content is in Pattern 8. Link would navigate to nothing in Obsidian graph. |
| `Interview 005 — Real Estate Agency` | "Pattern 10 — The gestionale/ERP ceiling" | Phantom — content was later added as Pattern 22. Navigates to nothing. |
| `Interview 009 — Colusso Hardware` | "Pattern 11 — 'Under-advised' as the felt problem" | Phantom — content was later added as Pattern 25. Navigates to nothing. |
| `CLAUDE.md` | "ICP Definition: planned file... does not yet exist" | Not a wikilink but a false statement about vault state |

### Previously broken (now fixed since May 05 audit) ✅
- `[[Standup — 2026-05-05]]` orphan: linked from Home.md now ✅
- All cross-references from the May 05 audit's confirmed broken list: fixed ✅

### Path-syntax links (non-standard but functional in Obsidian)

| Source | Link | Standard form |
|---|---|---|
| `Interview 005` | `[[05-Open-Questions/Open Questions]]` | `[[Open Questions]]` |
| `Interview Guide` | `[[Templates/Meeting Notes Template]]` | `[[Meeting Notes Template]]` |

These work in Obsidian but violate the CLAUDE.md convention.

---

## 9. Standup & 1-to-1 Chain Check

### Standup chain

| From → To | Linked? |
|---|---|
| May 04 → May 05 | ✅ (May 04 Related section) |
| May 05 → May 06 | ✅ (May 05 Related section) |
| May 06 → May 09 | ✅ (May 06 Related section) |
| May 09 → May 11 | ✅ (May 09 Related section) |
| May 11 → *(next)* | N/A — most recent |

**Full standup chain is navigable.** ✅

### 1-to-1 chain

| From → To | Linked? |
|---|---|
| Week 3 → Week 4 | ✅ (Week 4 referenced in Week 3 Related) |
| Week 4 → Week 5 | ✅ (updated this session) |
| Week 5 → *(next)* | N/A — most recent |

**Full 1-to-1 chain is navigable.** ✅

### Content completeness

- **Standup May 06**: logistics/coordination standup, no strategy content — correctly labeled as such. ✅
- **Standup May 11**: Monday planning + Bergerhoff debrief context. Contains specific note: Bergerhoff interview "proposed many potential changes and specifications in our direction." This is referenced but the actual strategy pivots triggered are NOT listed in any standup or strategy doc. The debrief is documented in Interview 016 but the link between the pivots and the strategic implications is missing from the standup record.
- **1 to 1s Week 5**: Mentor feedback section is blank ("Add direct feedback from mentor here after the session"). This is expected if the session hasn't happened yet as of the file creation date.

---

## 10. Graph Structure Analysis

### Most-linked files (incoming links)
1. `Patterns From Fieldwork.md` — 45+ incoming (every interview links here; foundational accumulation point)
2. `Problem Statement.md` — 32+ incoming (backbone of the vault)
3. `Interview 001 — Successor.md` — 25+ incoming (origin interview, heavily cross-referenced)
4. `Competitors.md` — 16+ incoming
5. `Interview 006 - John Lynch (Lynka).md` — 18+ incoming (ERP ceiling, Patterns 22–27)

### Islands and near-islands

| File | Incoming links | Risk |
|---|---|---|
| `Gemini Export — Bootcamp (5H).md` | 1 (Origin Story) | Low connectivity for a 49K-word primary source |
| `Council Report.md` | 1 (Council Verdict) | Near-orphan; expected for a pointer file |
| `Interview 011 — Dairy Chemicals` | 2 | Newly integrated since May 05 audit; still low |
| `ICP Definition.md` | ~3–5 (Problem Statement + some interviews) | New file; expected to accumulate links |

### Key clusters (unchanged structure, growing volume)

**Cluster A — Core Thesis:** Problem Statement ↔ Four Sub-Problems ↔ Upstream vs Downstream ↔ Council Verdict ↔ Interview 001 — still the conceptual backbone

**Cluster B — Research Accumulation:** Interviews 001–019 → Patterns From Fieldwork ← Interview Guide ← Open Questions — substantially grown since May 05

**Cluster C — Delivery:** One-Pager ↔ Email Templates ↔ Outreach Strategy ↔ Pitch Deck — minimal internal cross-linking; weakly connected to fieldwork findings

**Cluster D — Project History:** Origin Story ↔ Market Data ↔ Gemini Export → Council Report — stable; Gemini Export remains the most under-connected large file

### Bridge nodes

1. `Problem Statement` — connects Clusters A, B, C
2. `Patterns From Fieldwork` — connects Clusters A and B; primary accumulation node
3. `Competitors` — bridges research (Cluster B) and strategy (Cluster A)
4. `One-Pager` — bridges strategy/research to delivery (Cluster C)

---

## 11. Competitors File Check

### Current entries in `Competitors.md`

| Competitor | Status | Last updated |
|---|---|---|
| Celonis | Well-documented; scale caveat added (Lorenz: sub-€250M revenue = not complex enough) | Current |
| Clonable | Present; decision-replication concern documented | Current |
| Omnivisor | Warsaw-based; engaged with Lynka; our direct competitor | Current |
| Life Book | **NEW** — added this session; YPO company, story-harvesting + AI, Andrea contact, methodology source | Current |
| Stubs (unresearched) | Kern Unternehmensnachfolge, others | Outdated stubs |

### Missing from Competitors file

- **Hubi's AI consulting partner** (Interview 018) — "manufacturing AI use cases, ~100km from AWW" — mentioned as CTO lead but may be adjacent competition. Not yet assessed or added.
- **Rocket Internet Builders Circle** (Week 5 check-in) — applied to program; could surface additional market context or competitive intelligence.

### Celonis comparison — updated context from Interview 019

Lorenz confirmed: "Their use case stops making sense when companies are smaller than €250M in revenue." This is the first empirically grounded scale cutoff from a practitioner. The Competitors file should note this. The "Celonis for analog companies" framing (from Interview 018) is powerful but needs the scale caveat added.

---

## 12. Deliverables Status

| Deliverable | Audience | Last content update | Key issue |
|---|---|---|---|
| Problem Statement | Internal | v4, post-Interviews 002–011 | STALE — see Section 2 |
| ICP Definition | Internal | v1, post-Interviews 001–011 | STALE — see Section 2 |
| One-Pager (all versions) | Founders / experts | v3, pre-fieldwork | "Within weeks" claim is wrong (per Interview 006) |
| Pitch Deck | Cohort / mentors | Interview 001 era | Q&A statistics wrong; N=19 not "1 done, 15+ planned" |
| Email Templates | Outreach | Created pre-fieldwork | Italian-only; no German template exists despite shift to DACH focus |
| Outreach Strategy | Internal | Created pre-fieldwork | German channels underdeveloped (trade associations, YPO, Fachvereinigungen) |
| Interview Guide | Operational | Current through Interview 016 | Contains phantom Pattern 9 reference |

### Critical delivery gap: German outreach templates

The outreach pivot toward Germany (Interviews 012–019 are all German contacts) has no corresponding outreach infrastructure. Email Templates has three Italian-language templates and zero German templates. Given the pipeline consists almost entirely of DACH contacts, this is an active gap.

---

## 13. Tags Audit

### Tag conventions observed

| Tag | Used in | Consistency |
|---|---|---|
| `#strategy` | Strategy files, key research | ✅ Consistent |
| `#research` | Research files, Patterns, Open Questions | ✅ Consistent |
| `#interview` | All interview files | ✅ Consistent |
| `#pattern` | Not used — patterns live in Patterns file | Expected |
| `#standup` | All standup files | ✅ Consistent |
| `#check-in` | All 1-to-1 files | ✅ Consistent |
| `#weekly` | All 1-to-1 files | ✅ Consistent |
| `#daily` | All standup files | ✅ Consistent |
| `#deliverable` | Deliverable files | ✅ Consistent |
| `#outreach` | Outreach + Email Templates | ✅ Consistent |
| `#living-document` | Patterns, Open Questions | ✅ Consistent |
| `#core` | Problem Statement, ICP, Product Methodology | ✅ Consistent |
| `#to-validate` | Occasional | Inconsistent — some interviews add this in-body but not as a file tag |
| `#audit` | Audit files | ✅ Consistent |
| `#home` | Home.md | ✅ |

### Issues

1. **`#to-validate`** appears in some interview files as a body marker for unverified claims but is not consistently used as a file-level tag. Decision: use it in body text only (current usage is fine), not as a file-level tag.
2. **Meeting Notes Template** has `#interview #research` as footer tags — this is the right convention. All 19 interview files follow it.
3. **Templates** themselves carry no tags — correct (template files shouldn't be in the knowledge graph).
4. **`#germany` / `#italy` / `#poland`** geography tags are used inconsistently. Interviews 012–019 use them; earlier Italian interviews (005, 007, 009, 011) do not. Not critical, but limits graph filtering by geography.

---

## 14. Recommended Actions

### CRITICAL (blocks credibility in external conversations)

**1. Fix CLAUDE.md: ICP Definition note**
Change: `ICP Definition: planned file at 01-Strategy/ICP Definition.md — does not yet exist`
To: `ICP Definition: \`01-Strategy/ICP Definition.md\` — v1 created May 2026, covers Interviews 001–011`
This is a false statement about vault state that will cause Claude Code to behave incorrectly.

**2. Add [[ICP Definition]] to Home.md navigation**
Under "Strategy & Thesis" section. ICP Definition is the only file in `01-Strategy/` not linked from the dashboard. Simple one-line fix.

**3. Update Pitch Deck Q&A: N count**
Line: `"What's your N? | 1 interview done, 15+ planned"`
Change to: `"What's your N? | 19 interviews complete across Germany, Italy, Poland. Validation pattern saturation beginning — fewer new patterns per interview."`
This is factually wrong and will undermine credibility in any live pitch context.

**4. Add three missing open questions from Interview 018 to Open Questions.md**
Under "Product & GTM" or new "GTM Applications" sub-section:
- Should "pre-transformation documentation" become a third application alongside "Preserve & Scale" and "Acquire & Exit"?
- Is Hubi's AI consulting colleague a CTO candidate, advisor, or adjacent competitor?
- Does the "Celonis for analog companies" framing resonate beyond audiences who already know Celonis?

---

### IMPORTANT (strategic alignment and vault navigability)

**5. Resolve phantom pattern numbers 9, 10, 11**
Option A (minimal): Add a note to Pattern 22 in Patterns From Fieldwork: "*(also referenced as Pattern 10 in Interview 005 and Interview 009)*" and same for Pattern 25 / Pattern 11. Add a note to Pattern 8: "*(also referenced as Pattern 9 in Interview Guide)*".
Option B (thorough): Update Interview 005, Interview 009, and Interview Guide to reference the correct current pattern numbers.
Recommendation: Option A — lower maintenance burden, preserves historical accuracy.

**6. Update Problem Statement to v5**
Minimum additions:
- Three-pillar crystallization from Week 5 (interview methodology as most uncertain pillar)
- Always-on vs event-driven GTM reframe (Interview 019 — Lorenz's challenge)
- Soft vs hard knowledge distinction (Interview 019)
- Pre-transformation documentation as third GTM angle (Interviews 016, 018)
- Campfire method as confirmed extraction approach (Pattern 28, three independent sources)

**7. Update ICP Definition to v2**
Minimum additions:
- "Motivated technical insider" as a distinct persona (Bauermeister, Bergerhoff, Hubi)
- AWW as above-ICP-size but perfect-pain-profile example
- Evidence table rows for Interviews 012–019
- Role-based vs size-based question — explicitly address or defer with reasoning

**8. Update Upstream vs Downstream with eight new data points**
This document has been frozen since Interview 001 and directly impacts GTM strategy. At minimum: add Interview 006 (downstream-too-late case), Interview 010 (prospective vs retroactive divide), and Interview 019 (always-on as third option beyond the binary).

**9. Fix Home.md timeline text: Interview 017 name**
Timeline row 103: `"Interview 017: Armin Stuttmeyer"` → `"Interview 017: Armin Struckmeier"` (consistent with filename and wikilink).

**10. Update Product Methodology**
Add campfire method as primary mechanism for Pillar 3 (Conversational Extraction). Add Standardgrundlage-first sequencing as an alternative entry sequence for technical-domain customers. Update Pillar 3 language from "decision replication" to "judgment framework capture."

---

### MINOR (housekeeping and future-proofing)

**11. Begin populating "Answered Questions" section in Open Questions.md**
At minimum move: "Is judgment framework capture a better framing?" (adopted in v4) and "Do storytelling methods outperform structured questioning?" (Pattern 28, three sources). Gives the living document closure and makes progress visible.

**12. Create German outreach email template**
Email Templates has three Italian-language templates and zero German templates. Given that 7 of the last 8 interviews are German contacts, this is an active outreach gap. A German warm-intro and a German cold-founder template are both needed.

**13. Add Hubi's AI consulting colleague to Competitors file as a stub**
Manufacturing AI for analog companies, ~100km from AWW. Not yet assessed but potentially adjacent competition. Worth a stub entry with the "CTO or competitor?" open question flagged.

**14. Add [[ICP Definition]] to Outreach Strategy**
Outreach Strategy currently describes channels without linking to who we're targeting. A single line in the document pointing to [[ICP Definition]] would anchor the strategy to the customer definition.

**15. Add geography tags to Interviews 005, 007, 009, 011**
Minor consistency fix for graph filtering. Interviews 012–019 use `#germany / #poland`; earlier Italian interviews use no geography tag.

---

## 15. Compact Vault Summary

**What this vault is:** A knowledge base for Wolf and Giuseppe (ESMT Vali Hub) building an AI-powered "digital due diligence" service that extracts and documents tacit knowledge from SME founders. Pre-product, fieldwork phase. Target customer: the successor (not the founder) of a family-owned SME in Germany or Italy, €5–25M revenue, 20–100 employees, founder 55–72.

**Current thesis:** Organically grown SMEs run on expertise that lives in people's heads. AI now makes this tractable to extract before it retires. The extractable asset is not processes (ERPs handle that) but judgment frameworks — the "chiavi di lettura" that let a successor read situations independently. Primary extraction mechanism: campfire storytelling. Primary value: compressing the 1–5 year post-succession handover period and increasing M&A deal price through documentation completeness.

**19 interviews completed:** Founders (10), successors (2), M&A/investor buyer-side (3), expert advisors (3), technical operations leaders (3). Germany: 6 interviews. Italy: 5. Poland: 3. Cross-country pattern confirmation is strong.

**35 patterns confirmed.** The most important for product design: Pattern 28 (stories beat processes), Pattern 34 (Standardgrundlage-first for technical domains), Pattern 35 (three trust thresholds within one company), Pattern 22 (digital maturity ≠ immunity to tacit knowledge bottleneck).

**Three GTM angles now confirmed:**
1. **Preserve & Scale** — founder succession, operational continuity
2. **Acquire & Exit** — M&A documentation completeness, deal price protection
3. **Pre-transformation documentation** — "do your homework before McKinsey arrives" (two independent sources)

**Open strategic questions remaining:**
- Always-on (continuous vulnerability monitoring) vs event-driven (M&A moments) — Lorenz's challenge, unresolved
- Role-based vs size-based ICP — two interviews above size but perfect pain profile
- Interview methodology as extraction pillar — is Life Book the quality benchmark? Andrea contact not yet reached.
- Technical co-founder — required to build demo

**Current vault health:**
- **Living documents** (Patterns, Open Questions) — well-maintained ✅
- **Strategy docs** — severely stale: Problem Statement at v4 (post-Interview 011), ICP Definition at v1 (post-Interview 011), Product Methodology, Four Sub-Problems, Upstream vs Downstream all frozen pre-Interview 012 ❌
- **Delivery docs** — outdated statistics in Pitch Deck Q&A; "within weeks" claim in One-Pager ❌
- **CLAUDE.md** — one false statement about ICP Definition file existence ❌
- **Wikilinks** — 3 phantom pattern references (9, 10, 11); all actual file links navigable ✅
- **ICP Definition** — missing from Home.md navigation despite being in 01-Strategy/ ❌
- **German outreach templates** — zero templates for DACH outreach despite pivot to German market ❌

**Most urgent:** Fix CLAUDE.md ICP note, add ICP Definition to Home.md, update Pitch Deck Q&A statistics, add Interview 018 open questions. Then update Problem Statement to v5 and begin Problem Statement v5 / Product Methodology update before next cohort presentation or investor conversation.

---

## Related
- [[Vault Audit — 2026-05-05]] — prior audit (38 files, 11 interviews)
- [[Home.md]] — dashboard; ICP Definition missing from navigation
- [[Problem Statement]] — v5 needed
- [[ICP Definition]] — v2 needed; missing from Home.md
- [[Patterns From Fieldwork]] — phantom patterns 9, 10, 11 need resolution
- [[Open Questions]] — Interview 018 questions missing; Answered section still empty
- [[CLAUDE.md]] — ICP Definition note is wrong
