# Vault Audit — 2026-05-20

#audit #meta #forensic

> **Generated:** May 20, 2026 (Opus 4.7)
> **Method:** Read every .md file in vault except 00-Raw/. Cross-referenced patterns, wikilinks, name variants, and Sonnet-processed content for forensic accuracy. Read-only.
> **Scope:** 125 files added since 2026-05-12 + all prior files. Total: ~165 .md files (excluding 00-Raw/).
> **Context:** Third full audit. Prior: 2026-05-05 (38 files), 2026-05-12 (53 files). Since May 12: Interviews 020–024 added, 18 MI notes consolidated, 04-Network/ folder created (46 files), 4 standups/1:1s added, 3 strategy docs touched.

---

## 1. Forensic Check of Sonnet-Processed Content

| File | Verdict | Detail |
|---|---|---|
| `Interview 020 — Francis de Vericourt` | ⚠️ WARNING | References to "Pattern 39 — Partial-capture honesty principle" cascade into multiple files. Interview 020 itself does NOT claim to add Pattern 39 (the file correctly says "New observation — not a pattern, a strategic directive"). But Interviews 021 and 022 cite "Pattern 39 (Francis, Interview 020)" as if it exists in `Patterns From Fieldwork.md`. **Pattern 39 is undefined in the patterns file.** Content otherwise clean; date correct; all wikilinks valid. |
| `Interview 021 — Roland Wübbe` | ⚠️ WARNING | Two issues. (a) "Pattern 8 — Long onboarding by osmosis" cited as confirmed, but Pattern 8 in `Patterns From Fieldwork.md` is "Neutral mirror sells better than improvement plan." Mismatch. (b) Cites "Pattern 39" twice — phantom. Patterns 37, 38 correctly added. All other refs (Patterns 2, 5, 14, 16) valid. Date correct, wikilinks valid. |
| `Interview 022 — Marco Nortmeier` | ⚠️ WARNING | Claims "Pattern 39 — Partial-capture honesty principle: Marco's '99,9999% aber nie 100%' framing is a practitioner's version of Francis's honesty principle" as CONFIRMED. Pattern 39 does not exist. Pattern 40 correctly added and well-sourced. All other refs (Patterns 2, 22, 25, 29, 35) valid. Wikilinks valid. |
| `Interview 023 — Maciej Bogacz` | ✅ PASS | All pattern references (17, 18, 14, 16) match existing patterns. SHARPENS Pattern 17 (correctly identified as not adding a new pattern). All wikilinks valid. Date correct. Strong file. |
| `Interview 024 — Eberhard Müller-Menrad` | ⚠️ WARNING | Cites Pattern 11 ("Self-preservation knowledge hoarding") confirmation but Pattern 11 is **renumbered to Pattern 25** in the patterns file (with explanatory note). Should reference Pattern 25, not Pattern 11. Patterns 41, 42 correctly added; Pattern 5, 14, 35 references valid. All wikilinks valid. **Note:** User-overwritten version replaced the original. Spelling typo "Armin Struckmier" appears in Action Items pointing to "Interview 017 — Armin Struckmeier" — wikilink is correct, prose spelling is the inconsistent one. |
| All 18 MI notes | ✅ PASS (spot-checked) | Consistent frontmatter format (title, tags, created date); each has a Solcus-angle section and Related section. Wikilinks valid. The three latest (Silver Tsunami, Domain Expert, Expert Interview Design) follow the established template. No phantom links. |
| `1 to 1s — Week 6` | ✅ PASS | Chained to Week 5; references Standup 2026-05-19; new leads table populated. Mentor Feedback section empty (expected — not yet held at writing time). |
| `Standup — 2026-05-14` | 🔴 FAIL (name accuracy) | Three name errors in the "Week Recap" interview table: (a) "Roland Werbe" should be **Roland Wübbe** (Interview 021), (b) "Michael Nordmeyer" should be **Marco Nortmeier** (Interview 022), (c) "Justus Müller-Menrad" — ambiguous: standup says "possibly in M&A in Dubai" but Interview 024 says Eberhard's Dubai son is **Lucas** (management consulting → INSEAD). One additional name in Outreach: "Johann Vermut" should be **Jochen Wermuth** (per Network folder + standup context). |
| `Standup — 2026-05-19` | ✅ PASS | Properly chained. Concise. Open threads documented. |
| `Standup — 2026-05-20` | ✅ PASS | User-restructured version. Frontmatter present, Related section added. Detailed sections all consistent with raw transcript. |

**Critical cascade finding:** Pattern 39 is referenced as if defined in at least 4 places (Interview 021 source list, Interview 022 confirmed-patterns list, Patterns From Fieldwork Pattern 37 commentary, Open Questions "OBJECTION CLUSTER 21+37+39"). It is the most consequential phantom in the vault.

---

## 2. Network Folder Scan (04-Network/)

**Total: Contact List + 45 People notes.**

### Linkage
- **Contact List ↔ People notes:** 45/45 ✅. Every People note is referenced exactly once.
- **People → Interviews:** 19/45 People notes link to a corresponding interview. 26 People notes have no interview link (most are "Must contact" / "Met-warm" — pre-interview).

### Interviews missing a People note (gaps)

| Interview | Interviewee | Status |
|---|---|---|
| 001 | Successor (anonymous) | Acceptable to keep anonymous |
| 002 | Karl Rohr | ✅ People note exists ([[Karl Rohr]]) but Karl's note doesn't backlink to Interview 002 — partial |
| 008 | **Antonio Rizza (M&A)** | 🔴 MISSING — No People note exists |
| 011 | Filippo Parovel | People note exists but content is template-only |
| 013 | David Richter | ✅ Exists and backlinks |
| 015 | Joerg von Weiler | People file is "Joerg Weiler" (no "von"); links correctly |

### Confirmed name typos in People filenames

| Current filename | Should be | Source of truth |
|---|---|---|
| `Armin Struckmier.md` | `Armin Struckmeier.md` | Interview 017 file + Home.md |
| `Eberhard Mueller-Menrad.md` | `Eberhard Müller-Menrad.md` | Interview 024 file |
| `Linus Wubbe.md` | `Linus Wübbe.md` | Roland Wübbe family + own note says "Wübbe family connection" |
| `Krzysztow Kwiatkowski.md` | `Krzysztof Kwiatkowski.md` (likely) | Standard Polish first name |

### Thin/empty People notes (template-only, no substantive content)

Aneta Sikora, MaCeVi, Oskar Gieburowski, Filippo Parovel, Jo Mate, Grzegorz Ptak, Leopold Weiler, Michael Pram Rasmussen, Emilia Grossmann, Krzysztow Kwiatkowski, Mikkel Karlsen, Mr Van Der Leyly, Scott Zuckerman, Thomas Maschall, Walter Davanzo, Yannick Schmidt, Yolla Salmuth, Sebastian Grass.

Total: 18 People notes are essentially placeholders. Most are intentional (pre-interview contacts) but worth flagging.

### Frontmatter / tags
**Zero People notes use YAML frontmatter or hashtag tags.** This is inconsistent with the rest of the vault. Decision needed: either add `#contact #person` tags to People notes for graph filtering, or keep them tagless by convention.

### Eberhard/Lucas/Justus identity ambiguity
- Armin (Interview 017) offered intro to "Müller-Menrad (PwC Dubai M&A)"
- Standup 2026-05-14 referenced this as "Justus Müller-Menrad" possibly in Dubai M&A
- Interview 024 confirms Eberhard's son **Lucas** is in Dubai management consulting → INSEAD
- The Eberhard People note explicitly flags this: "To be clarified whether this is the same person as the Müller-Menrad (PwC Dubai M&A) that Armin offered to introduce."
- **Unresolved.** Could be (a) same person (Lucas works at PwC), (b) different family member entirely, or (c) Lucas + a separate cousin. Verify before duplicate outreach.

---

## 3. Phantom Links Sweep

**Active phantom wikilinks (excluding audit files): 0.**

All active wikilinks across 02-Research, 04-Network, 04-Deliverables, and the recently-Sonnet-created MI/interview/standup notes resolve to existing files. The Explore agent's report is confirmed.

**Historical phantom references (from prior audit narrative, harmless):** 5 in `99-Audit/Vault Audit — 2026-05-05.md` documenting earlier broken links since fixed.

**Non-wikilink phantom references (CRITICAL — these are inline pattern numbers and concept references):**

| Type | Phantom | Source | Recommendation |
|---|---|---|---|
| Pattern number | "Pattern 39" — Francis's "Partial-capture honesty" | Interview 021 (Patterns Confirmed + objection cluster); Interview 022 (Patterns Confirmed); Patterns 21, 37 commentary; Open Questions "OBJECTION CLUSTER" | Either define Pattern 39 explicitly in Patterns From Fieldwork (using the language from Interview 020's "New observation"), OR rewrite all references to make clear it's an unnumbered strategic directive, not a pattern |
| Pattern number | "Pattern 11" — self-preservation hoarding | Interview 024 confirmed-patterns list | Replace with Pattern 25 (the renumbered location) — note in Patterns file already documents this |
| Pattern number | "Pattern 10" — ERP ceiling | Interview Guide line 89; Interview 005; Interview 009 | Replace with Pattern 22 (renumbered) |
| Pattern number | "Pattern 9" — neutral mirror | Interview Guide line 127 | Replace with Pattern 8 (renumbered) |
| Pattern number | "Pattern 8 — Long onboarding by osmosis" | Interview 021 confirmed-patterns | Misnaming. Pattern 8 is "Neutral mirror." There is no pattern named "long onboarding by osmosis" — the concept is partially in Pattern 27 (onboarding speed) |

---

## 4. Patterns From Fieldwork Integrity

### Pattern count: 36 active + numbering gaps

**Sequential numbering:** 1–8, 12–35, 37, 38, 40, 41, 42.

**Gaps:**
- 9, 10, 11 — historical renumberings; explanatory notes present in patterns file. Acceptable.
- **36 — true gap.** No pattern, no explanatory note. Status unknown.
- **39 — phantom.** Heavily referenced as if defined, but the patterns file has no Pattern 39 entry. Most consequential vault inconsistency.

### Order anomaly
Patterns are **out of numerical order in the file:** 37, 38, **41, 42, 40** (last three are out of sequence). Should be 37, 38, 40, 41, 42.

### Pattern-to-source verification (Interviews 016–024)

| Pattern | Claimed source | Source file confirms claim? |
|---|---|---|
| 34 | Interview 016 | ✅ |
| 35 | Interview 016 + 014 cross-ref | ✅ |
| 37 | Interview 021 | ✅ |
| 38 | Interview 021 | ✅ |
| 40 | Interview 022 | ✅ |
| 41 | Interview 024 | ✅ |
| 42 | Interview 024 + cross-refs 014, 016, 018 | ✅ |

All defined patterns from recent interviews have valid sources. ✅

### Interview-pattern claims (forward check: does every pattern an interview claims actually exist?)

- Interview 016: claims 34, 35 — both exist ✅
- Interview 017: no new patterns claimed (3 emerging hypotheses added) ✅
- Interview 018: no new patterns; claims Pattern 34 confirmation ✅
- Interview 019: no new patterns; cross-references 17, 18, 22, 27 ✅
- Interview 020: no new patterns (correctly marked as "strategic directive") ✅
- Interview 021: claims 37, 38 + cites Pattern 8 (mismatch) + Pattern 39 (phantom) ⚠️
- Interview 022: claims 40 + cites Pattern 39 (phantom) ⚠️
- Interview 023: claims SHARPENS 17, QUANTIFIES 18 ✅
- Interview 024: claims 41, 42 + cites Pattern 11 (renumbered to 25) ⚠️

### Emerging hypotheses currency

Three emerging hypotheses from Interview 017 still in the file:
- Olive tree mapping deliverable — STATUS: now part of Product Methodology as a deliverable. Could move from "emerging" to "adopted concept" or be removed.
- Life Book competitor/partner — STATUS: open. Andrea contact still pending. Keep.
- Boomerang successors sub-segment — STATUS: open. Keep.

The other emerging hypotheses (older) have several entries that could be re-evaluated:
- "Tacit knowledge can actually be extracted with structured protocols" — substantially answered by Patterns 28, 34, MI — Silver Tsunami (Kempten study), MI — Expert Interview Design. Should move to Answered.
- "Eager successors (not reluctant ones) are the real population" — answered by Pattern 16 (refusal pattern) + multiple interviews. Should move to Answered.
- "Employees will resist having their knowledge captured" — answered by Pattern 28 (storytelling welcomed) + Pattern 41 (timing matters). Mixed evidence already captured; can be moved to Answered with nuance note.

---

## 5. Open Questions Sync

### Total
~85 open questions across 8 categories. Answered section grew from empty (May 12) to substantive (~15 entries). ✅ Good progress.

### Verified evidence links
Spot-checked Answered section: all wikilinks to evidence interviews resolve. ✅

### Interview 024 questions MISSING from Open Questions

The Eberhard interview raises 5 explicit open questions that are **NOT in Open Questions.md:**
1. How do we operationally screen prospects on the Pattern 41 axis (expert career stage / retirement timing)?
2. Is the creative bottleneck (fashion/design) a future market to name in pitch materials, or kept internal?
3. Should "stuck in the middle" consolidation pressure become a fourth urgency force alongside succession + AI window + talent scarcity?
4. NPal (Berlin scale-up via Moritz) — is this a research conversation only, or a genuine ICP probe?
5. How does Pattern 41 (retirement window) intersect with Pattern 37 (atrophy)? Does engaging at retirement partially resolve the atrophy concern?

### Questions that LATER interviews effectively answered but weren't crossed off

| Question | Now answered by | Suggested move |
|---|---|---|
| "Can we quantify our product reduces earn-out percentage from X% to Y%?" (Interview 023) | Maciej's detailed quantification gives the data (10-20% retention, €20-40K/month advisory). Calculation is buildable. | Move to PARTIAL-ANSWERED with calculation framework |
| "What is the right framing for an internal Filigran exercise...?" (Interview 022) | Standup 2026-05-20 crystallised "seminar / delegation-first" approach | Move to ANSWERED — Filigran is positioned as co-development partner |
| "Should 'pre-transformation documentation' become a third application?" (Interview 018) | Adopted in Problem Statement v5 as Pivot 13 | Move to ANSWERED |

### Phantom Pattern 39 referenced in Open Questions
The "OBJECTION CLUSTER (21 + 37 + 39)" entry repeats the Pattern 39 phantom reference. Fix downstream of resolving the Pattern 39 issue itself.

---

## 6. Home.md Completeness

### What's correctly linked ✅
- Every interview 001–024 ✅
- Every standup (May 04 → May 20) in chronological order ✅
- Every 1-to-1 (Week 3 → Week 6) ✅
- All 11 strategy docs (including ICP Definition, fixed since May 12) ✅
- All 18 MI notes + Interview Guide + Patterns From Fieldwork ✅
- All 4 deliverables ✅
- Open Questions ✅
- Templates not linked (correct — templates shouldn't be in graph)

### Missing from Home.md ❌

1. **`[[Vault Audit — 2026-05-12]]`** — Audits section only links the May 5 audit. May 12 audit exists but is not linked.
2. **`[[Contact List]]` (04-Network/)** — Entire 04-Network/ folder is not surfaced from Home.md. This is a 46-file structural addition since May 12 with zero dashboard visibility.
3. **`Files/Future of European SME.pdf`** — Files/ folder content not linked. If `Files/` is meant to be an asset folder, this is fine; if it's research, it should be linked.
4. **`Untitled.canvas`** — Untracked file at vault root. Either name it/move it or delete.

### Timeline accuracy
- All 24 interviews appear in timeline ✅
- All 8 standups appear ✅
- Roland Wübbe correctly spelled ✅ (May 12 audit's Stuttmeyer flag now appears resolved — current Home.md uses Struckmeier ✅)

---

## 7. CLAUDE.md Consistency

### Accurate ✅
- After-interview protocol
- Wikilink convention
- Raw file hub-link rule (added since May 12)
- No-phantom-links rule (added since May 12)
- Audit operations

### Stale / Wrong

1. **Living documents line:** *"Patterns From Fieldwork.md — patterns 1-27, add new ones here"* — count is wrong. Now 42 numbered, with gaps. Should be "patterns 1-42 with documented numbering gaps at 9, 10, 11, 36, 39."
2. **Folder Structure section:** Does NOT acknowledge **04-Network/** (new since May 12; 46 files). Add: `04-Network/ → Contact List + per-person notes for outreach pipeline`.
3. **Folder Structure section:** Does NOT acknowledge **Files/** folder (exists per git history with `Future of European SME.pdf`). Add or remove the folder.
4. **02-Research/ description:** *"All interviews (001-011+)"* — imprecise; bump to "001-024+".
5. **ICP Definition note:** *"v1 created May 2026, covers Interviews 001–011. Needs v2 update."* — outdated; ICP Definition is already at v2 (covers 001–019). Should say: *"v2 created May 12 2026, covers Interviews 001–019. Needs v3 update to incorporate Interviews 020–024 + Pattern 41 timing axis + post-handover former CEO segment."*

### No mentions of Solcus name
The CLAUDE.md `## Project` line refers to *"an AI-powered 'digital due diligence' service"* — no mention that the project is named **Solcus** (decided 2026-05-14). Either update or note that "Solcus" is the working name.

---

## 8. Raw Files Cluster Integrity

Per audit instructions, 00-Raw/ contents were NOT read. Cannot verify `[[RAW FILES]]` hub-link on every file individually. However, sample evidence from previously-read raw files (in earlier conversation context) confirms the convention is being applied (e.g. `Capturing Tacit Knowledge from the Great Retirement Cohort.md`, the standup transcripts, all end with `[[RAW FILES]]`).

**Recommendation:** A separate audit run with raw-files-included scope can verify the convention completely.

**Approximate ratio of raw files to structured notes:**
- Raw files in 00-Raw/: ~52 (per directory listing)
- Structured notes derived from them: 24 interviews + 18 MI notes + 8 standups + 4 1:1s = 54 structured notes
- Ratio is ~1:1 — every raw file has a structured corollary, which is healthy. ✅

---

## 9. Strategy Docs Currency

| Doc | Last touched | Covers up to | Reflects post-May 12 work? |
|---|---|---|---|
| `Problem Statement.md` | May 12, v5 | Interviews 012–019 | ❌ No mention of Interviews 020–024, Patterns 40/41/42, methodology-not-model framing (020/022), Solcus name, closed-loop system, post-handover CEO segment |
| `ICP Definition.md` | May 12, v2 | Interviews 001–019 | ❌ Missing post-handover CEO segment (021, 024), Pattern 41 timing axis, Pattern 42 cross-industry confirmation, "internal IT lead with operational authority" persona (022) |
| `Product Evolution Log.md` | May 12 | Pivots 1–14 | ❌ Missing: Solcus name (Pivot 15+), two-track Filigran pilot (Pivot from 022), "consulting practice not tech company" identity reframe (Pivot from 020), closed-loop system (Pivot from Week 6), delegation-first scalability (Pivot from Standup 20), retirement-window timing (Pivot from 024) |
| `Product Methodology.md` | Updated post-Pattern 28/34 | Pillars + Pattern 28, 34 | ❌ Missing Pattern 35 (three trust thresholds), Pattern 40 (documentation entropy → maintenance mechanism), Pattern 41 (timing), methodology-not-model framing |
| `Competitors.md` | May 14 | Inc. Ontora (Week 6) | ❌ Missing: SAP-implementation knowledge-capture startup (€3.5M raised, mentioned in Interview 024); Pattern 41 timing dimension; "Armin Stuttmeyer" (Life Book section) — name still misspelled |
| `Upstream vs Downstream.md` | May 12 | Through Interview 019 | ❌ Missing: post-handover Roland case (021) — the meta-witness; insolvent Eberhard case (024) — the cautionary tale |
| `Business Model.md` | Pre-May 12 (stale, per May 12 audit) | Pre-Interview 011 | ❌ Same staleness as May 12 audit identified; no progress |
| `Four Sub-Problems.md` | Pre-May 12 (stale) | Pre-Interview 002 | ❌ Same staleness as May 12 audit identified |
| `Market Data.md` | Unchanged | Country-level stats | Stable; but could be augmented with Silver Tsunami MI numbers (43% Germany retiring by 2036, $31.5B Fortune 500 attrition) |

### Cross-doc consistency issues

**Pitch Deck Slide 4** says ICP is *"€2-20M revenue"* but **ICP Definition** says **€5-25M revenue**. Mismatch.

**Pitch Deck Slide 5** still says "What the First Interview Told Us" — narrative anchor is 23 interviews stale.

**Pitch Deck Slide 1** still has `[Project Name]`, `[Names]`, `[Accelerator]`, `[Date]` placeholders. Solcus name not integrated.

**Pitch Deck Q&A** says "19 interviews complete... 35 patterns surfaced." Now 24 interviews + 36 patterns + 5+ MI-validated insights.

**Three Pillars sequencing** differs across docs:
- Problem Statement v5: storytelling first (campfire)
- Product Methodology: OCR/digital archaeology first (Pillar 1)
- These can be reconciled via Pattern 34 (Standardgrundlage-first for technical domains, campfire-first for relational) — but neither doc names this reconciliation cleanly.

---

## 10. Market Intelligence Assessment

**18 MI notes + 1 Second Brain Landscape index.**

### Format consistency
All 18 follow approximately the same template:
- Sources block at top
- "What This Is" framing paragraph
- Key Insights Relevant to Solcus (numbered, with "Solcus angle" subsections)
- "What We Can Learn" / actionable summary
- Related links

✅ Strong format consistency. The three most recent (Silver Tsunami, Domain Expert, Expert Interview Design) match the established template.

### Second Brain Landscape index
Lists all 18 MI notes ✅. Updated through the most recent batch (2026-05-20).

### Cross-reference to product
Every MI note has a "Solcus angle" or product-relevance section. ✅ Strong.

### Possible merges / overlaps

| Pair | Reason | Recommendation |
|---|---|---|
| MI — Storytelling and Tacit Knowledge Capture **+** MI — Classical Knowledge Elicitation Methods **+** MI — Expert Interview Design | All three cover knowledge elicitation methodology from different academic/applied angles | KEEP SEPARATE — they're distinct disciplines (KM, KE engineering, qualitative research). Cross-links are correct. |
| MI — Mem (a16z) **+** MI — Second Brain Execution Layer | Both consumer-second-brain perspectives | KEEP SEPARATE — different audiences (consumer vs team) |
| MI — Company Brain Concept **+** MI — Context Engineering Platforms | Overlapping enterprise context layer themes | KEEP SEPARATE — different layers of the same stack |

No empty/raw-dump MI notes found.

---

## 11. Tag and Frontmatter Consistency

### Tag inventory (unique tags found across vault)

Recurring tags (consistent): `#strategy`, `#research`, `#interview`, `#standup`, `#daily`, `#check-in`, `#weekly`, `#deliverable`, `#outreach`, `#living-document`, `#core`, `#home`, `#dashboard`, `#audit`, `#meta`, `#patterns`, `#market-intelligence`, `#mom-test`, `#thesis`, `#critical`, `#unresolved`

Geography tags (inconsistent): `#germany`, `#italy`, `#poland` used in Interviews 012–024 but NOT in earlier Italian interviews (005, 007, 009, 011).

Industry tags (inconsistent): `#manufacturing`, `#construction`, `#eyewear`, `#family-business`, `#m-and-a`, `#sell-side`, `#post-insolvency-mittelstand`, `#ypo`, `#non-executive-director`, `#planungsleiter-validation`, `#post-handover`, `#sme-owner`, `#academic`, `#expert`, `#feasibility-test`, `#successor`, `#completed-successor`, `#internal-it`, `#filigran`, `#internal-network`, `#pilot-enabler`, `#knowledge-transfer`, `#mittelstand`, `#deal-mechanics`, `#technology-research` — most used 1–3 times.

### Issues

1. **04-Network/People/ notes have NO tags or frontmatter** (45 files). Decision needed: add `#contact #person` for graph filtering, or keep tagless.
2. **04-Network/Contact List.md** has no frontmatter tags. Should have at least `#network #pipeline`.
3. **Interview tag inconsistency:** Some interview tags vary (`#m-and-a` in 023 vs `#m&a` elsewhere — actually consistent; `#sme-owner` vs `#sme-founder` — minor variation).
4. **`#patterns` vs `#pattern`** — Patterns From Fieldwork uses `#patterns`; Open Questions uses `#patterns` (indirectly via inline). Consistent.
5. **`#filigran` and `#internal-network`** — appear once each (Interview 022). Single-use tags add noise; consider removing or applying to more files.

### Tags used only once
`#post-insolvency-mittelstand`, `#planungsleiter-validation`, `#completed-successor`, `#pilot-enabler`, `#feasibility-test`, `#internal-it`. Most are intentional descriptors for specific interview character. Acceptable but consider whether they aid graph navigation.

---

## 12. Superfluous Content / Archive Candidates

| File | Description | Recommended action |
|---|---|---|
| `Untitled.canvas` | Unnamed Obsidian canvas at vault root | INVESTIGATE then RENAME or DELETE |
| `Vault Audit — 2026-05-05.md` | First audit, fully superseded | KEEP (historical record) |
| `Vault Audit — 2026-05-12.md` | Second audit | KEEP (historical record) |
| `Gemini Export — Bootcamp (5H).md` | 49K-word archival; only Origin Story links to it | KEEP (archival source) |
| `Council Report.md` | Pointer to external HTML/PDF; near-orphan | KEEP (referenced from Council Verdict) |
| `One-Pager — German (v3).md` | German translation of v3 content; v3 framing is pre-fieldwork | REVISE alongside English v4/v5 (don't archive — translation is needed for German outreach) |
| `One-Pager.md` "within weeks" claim | Specific text undermines credibility per Interview 006 | EDIT (don't archive) |
| 18 thin People notes | Aneta Sikora, MaCeVi, Oskar Gieburowski, etc. | KEEP as placeholders or COMPLETE — they are pre-interview contact stubs, intentional |
| `Files/Future of European SME.pdf` | Unreferenced from any .md note | LINK from Market Data or Problem Statement if relevant; otherwise FLAG |
| Pre-fieldwork Pitch Deck slide placeholders | `[Project Name]`, `[Co-founder]`, `[Names]`, `[Accelerator]`, `[Date]` | EDIT — fill with Solcus + Wolf+Giuseppe + Vali Entrepreneurship Hub + current date |
| "Flagged for Research" table in Competitors.md | 8 stubs (Remly, Noah, Runeform, etc.) without assessment | MERGE into a separate "Adjacent companies for monitoring" subsection or fully assess each |
| Pre-Pattern-28 Product Methodology language ("structured interviews" relics) | Some inconsistency with current "campfire" framing | EDIT for consistency |

**Net assessment:** Vault is dense but not bloated. Most "thin" files have intentional placeholder roles. The most actionable cleanup is the Pitch Deck Content (placeholders + outdated stats), the One-Pager "within weeks" claim, and the Untitled.canvas mystery file.

---

## 13. Hidden Inconsistencies (cross-file)

### Name variants (same person, multiple spellings)

| Canonical name | Variants found | Where wrong |
|---|---|---|
| **Armin Struckmeier** | "Stuttmeyer", "Struckmier" | `Competitors.md` (Life Book section: "Armin Stuttmeyer"), `04-Network/People/Armin Struckmier.md` (filename) |
| **Marco Nortmeier** | "Michael Nordmeyer", "Marco Notmeyer" | `Standup — 2026-05-14.md` (Wednesday entry), `Standup — 2026-05-20.md` raw transcript uses "Notmeyer" (transcript artifact) |
| **Roland Wübbe** | "Roland Werbe" | `Standup — 2026-05-14.md` (Wednesday entry) |
| **Jochen Wermuth** | "Johann Vermut" | `Standup — 2026-05-14.md` (Outreach Priorities) |
| **Eberhard Müller-Menrad** | "Eberhard Mueller-Menrad" (ASCII) | `04-Network/People/Eberhard Mueller-Menrad.md` filename + Contact List |
| **Linus Wübbe** | "Linus Wubbe" (no umlaut) | `04-Network/People/Linus Wubbe.md` (filename); cf. Interview 021 says Wolf was introduced "via Linus Wübbe (mutual friend)" |
| **Lucas Müller-Menrad** vs "Justus Müller-Menrad" | Interview 024 says Lucas; Standup May 14 says Justus | Identity unconfirmed — same person or different? |
| **Joerg von Weiler** | "Joerg Weiler" | `04-Network/People/Joerg Weiler.md` (filename) — drops "von" |
| **Krzysztof Kwiatkowski** | "Krzysztow Kwiatkowski" | `04-Network/People/Krzysztow Kwiatkowski.md` (filename) |

### Three pillars: inconsistent vocabulary

| Doc | Pillar 1 | Pillar 2 | Pillar 3 |
|---|---|---|---|
| Problem Statement v5 | Interview methodology (campfire) | Computer-use tracking | Document scanning |
| Product Methodology | Digital Archaeology (OCR) | Passive Shadowing | Campfire Storytelling |
| Pitch Deck Content | Not explicitly numbered | | |

Order, naming, and emphasis differ across the three core docs. Reconciliation: Pattern 34 says order is domain-dependent (technical: docs first; relational: storytelling first). Make this explicit in both Problem Statement and Product Methodology.

### Vocabulary alignment

- **"Solcus" name:** Used consistently in Standups (May 14+), Week 6 1:1, Competitors (Ontora response), Product Evolution Log entries since May 14, recent MI notes. NOT in Pitch Deck (still placeholder), NOT in Problem Statement v5, NOT in CLAUDE.md project description, NOT in One-Pager.
- **"Closed-loop system":** Introduced in Week 6 1:1 and Standup May 19. Not yet in Problem Statement, Product Methodology, or Pitch Deck.
- **"Delegation-first methodology":** Standup May 20. Not yet in Product Methodology or Pitch Deck.
- **"Judgment framework capture":** Consistent across Problem Statement v5, ICP Definition v2, Product Methodology. ✅
- **"Olive tree":** Consistently attributed to Armin (Interview 017) across Pattern emerging-hypotheses, Product Methodology, Standup May 14, Problem Statement v5. ✅
- **"Campfire method":** Consistent across Pattern 28, Product Methodology, multiple interviews. ✅
- **NUK vs Novatex:** Used as "NUK / Novatex" or "NUK Novatex" interchangeably. Cosmetic.

### Quote attribution
Spot-checked: Marco's "99,9999% aber nie 100%" cited in Interview 022 as Pattern 39 confirmation — but Pattern 39 doesn't exist. The quote itself is correct from Marco's interview, but the pattern attribution is phantom.

### ICP revenue range mismatch
- ICP Definition: **€5–25M revenue**
- Pitch Deck Slide 4: **€2–20M revenue**
- Problem Statement v4 says €5-25M; v5 doesn't restate; ICP Definition v2 says €5-25M

The Pitch Deck range is stale. Fix the Pitch Deck.

---

## 14. HIDDEN CONNECTIONS — Unseen Cross-References

These are insights or reinforcements that emerge only when reading across multiple files and are not captured in any current Related section.

### Theme: The Methodology-Not-Model Moat is Triple-Validated and Has Academic Backing

**HIGH IMPORTANCE.** Three independent voices in the interview dataset (Francis 020, Marco 022, Roland 021's atrophy critique implicitly) converged on the same insight: the moat is the methodology, not the AI model. The recent `MI — Domain Expert Knowledge in AI Systems` adds academic backing (Sundberg & Holmström's three mechanisms: consolidation / algorithmic mediation / naturalization). These four sources together form a coherent theoretical-and-empirical framework that:

- Resolves Francis's Challenge 3 ("the missing middle")
- Reframes Pillar 1 of the methodology (campfire) as the "consolidation" step
- Reframes domain-specific prompting as the "algorithmic mediation" step
- Identifies "naturalization" (organisational acceptance of AI output) as the unaddressed third step

**Current state:** None of the strategy docs cite the Sundberg & Holmström framework. The Product Evolution Log doesn't have a Pivot for "consulting-practice identity confirmed by independent academic + practitioner + retiree triangulation."

**Recommendation:** Add to Product Evolution Log as Pivot 15 ("Methodology-not-model moat — academic + practitioner triple confirmation"). Reference all four sources.

### Theme: Pattern 41 Has Strong Academic Validation Not Yet Documented

**HIGH IMPORTANCE.** Pattern 41 (knowledge hoarding as job security; willingness spikes at exit) is attributed to Eberhard. But the `MI — Silver Tsunami` Kempten paper independently names "fear of losing significance" as one of the three primary social barriers to knowledge management. Same insight, two sources (one interview, one academic). Pattern 41 currently cites only the single Eberhard source.

**Current state:** Pattern 41 strength is rated "Strong — named explicitly by an experienced Mittelstand director." Could be upgraded to "Very strong" with the academic citation.

**Recommendation:** Update Pattern 41 in Patterns From Fieldwork to add `MI — Silver Tsunami and AI Knowledge Capture` (Kempten 2025) as second source.

### Theme: Pattern 27 (onboarding speed, John Lynch's "400% improvement") Has Quantified Market Confirmation

**HIGH IMPORTANCE.** John's intuition that onboarding-speed improvement is a no-brainer value driver is empirically confirmed by `MI — Silver Tsunami`: eGain platform users report **46% reduction in onboarding time for technical roles**, **38% improvement in problem resolution times**, **27% increase in first-time fix rates**. Pattern 27 currently has only the John Lynch source.

**Current state:** Pattern 27 strength: "Strong — universal logic + specific numbers from one source." Should be upgraded with eGain data as second-source quantification.

**Recommendation:** Update Pattern 27 to cite Silver Tsunami MI. This is also a strong number for the Pitch Deck (a third-party validated 46% onboarding-time reduction).

### Theme: Pattern 40 (documentation entropy) IS the Closed-Loop System Problem IS the MI — Context Farming Solution

**HIGH IMPORTANCE.** Three different framings of the same problem appear in three different files, never connected:

- **Pattern 40 (Marco, Interview 022):** Documentation decays under external system change; nachdokumentation rarely happens
- **Week 6 1:1 (closed-loop framing):** Knowledge base needs "action → measure → feedback" cycle to stay current
- **MI — Context Farming for Company Second Brain (YouTube):** Automated agents pull context from Slack/Notion/Fireflies on a schedule = the maintenance layer

These are the same engineering problem articulated as pattern, product strategy, and market practice. None of the three references the other two.

**Recommendation:** In the next Patterns From Fieldwork update, add to Pattern 40: "See `MI — Context Farming` for the proposed solution (automated context-pull agents) and Week 6 1:1 for the product framing (closed-loop system)." In Product Methodology, add a "Maintenance Mechanism" section that references all three.

### Theme: Pattern 22 (ERP ceiling) + Pattern 42 (head-of-dept sweet spot) Together Define the ICP Wedge

**MEDIUM-HIGH IMPORTANCE.** Pattern 22 says ERP captures processes but not judgment. Pattern 42 says head-of-department roles hold the transferable judgment that ERP cannot capture. Together they define the wedge precisely:

> "The ICP is the head-of-department role layer (Pattern 42) inside a Mittelstand company that has hit the ERP ceiling (Pattern 22)."

This is the most precise wedge definition possible. Neither pattern alone has this clarity.

**Current state:** Patterns 22 and 42 are not cross-referenced in either pattern's entry.

**Recommendation:** Update both pattern entries to cross-reference. Update ICP Definition v3 to lead with this combined framing.

### Theme: Three "Framing Too Narrow" Signals (016, 018, 021) Are Empirically Confirmed by MI — Domain Expert (400% YoY Vertical AI Growth)

**HIGH IMPORTANCE.** Three independent prospects told us succession framing is too narrow. The MI — Domain Expert Knowledge in AI Systems shows vertical AI growing 400% YoY — empirical market evidence that the broader "expert intelligence" framing is exactly where the market is moving. The Open Question on "framing too narrow vs go narrower" is a positioning tension that can now be resolved with this synthesis:

> "Broad applicability (the trend Vertical AI 400% YoY confirms) + Narrow proof of concept (Francis's directive). Lead with the Planungsleiter wedge; close with the broader market frame."

**Current state:** This synthesis isn't documented anywhere as a resolved position.

**Recommendation:** Add to Problem Statement v6 and Pitch Deck refresh. This is the dual-framing pitch deck strategy.

### Theme: Eberhard's "Stuck in the Middle" Insolvency (Interview 024) is the Cautionary Tale for Filigran (Interview 015) and Should Be Named

**MEDIUM IMPORTANCE.** Eberhard's eyewear business filed insolvency partly because €50M was "stuck in the middle" — too big for niche, too small for consolidation play. Filigran faces structurally identical consolidation pressure in Polish steel (per Joerg's Interview 015 framing). The "stuck-in-the-middle" framing could become a fourth urgency force in pitch materials (alongside succession, AI window, talent scarcity), but currently:

- It's an Open Question raised by Interview 024
- Not connected to Filigran's strategic reality
- Not in Problem Statement or Pitch Deck

**Recommendation:** Test "consolidation pressure" as a fourth urgency force in next 2-3 conversations with Mittelstand owners. If it lands, formalise.

### Theme: Network Folder Reveals Tribal-Context Patterns Not Documented

**MEDIUM IMPORTANCE.** Reading across 04-Network/People/ reveals connection patterns:

- **Polish cluster:** John Lynch ↔ Maciej Bogacz ↔ Joerg Weiler ↔ Grzegorz Ptak — all gateway to Polish market via different channels (YPO, M&A, family, family-uncle). Not mapped anywhere.
- **Filigran ecosystem:** Stefan Weiler (CEO) ↔ Ulrich Bauermeister (engineer) ↔ Marco Nortmeier (IT) ↔ Joerg Weiler (Polish ops, Wolf's father) — Pattern 35's three trust thresholds, but ALSO a complete operational team for the internal PoC. Not mapped as a unit.
- **YPO cluster (Joerg's network):** Armin Struckmeier, Eberhard Müller-Menrad, Thomas Maschall, Jochen Wermuth — same network, same channel, same level of relationship. Filterable as "Father's YPO" channel.
- **Wübbe-Hülscher cluster:** Roland (former CEO H&W), Karsten Böing (current CEO, not in network folder), Linus Wübbe (Wolf's friend), Leonhard Wübbe (Roland's son, pending intro). Roland's network reaches into Peter May / Hamburg Family Summit.

**Recommendation:** Either create a "Network Clusters" page in 04-Network/ mapping these, or add cluster tags (`#cluster-polish`, `#cluster-filigran`, `#cluster-ypo`, `#cluster-wuebbe`) to People notes for graph filtering.

### Theme: Life Book (Armin's lead) Is the External Validation of the MI — Storytelling SECI Externalization Quadrant

**MEDIUM IMPORTANCE.** Life Book uses structured interview methodology, now AI-integrated, to harvest life stories — exactly the operation SECI model calls "Externalization" (tacit → explicit). They sell this service at $10-20K/book. Solcus does the same operation for business knowledge at $15-25K/engagement. The methodology equivalence is precise but not documented:

- Competitors.md describes Life Book as competitor/methodology source
- MI — Storytelling describes SECI externalization quadrant
- No file says "Life Book is the for-profit operationalization of SECI externalization at a price point we should match or undercut"

**Recommendation:** Add this framing to Competitors.md (Life Book section) and to Product Methodology.

### Theme: Antler / Alan Connection (Standup May 20) ↔ 1:1 Week 6 Accelerator Strategy

**LOW-MEDIUM IMPORTANCE.** The Standup May 20 references "Alan (Antler partner)" with the maxim "founders do everything required at each moment." Week 6 1:1 mentions "Antler investors — 2-3 investors for intro and Q&A" at 3:30 PM. Standup May 19 named accelerator application as a priority. These three references are about the same accelerator network but not connected.

**Recommendation:** Confirm Antler engagement status in next Outreach Strategy update and link explicitly across these three docs.

### Theme: Pattern 41 (timing window) Partially Resolves Pattern 37 (atrophy)

**HIGH IMPORTANCE — already noted in Interview 024 file but not propagated.** Interview 024 explicitly identifies that engaging at the retirement window dissolves Roland's atrophy concern: the expert is leaving anyway; the question becomes how much judgment to preserve, not whether replication damages continued capability. This is a structural pattern-level resolution that should be documented in Patterns From Fieldwork itself, not only in Interview 024.

**Recommendation:** Update Pattern 37 in Patterns From Fieldwork: "Partially resolved by Pattern 41 — if engagement happens at retirement window, atrophy concern dissolves naturally."

### Theme: The MCP-First Phase 2 Architecture is Theoretically Grounded Across 4 MI Notes But Not in Product Methodology

**MEDIUM IMPORTANCE.** Four MI notes (Context Engineering Platforms, The AI Operating Layer, Knowledge Graphs for Enterprise AI, Domain Expert Knowledge in AI Systems) together describe the technical architecture Solcus's Phase 2 should adopt: MCP standard, temporal knowledge graphs, vertical-AI expert-intelligence layer, governance. Product Methodology mentions none of these.

**Recommendation:** Add a "Technical Architecture (Phase 2)" section to Product Methodology summarising the MCP-first / GraphRAG / Zep-temporal stack with citations to the four MI notes.

---

## 15. Recommended Action Plan (Prioritized)

### CRITICAL (errors that mislead)

1. **Resolve Pattern 39 phantom** — Either define Pattern 39 in Patterns From Fieldwork using Francis's "partial-capture honesty" language, OR rewrite all references in Interview 021, 022, Patterns 21/37 commentary, and Open Questions to make clear it's an unnumbered strategic directive. Recommended: define it as a real pattern; the cluster narrative depends on it. (File: `Patterns From Fieldwork.md`, plus all dependent references.)

2. **Fix Pattern numbering order in Patterns From Fieldwork** — Move Pattern 40 to its sequential position before 41/42. Also document the Pattern 36 gap (or add a missing pattern).

3. **Fix wrong pattern references in Interview 021 and Interview 024:**
   - Interview 021: "Pattern 8 — Long onboarding by osmosis" — this is wrong; either rename to "Pattern 27 — onboarding speed" or remove the pattern claim.
   - Interview 024: "Pattern 11 — Self-preservation knowledge hoarding" → should be "Pattern 25" (per documented renumbering).

4. **Fix Pitch Deck factual errors:**
   - ICP revenue range: change €2-20M → €5-25M (align with ICP Definition).
   - Q&A stats: 19 interviews → 24; 35 patterns → 36 (+5 MI-validated insights).
   - Replace `[Project Name]` placeholder with **Solcus** on Slide 1.
   - Replace `[Co-founder]` / `[Names]` placeholders on Slide 6 with Wolf + Giuseppe.
   - Rename Slide 5 ("What the First Interview Told Us" → "What 24 Interviews Told Us").

5. **Fix Standup 2026-05-14 name errors** — three name typos in the Week Recap table (Roland Werbe → Wübbe, Michael Nordmeyer → Marco Nortmeier, Justus Müller-Menrad — needs clarification) and one in Outreach (Johann Vermut → Jochen Wermuth).

6. **Fix CLAUDE.md folder structure** — Add `04-Network/` and `Files/` to the folder map. Update pattern count line (1-27 → 1-42 with gaps).

### IMPORTANT (structural cleanliness)

7. **Add Vault Audit — 2026-05-12 + Contact List to Home.md.** Two minor edits.

8. **Resolve four name typos in 04-Network/People filenames:**
   - `Armin Struckmier.md` → `Armin Struckmeier.md`
   - `Eberhard Mueller-Menrad.md` → `Eberhard Müller-Menrad.md`
   - `Linus Wubbe.md` → `Linus Wübbe.md`
   - `Krzysztow Kwiatkowski.md` → `Krzysztof Kwiatkowski.md`

   Update Contact List wikilinks accordingly.

9. **Fix "Armin Stuttmeyer" in Competitors.md** (Life Book section) → "Armin Struckmeier".

10. **Add 5 Interview 024 open questions to Open Questions.md.**

11. **Update Product Evolution Log** — Add Pivots 15-19 covering Interviews 020-024, Solcus name, closed-loop system, delegation-first methodology, two-track Filigran pilot, retirement-window timing.

12. **Update Problem Statement to v6** — Reflect Interviews 020-024, Patterns 40/41/42, Solcus name, methodology-not-model framing.

13. **Update ICP Definition to v3** — Add post-handover former CEO segment (021, 024), Pattern 41 timing axis, Pattern 42 cross-industry confirmation, "internal IT lead with operational authority" persona.

14. **Update Interview Guide** — Replace "Pattern 9" → "Pattern 8"; "Pattern 10" → "Pattern 22". Add three new extraction prompts from `MI — Expert Interview Design`: (a) last critical incident, (b) typical process walkthrough, (c) week-one training list.

15. **Create People note for Antonio Rizza** (Interview 008 has no Network entry). Update Karl Rohr's note to backlink to Interview 002.

16. **Resolve Eberhard / Lucas / Justus Müller-Menrad identity ambiguity** — Email Eberhard or Armin to confirm whether Lucas (Interview 024) is the same as Armin's "Müller-Menrad PwC Dubai M&A" intro.

17. **Update Patterns 22, 27, 37, 41, 42** with the cross-references identified in Section 14 (academic/MI validation).

### CONNECTIONS (newly discovered, for human review)

(All HIGH-importance findings from Section 14 — repeated here for prioritization)

18. **Methodology-not-model academic-practitioner-retiree triangulation** — Add to Product Evolution Log + Product Methodology + Pitch Deck identity slide.

19. **Pattern 41 + Silver Tsunami Kempten academic backing** — Update Pattern 41 source list.

20. **Pattern 27 + Silver Tsunami eGain 46% onboarding stat** — Update Pattern 27 source list and Pitch Deck.

21. **Pattern 40 + Closed-Loop + Context Farming** — Three framings of one problem. Add explicit connection in Pattern 40 entry, Product Methodology Maintenance Mechanism section, and Open Questions.

22. **Pattern 22 + Pattern 42 = the wedge definition** — Cross-reference in both pattern entries. Lead ICP Definition v3 with this combined framing.

23. **Framing-too-narrow vs go-narrower synthesis** — Document the resolved position ("broad applicability + narrow PoC") in Problem Statement v6 and Pitch Deck.

24. **Network cluster mapping** — Either create `04-Network/Clusters.md` mapping Polish / Filigran / YPO / Wübbe clusters, OR add cluster tags to People notes.

25. **Life Book = SECI externalization at $10-20K/book** — Update Competitors.md (Life Book section) and Product Methodology with this methodology-equivalence framing.

26. **Pattern 41 partially resolves Pattern 37 (atrophy)** — Add cross-link in Pattern 37 entry.

27. **MCP-first technical architecture** — Add Technical Architecture section to Product Methodology referencing the four MI notes (Context Engineering, AI Operating Layer, Knowledge Graphs, Domain Expert).

### EDITORIAL (judgment calls)

28. **Investigate `Untitled.canvas`** — Rename, move to appropriate folder, or delete.

29. **Move 3-5 Emerging Hypotheses to Answered** in Patterns From Fieldwork (tacit extractable, eager successors, employee resistance — all now substantially answered by Patterns 28/34/41 + MI corroboration).

30. **Move 3 Open Questions to Answered** (pre-transformation as third application — adopted; Filigran exercise framing — resolved as co-development partner; earn-out quantification — partially answered by Maciej's data).

31. **Refresh One-Pager** — Remove "within weeks" claim per Pattern 24 (3-6 month realistic timeline). Update both English and German versions.

32. **Decide on Files/ folder fate** — Link `Future of European SME.pdf` from Market Data or Problem Statement, or remove.

33. **Decide on Flagged for Research stubs** in Competitors.md — assess each or move to a separate "Adjacent companies monitoring" subsection.

### COSMETIC

34. **Add geography tags** to early Italian interviews (005, 007, 009, 011) for graph filtering consistency.

35. **Decide on People-note tag convention** — add `#contact #person` to all 45 People notes, or keep tagless explicitly in CLAUDE.md.

36. **Standardise tag plural vs singular** — `#patterns` is used consistently; spot-check for `#interview` vs `#interviews` (none found inconsistent, but verify with mass-tag list).

37. **Update CLAUDE.md project description** to mention "Solcus" as the working name.

---

## 16. Compact Vault Summary

**What the vault contains.** ~165 .md notes (excluding 00-Raw) representing the knowledge work of Wolf & Giuseppe at Vali Entrepreneurship Hub. Project: Solcus — an AI-powered service that extracts tacit, decision-making, and relational knowledge from organically grown Mittelstand SMEs in Germany/Italy/Poland. Customer-discovery phase. ~52 raw transcripts and source documents in 00-Raw; ~24 structured interview notes; 18 Market Intelligence notes synthesizing academic, industry, and practitioner research; 11 strategy docs; 8 standups; 4 weekly 1:1s; a 46-file Network folder with Contact List + per-person notes for the outreach pipeline; 2 prior audits + this one.

**State.** Methodologically converged, organisationally maturing, strategy docs lagging. The fieldwork data (24 interviews across 4 industries — eyewear, construction/precast, aluminium, textile) is rich and the 36 named patterns are well-sourced (with phantom Pattern 39 being the most consequential bug). The 18 MI notes provide strong academic backing for the methodology — three external angles (knowledge elicitation, knowledge graphs, context engineering / vertical AI) all converging on the Solcus thesis. The most important strategic ideas (Solcus name, closed-loop system, methodology-not-model identity, two-track Filigran pilot, retirement-window timing window) are documented in standups/1:1s/interviews but **not yet flowing into Problem Statement v6, ICP Definition v3, Product Methodology, or Pitch Deck.** The Pitch Deck in particular has factual placeholders and stale statistics that block external presentation.

**What 24 interviews + 18 MI notes have taught us.** (a) The ICP is precisely the head-of-department role layer (Pattern 42) inside Mittelstand companies that have hit the ERP ceiling (Pattern 22) — cross-industry confirmed in 4 sectors. (b) The extraction methodology is the moat, not the AI — Francis, Marco, Roland, and Sundberg & Holmström all independently arrive at this. (c) The market is moving toward vertical AI / expert intelligence (400% YoY) and Solcus is structurally positioned at the front of this wave. (d) The Silver Tsunami is quantified — 43% of Germany's workforce retires by 2036, $31.5B Fortune 500 attrition, 20/80 explicit-vs-tacit split, 68% of industrial companies have no KM program. (e) Knowledge hoarding is real but timing-resolvable (Pattern 41 — the retirement window of openness). (f) Three GTM angles validated: succession (Preserve & Scale), M&A (Acquire & Exit, with quantified ROI from Maciej's data: 40-60× return on €15-25K fee), pre-transformation documentation. (g) The "always-on" / closed-loop system framing addresses Pattern 40 (documentation entropy) and is the Phase 2 product evolution beyond the initial 4-6 week engagement.

**Direction.** Solcus is moving from research mode to delivery mode. Filigran is verbally-greenlit as the first internal proof-of-concept (Marco Nortmeier: "Also machen wir's"). AWW is the leading external beta candidate via Hubi's AI partner. Two-track approach (internal + external) is implicit but not yet formally documented. Mentor Day prep + Ivor Fellowship application deadline (June 2) are the immediate forcing functions for the strategy doc refresh and the Pitch Deck rebuild.

**Most urgent needs.**
1. **Define or remove Pattern 39** — the phantom cascades through four files and undermines pattern integrity.
2. **Refresh the Pitch Deck before Mentor Day (May 27)** — Solcus name, ICP revenue range, N=24, integrate two-pillar framing (broad applicability + narrow proof of concept).
3. **Update Problem Statement to v6 and ICP Definition to v3** before the Ivor Fellowship application (deadline June 2).
4. **Resolve the Pattern 41 + Pattern 22 + Pattern 42 cross-references** to give the ICP framing the precision the data supports.
5. **Map the network clusters** (Polish / Filigran / YPO / Wübbe) so the outreach pipeline becomes navigable rather than just listable.
6. **Investigate `Untitled.canvas`** at vault root.

---

## Related

- [[Vault Audit — 2026-05-12]] — prior audit (53 files); most recommendations partially implemented
- [[Vault Audit — 2026-05-05]] — first audit (38 files)
- [[Home]] — needs Contact List + May 12 audit links
- [[Problem Statement]] — v6 needed
- [[ICP Definition]] — v3 needed
- [[Product Evolution Log]] — Pivots 15-19 needed
- [[Product Methodology]] — Maintenance Mechanism + Technical Architecture sections needed
- [[Patterns From Fieldwork]] — Pattern 39 phantom + Pattern 36 gap + numbering reorder
- [[Open Questions]] — Interview 024 questions missing
- [[Pitch Deck Content]] — multiple factual fixes needed before May 27
- [[Competitors]] — Stuttmeyer typo, SAP-implementation startup missing
- [[Interview Guide]] — phantom Pattern 9 + Pattern 10 references
- [[CLAUDE.md]] — folder structure stale; pattern count stale; Solcus name missing
