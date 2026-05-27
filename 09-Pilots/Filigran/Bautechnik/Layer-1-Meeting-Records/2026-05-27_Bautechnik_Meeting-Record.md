# Meeting Record — Filigran Pilot, Bautechnik Session 1

#pilot #filigran #meeting-record #bautechnik

## 1. Metadata

- **Date:** 2026-05-27
- **Participants:** Wolf (SOLCO); U. Bauermeister (Bautechnik expert); M. Nortmeier (Filigran IT lead). Named but not present: Harald Frei (kiwissen.org — AI consultant found via YouTube), Jenny Frank (Filigran-internal data-protection coordinator), Scope and Focus (external data-protection firm, Hannover), Kumpor/Combro (external IT systemhouse — name garbled in transcript), Tobi (QS), Jörg / Stefan (Geschäftsleitung), the AWW Wutöschingen managing director's AI-consultant contact, Frau von Walter's household (Wolf's father called mid-meeting).
- **Duration:** 1h 10m 27s.
- **Format:** Microsoft Teams call with screen-sharing (Bauermeister shared his Vorüberlegungen document and his local Ollama setup). German.
- **Primary domain(s):** Bautechnik (with IT-infrastructure and data-protection threads).
- **Source transcript filename:** `27.05.26 Transcription - Treffen 1 Fokus Bautechnik.docx`

*Speaker labels here are more reliable than in the kickoff (Teams attribution), but treat them as indicative, not authoritative.*

## 2. Attached materials inventory

- **`SUPPLEMENT - 2026-05-26-Vorüberlegungen.docx`** — Bauermeister's one-page preliminary-considerations note (dated 2026-05-26, "UB"). *What it is:* a structured brain-dump of the questions to resolve before restarting the AI effort. *How referenced:* shared on screen at the start ("was ich damals auch als Vorüberlegung gestartet habe"). *Role:* source of facts + agenda backbone for the meeting. *Notable form:* bulleted outline covering "Welche KI ist sinnvoll für Filigran?", local language models, data sovereignty, hardware requirements, per-domain use cases (Bautechnik / Vertrieb / Produktionsplanung), *Atomisierung* (resource-light, machine-friendly storage), and workflow; ends with Harald Frey / ki-wissen.org links (Skills + MCP-server YouTube videos).
- **`SUPPLEMENT - 2025-11-25-Anleitung-llama-index.docx`** — the step-by-step guide Bauermeister followed in his failed Dec-2025 self-build. *What it is:* an AI-generated install walkthrough for **Ollama + Llama 3 8B + LlamaIndex**, ending with **Schritt 5: Vektordatenbank einrichten** (Pinecone / Weaviate / FAISS). *How referenced:* Wolf asked Bauermeister to send it ("im fünften Schritt, könnten Sie mir dieses Dokument auch mitschicken"); Bauermeister emailed it during the call. *Role:* tacit-knowledge evidence + source of facts — it pinpoints exactly where the self-build failed (vector-DB storage via Python). *Notable form:* numbered tutorial with shell/Python snippets; the failure point is the transition from working chat (Ollama/Olama) to persistent vector storage.

*Treat these as context for the meeting, not as documents to summarize in their own right. Their existence and homemade/YouTube-sourced shape is itself a tacit-knowledge signal: Filigran had no formal path to build this and improvised one.*

## 3. Executive summary

**One-liner:** Bauermeister walked through his failed Dec-2025 local-AI self-build (Ollama + LlamaIndex, which broke at the vector-database step), and the group agreed Wolf/SOLCO will research how to complete that last step and which approach/model fits, while Marco handles the binding data-protection and hardware constraints.

The session diagnosed Bauermeister's earlier attempt to build a local, data-sovereign Bautechnik knowledge base: he got Ollama running with local language models and could chat, but hit a wall at persisting documents in a vector database via Python (Schritt 5 of his guide) and gave up — "da bin ich dann gescheitert." Wolf reframed the real challenge as **Atomisierung**: chunking heterogeneous documents (PDFs, drawings, tables, photos) into context-rich *Wissensbausteine* a model can retrieve over, which is harder than dumping files into a database (otherwise "kein großer Unterschied … zum File Explorer"). The Bautechnik corpus is ~1,500 files / ~2 GB of external research reports, *Gutachten*, *Bemessungshilfen*, and test reports (*Versuchsberichte*: Durchstand, Ermüdung, Brand, Querkraft). Marco stressed that almost every downstream decision is undefined ("ganz, ganz viel Nebel") and that **data protection is the binding constraint**: Filigran's AI guideline took ~9 months, his default posture is "alles was nicht erlaubt ist, ist verboten," and any Claude/cloud use must clear internal coordinator Jenny Frank → external DPO Scope and Focus → Geschäftsleitung (a 2–4 week loop, sometimes far longer). The agreed path: finish the small win first (get Bauermeister's vector-DB ingest working, possibly with consultant Harald Frei or an AI-consultancy partnership), learn from it, then expand. Wolf to send a summary and a proposed strategy by Friday.

## 4. Thematic breakdown

### Theme A — Bauermeister's failed self-build and the real bottleneck (highest priority)
- Setup that worked: **Ollama** (local language-model interface) + downloadable models (he thinks Qwen 3 8B or **Mistral**), local chat, no data leaving the laptop ("keine Datenschutzbedenken"). Could draft English sales emails, summarize single documents.
- Where it broke: limited context memory → needs a **vector database**; populating it required **Python** (per the LlamaIndex guide, Schritt 5); he got error messages and abandoned it in Dec-2025 ("zurück auf Start").
- Wolf's reframe: the hard part is **Atomisierung** — giving each document chunk enough context that the LLM can retrieve meaningfully across formats. Brute-force file dump ≈ a searchable folder; the value is the structured context layer.
- Bauermeister's counter: an intermediate step — have the model pre-summarize each document into machine-readable top-down tables/lists — is more storage-efficient and searchable, but doesn't scale to a 150-page *Tonkalenderbeitrag*.
- *Action:* SOLCO to research how to complete the vector-DB ingest + which model/tools fit; bring 2–3 approaches to the next meeting. Owner: Wolf (+ Gigi). Deadline: summary by Friday 2026-05-29.

### Theme B — The Bautechnik corpus (source-of-facts)
- ~1,500 files / ~2 GB (roughly half is *Bemessungsprogramme*, which can be excluded). Document types: external research/test reports (*Versuchsberichte* — Durchstand, Ermüdung, Brand, Querkraft; text + drawings + many photos describing test setup and failure mode), *Gutachten* (similar + how it is dimensioned), *Bemessungshilfen* (formulas, diagrams, big number tables). Reports are produced **externally at universities**, not in-house QA.
- Distinct from daily QA tests (tensile / surface-rib measurements documenting consistent product quality for DIN purposes).
- Key property: Filigran runs tests on things they *don't* already know ("wir überprüfen üblicherweise Sachverhalte, von denen wir nicht wissen, wie sie funktionieren") — so the archive is genuinely irreplaceable, not reproducible cheaply.
- *Action:* SOLCO + Gigi to research how to break down/atomize these mixed-format documents (text, drawings, tables, photos) — likely multiple models for different parts. Owner: Wolf + Gigi. Deadline: next meeting.

### Theme C — Data protection as the binding constraint (high priority)
- Marco's posture post-AI-guideline: "alles was nicht erlaubt ist, ist verboten." He has already **banned** AI transcription and Adobe auto-PDF-summarization pending review.
- Approval chain for Claude/cloud use: **Jenny Frank (internal coordinator) → Scope and Focus (external DPO, Hannover) → Geschäftsleitung (Jörg/Stefan)**, typically 2–4 weeks, "darüber hinaus" possible. The AI guideline itself took ~9 months.
- Specific concerns: where Claude's servers sit (US / "über den großen Teich"), AVV (Auftragsverarbeitungsvertrag), GDPR, NIS2 (Filigran currently *not* in scope, fortunately), accidental ingestion of personal data (e.g. birthdate in an old list) and how to delete it once in the store.
- Wolf's takeaway: invaluable real-world context on the **approval friction** that distinguishes a two-student pace from an enterprise pace.
- *Action:* Marco to progress the data-protection review (license costs, hosting, what's permissible) and document everything. Owner: M. Nortmeier (with Jenny Frank / Scope and Focus). Deadline: 2–4 weeks, open.

### Theme D — Build vs partner; consultant options
- Options surfaced: (1) **Harald Frei / ki-wissen.org** — the YouTube tutorial author, offers paid consulting, has handled ingestion/automation and Claude "Skills"; (2) the **AWW Wutöschingen** managing director's ex-classmate at an AI consultancy (joint 3-way meeting pending); (3) **KI-Allianz Baden-Württemberg** network for partner matchmaking; (4) **Amber Search** — an existing finished product, but priced at ~50 licenses, too big for Filigran's handful of Bautechnik users.
- Wolf's strategic preference: not a normal pay-per-hour consultancy but a **partnership** to co-build, because the local context-layer-per-company concept "gibt es noch nicht" and SOLCO wants to develop it (and its own Obsidian-based platform) across domains.
- *Action:* SOLCO to contact AI consultancies / the AWW contact / KI-Allianz BW and explore a partnership. Owner: Wolf. Deadline: open.

### Theme E — Hardware / hosting
- Local models need GPUs; SSD is too slow ("alles über Grafikkarten"). Marco: current server architecture can't take the GPUs — would need new server hardware or a dedicated second server; Kumpor/Combro (IT systemhouse) would scope and supply it. A dry cellar room is available.
- *Action:* Marco to size requirements once the use case is firmer and engage Kumpor/Combro. Owner: M. Nortmeier. Deadline: once dimensioning is known.

## 5. Decisions made

- **Finish the small win first: complete Bauermeister's vector-DB ingest and test whether it is useful before broadening.** Rationale (Marco): maybe "90% schon abgeschlossen," low data-protection risk for non-personal technical docs, and it produces a real learning either way. Supersedes: starting many domains in parallel.
- **SOLCO/Wolf owns the research on the ingest method and model selection; Bauermeister sets his attempt aside** to avoid duplicated effort ("das reicht, wenn es einer tut").
- **One model, not many, for Filigran** — because Marco has to administer/support it. Rationale: supportability + data-protection. 
- **Whatever is chosen must be data-protection-compliant** and clear the Jenny → Scope and Focus → Geschäftsleitung chain.

## 6. Open questions and unresolved items

- How to complete Schritt 5 (vector-DB storage) — the exact technical blocker.
- Which model/approach fits (Mistral? Qwen? something multimodal that reads drawings/tables/photos, not just text).
- How much manual effort atomization requires per document type — "muss man genau mal ausprobieren."
- Whether to engage Harald Frei, an AI-consultancy partnership, or KI-Allianz BW — and on what commercial basis.
- Hardware dimensioning (GPUs, new server) — unknown until the use case is firm.
- Whether Claude/cloud will be approved at all by Scope and Focus given US server location.
- Data-deletion mechanics (GDPR) for anything accidentally ingested.

## 7. Tacit-knowledge signals

- *"da bin ich dann gescheitert"* — U. Bauermeister. Domain: Bautechnik / AI build. Why: the precise failure point (vector-DB storage) of a motivated internal expert's self-build — the strongest possible evidence that the atomization step is the hard, value-bearing part.
- *"wir überprüfen üblicherweise Sachverhalte, von denen wir nicht wissen, wie sie funktionieren"* — U. Bauermeister. Domain: Bautechnik. Why: the archive documents genuinely novel, non-reproducible knowledge — high stakes if lost.
- *"alles was nicht erlaubt ist, ist verboten"* — M. Nortmeier. Domain: IT / governance. Why: the default-deny posture that gates every AI step; the real adoption bottleneck.
- *"das K.I. Richtlinie wurde letztes Jahr im Sommer angestoßen … hat ein Dreivierteljahr gedauert"* — U. Bauermeister. Domain: governance. Why: quantifies the institutional speed of AI adoption in a Mittelstand (~9 months for a policy).
- *"die fehlenden Brandschutzversuche … das hat uns 20.000 gekostet"* (recurring) — running gag continued from the kickoff. Domain: Bautechnik. Why: the canonical forgotten-experiment pain, now self-sustaining inside Filigran's own conversation.

## 8. Vocabulary watch

- **Project vocabulary that appeared:** Atomisierung, Wissensbausteine (knowledge blocks), Wissensarchivierung / Wissensdatenbank, Kontextschicht (context layer), Second Brain (implied via Obsidian), MVP (not used).
- **Partner-specific / technical terms:** *Versuchsberichte* (test reports), *Gutachten* (expert opinions/assessments), *Bemessungshilfen* (design aids), *Bemessungsprogramme* (design software), Durchstand-/Ermüdungs-/Brand-/Querkraftversuche (punching-shear / fatigue / fire / shear-force tests), *Montagezustand* (installation/assembly state), *Tonkalenderbeitrag* (a 150-page reference-yearbook article), *Atomisierung*, AVV (Auftragsverarbeitungsvertrag), NIS2, *Datenschutzbeauftragter* / *Datenschutzkoordinatorin*.
- **Tools named:** Ollama (transcribed "Olama/Alama"), Llama 3 8B, LlamaIndex, Qwen 3 8B, Mistral, Notebook LM, Docker, FAISS/Pinecone/Weaviate (vector DBs), Claude (+ Claude "Skills", MCP server), Amber Search.

## 9. Methodological observations

- **(a) Extraction-methodology learnings:** This session is itself an extraction artifact — the failed-self-build narrative is exactly the kind of tacit "we tried and hit a wall here" knowledge SOLCO captures. Confirms the **documentation-first, AI-later** sequencing (Marco explicitly preferring to finish the concrete ingest and learn). Confirms **Atomisierung / Wissensbausteine** as the client-facing name for the core technical value — and that brute-force file dumping is explicitly *not* the product.
- **(b) Vault/structural implications:** Strong support for the per-domain split and for the SUPPLEMENT-as-attachment convention. The data-protection approval chain is a recurring, generalizable constraint that may warrant a research-vault pattern (see Cross-references). The "one model, supportable by one internal admin" constraint shapes any future productization.

## 10. Operational hand-off

**Filigran-side actionables:**
- Set the Bautechnik self-build aside to avoid duplicated effort; await SOLCO's research. Owner: U. Bauermeister. Deadline: next meeting.
- Progress the data-protection review (license cost, hosting, permissibility) and document all guideline changes. Owner: M. Nortmeier (with Jenny Frank → Scope and Focus). Deadline: 2–4 weeks, open.
- Send the LlamaIndex guide (Schritt-5 document) to Wolf. Owner: U. Bauermeister. Status: done during the call.
- Size GPU/server requirements and engage Kumpor/Combro once the use case is firm. Owner: M. Nortmeier. Deadline: open.

**SOLCO-side actionables:**
- Research how to complete the vector-DB ingest; evaluate Ollama, Notebook LM, alternative models/tools (incl. multimodal for drawings/tables/photos); prepare 2–3 approaches. Owner: Wolf + Gigi. Deadline: next meeting.
- Send a written summary + proposed strategy. Owner: Wolf. Deadline: Friday 2026-05-29 ("heute, morgen oder spätestens Freitag").
- Explore AI-consultancy partnership (AWW contact, KI-Allianz BW, possibly Harald Frei). Owner: Wolf. Deadline: open.
- Schedule the next Bautechnik working session. Owner: Wolf. Deadline: next week.

## 11. Cross-references and gaps

- **Continues from:** [[2026-05-22_Kickoff_Meeting-Record]] (the cross-domain kickoff, where Bautechnik was chosen as the first build).
- **Attachments:** the two SUPPLEMENT files in `_Raw/` (Vorüberlegungen; LlamaIndex guide).
- **Research-vault links:** the pain and people originate in Interview 014 (Bauermeister's €20K / failed self-build), Interview 022 (Marco Nortmeier), Interview 016 (Bergerhoff).
- **Candidate new research-vault pattern (for the user to add in Obsidian — see summary):** the *data-protection approval chain as a sales-cycle gate* in regulated Mittelstand.
- **Notable absences / gaps:** no resolution on the technical blocker (deferred to SOLCO research); Vertrieb and Produktionsplanung not advanced; Geschäftsleitung (Jörg/Stefan) sign-off on Claude still pending; the AWW 3-way consultancy meeting still unscheduled.

---
*Source transcript and attachments live in `09-Pilots/Filigran/_Raw/` (immutable). This record is a synthesis, not a verbatim transcript.*
