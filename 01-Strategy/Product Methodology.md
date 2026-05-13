# Product Methodology

#strategy #product #core #living-document

> **Status:** Working definition — not finalized
> **Purpose:** Formalizes how we extract, structure, and deliver operational knowledge

---

## The Core Philosophy: The Neutral Mirror

We do not act as consultants. We do not tell a founder how to run his business. We hold up a mirror — documenting exactly what exists, as it exists, without judgment or recommendation.

**What this means in practice:**
- We document the reality of the business, not the ideal version
- Improvements become obvious once documentation exists — we don't have to name them
- The founder never feels critiqued; he feels understood and respected

**What we never do:**
- Name bottlenecks or inefficiencies unprompted
- Recommend changes to how the business operates
- Frame the deliverable as "here's what you should fix"

This is what makes the product sellable to a 60-year-old SME owner who built the business on instinct and would immediately reject a consultant.

---

## The Three Pillars of Extraction

### Pillar 1 — Digital Archaeology

OCR scanning and ingestion of legacy files — the accumulated paper trail of a business.

- Old invoices, contracts, and purchase orders (scanned or photographed)
- Archived PDFs and internal documents
- Physical ledgers, handwritten notes, whiteboard records
- ERP exports and legacy database dumps

The goal is to surface the documented process layer — thin as it often is.

### Pillar 2 — Passive Shadowing

Direct observation of how work actually happens day-to-day.

- Workflow tracking (how employees move through digital tools)
- Computer-use observation (what applications are used, in what sequence)
- Communication pattern mapping (email metadata, messaging tools)
- Physical floor presence and structured note-taking

**Key constraint:** Zero operational disruption. We observe the reality, not the desired state. Employees are not asked to change how they work.

### Pillar 3 — Campfire Storytelling (Conversational Extraction)

Structured storytelling sessions — not questionnaires — that surface tacit knowledge through narrative. Three independent sources (David, Joerg, Armin) confirmed that stories and anecdotes surface tacit knowledge more truthfully than structured process questioning. People hate documenting processes; they love telling stories. The exceptions, the judgment calls, the "how we do things here" — these emerge through storytelling, not flowcharts. (Pattern 28)

- "Tell me about a time when…" — not "Describe your process for…"
- Nostalgic framing bypasses defensiveness and tech fatigue
- AI transcription + synthesis: transcript → judgment framework capture
- Follow-up prompting to fill gaps identified in Pillars 1 and 2

**Sequencing depends on domain (Pattern 34):**
- *Technical-domain SMEs* (engineering, manufacturing): the normative/document layer (Standardgrundlage) must be ingested via Pillar 1 FIRST. Storytelling adds the judgment layer on top once the standard-answer capability is in place.
- *Relational/decision-heavy domains* (commercial, leadership, sales): storytelling comes first. The judgment framework IS the standard layer.

**Life Book benchmark:** YPO company that professionally harvests life stories using structured interview techniques, now integrating AI. Represents the professional quality bar for Pillar 3. See [[Competitors]].

---

## The Fourth Input: Communication Network Analysis (ONA)

Email and communication metadata → **Organizational Network Analysis**

- Maps who actually communicates with whom to get things done
- Surfaces the *informal* network (often dramatically different from the formal org chart)
- Shows centrality: which employees are the real communication hubs
- Identifies single points of failure: which people are the de facto decision bottleneck

This operates as an analytical layer across all three extraction sources, not a separate phase.

**Note:** Email metadata analysis under GDPR requires legal validation — see Open Questions below.

---

## The Deliverable: Organizational Report

The final output. Not a consulting memo. A structured asset.

**Core contents:**
- Process maps (BPMN-style "as-is" flows for each critical operation)
- Organizational network map (formal org chart vs. informal communication network)
- Role knowledge profiles (what each key employee knows; what breaks if they leave)
- Standard Operating Procedures (SOPs) — generated from combined extraction inputs
- Single-point-of-failure inventory (which operations rely on one person)

**Naming conventions:**
- "Organizational Report" — neutral, non-threatening; right for most founder-facing conversations
- "Buyer-Ready Organizational Report" — appropriate when the context is sale or succession planning
- "Information Vulnerability Map" — for investor/PE board audiences; makes knowledge concentration risk visible as a dashboard. (Source: [[Interview 019 — Lorenz Essing (EMH Partners, Germany)]])
- Avoid: "M&A Data Room," "Due Diligence Package" — banker register, triggers resistance in traditional founders

**Additional deliverable concept — Olive Tree Mapping:**
Some roles cannot be replaced 1:1 — they grew organically over 30-40 years. The olive tree deliverable maps which branches exist within an irreplaceable role and helps plan how to split the role across multiple people or systems. Concrete output: a role-decomposition plan paired with the knowledge map of each branch. (Source: [[Interview 017 — Armin Struckmeier (NUK Novatex, Germany)]])

**Timeline target:** 4–6 weeks per engagement at Phase 1 (manual). Compresses in Phase 2 as AI handles more extraction.

---

## Messaging Rules

| Avoid | Use instead | Why |
|---|---|---|
| "M&A" | "Buyer-ready" / "Valuation-protected" | "M&A" signals bankers and deal complexity |
| "Surveillance" / "monitoring" | "Passive shadowing" / "workflow observation" | Privacy and employee resistance triggers |
| "AI tool" / "platform" | "Tech-enabled service" / "done-for-you" | Founders don't want to learn software |
| "Bottlenecks" / "inefficiencies" | "How the business actually runs" | Never critique the founder's decisions |
| "Digitalization" | "Documenting your operations" | Buzzword fatigue in traditional industries |

---

## Open Questions

- [ ] Is "Organizational Report" the best final name, or does "Operations Blueprint" (from One-Pager v1) land better with founders?
- [ ] What is the minimum digital footprint required for Pillar 2 to produce meaningful data? (If a company runs entirely on paper and verbal communication, does passive shadowing fail?)
- [ ] Is email metadata analysis compliant under GDPR without explicit individual consent? What does this mean for the ONA layer?
- [ ] How do we handle employee resistance to shadowing (privacy concerns, Works Council / Betriebsrat rules in Germany)?
- [ ] Does judgment framework capture (formerly "decision replication" — see [[Interview 003 - Merih (Finance Professor)]], refined in [[Interview 011 — Dairy Chemicals Commercial (Italy)]]) belong in the core methodology, or is it a Phase 3 product extension?

---

## Related

- [[Problem Statement]] — the thesis this methodology is built to validate and deliver
- [[One-Pager]] — the customer-facing description of how we work
- [[Interview Guide]] — Conversational Extraction in operational detail
- [[Business Model]] — how the methodology maps to a revenue model
- [[Competitors]] — why our methodology works where Celonis fails (no event logs required)
- [[Origin Story]] — where the three-pillar framework was first articulated
