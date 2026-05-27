# Product Methodology

#strategy #product #core #living-document

> **Status:** Working definition — updated May 20, 2026 to reflect Interviews 020-024 and Patterns 35, 40, 41
> **Project name:** Solco
> **Purpose:** Formalizes how we extract, structure, and deliver operational knowledge

---

## Pillar Sequencing — Domain-Dependent (Pattern 34)

The three pillars are universal; the **order** in which they are applied depends on the domain:

### Technical domains (manufacturing, engineering, construction)
1. **Pillar 1 — Document/Archive Ingestion FIRST.** Normative documents, technical standards, regulations, past project archives (Standardgrundlage). The standard-answer layer must exist before the judgment layer adds value.
2. **Pillar 2 — Computer-Use Tracking.** Passive workflow observation captures how the existing standards are applied operationally.
3. **Pillar 3 — Campfire Storytelling LAST.** Judgment extraction on top of the established normative + workflow layers. Stories surface the exceptions, the "when I see X I do Y because Z" logic that lives outside the normative framework.

### Relational domains (commercial, sales, leadership, founder-decision)
1. **Pillar 3 — Campfire Storytelling FIRST.** In these domains, judgment IS the standard layer. Process documentation is thin or non-existent; the founder's interpretive framework is the operating system.
2. **Pillar 2 — Computer-Use Tracking.** Email metadata, communication patterns, decision logs supplement the narrative.
3. **Pillar 1 — Document Ingestion.** Supplements the judgment layer — past contracts, customer histories, decision artifacts.

**Source:** Pattern 34 from [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]], confirmed by [[Interview 018 — Hubertus von Huelsen (AWW, Germany)]].

---

## The Three Trust Thresholds (Pattern 35)

Extraction within an ICP-fit company follows three distinct trust thresholds. The methodology must enter at the layer of highest openness and earn access to the deeper layers over time:

1. **Technical layer (high openness)** — Domain experts (Planungsleiter, engineers, tool-making leads) share readily because they recognise the bottleneck themselves. Entry point.
2. **Commercial/operational layer (moderate)** — Operations leads, internal IT (Marco at Filigran), commercial managers. Open if the framing is value-enhancing (Personalkosten reduction, onboarding speed, ERP-gap closure).
3. **Ownership/strategic layer (protective)** — CEOs, family owners, board-level stakeholders. Protective of the business-model layer. Requires deepest trust. Activate only after technical + operational layers have produced visible results.

**Pattern 35 fully aligned at:** Filigran (Stefan Weiler + Bauermeister + Marco Nortmeier). First complete-alignment case in the dataset. Confirms the methodology.

### The Job Security Paradox
- Employees often view their undocumented, proprietary knowledge as their core value to the company (job security).
- Knowledge extraction must be framed delicately to prevent employees from feeling they will be "ditched" once their expertise is captured.
- The intervention must be framed around **delegation**, emphasizing the employee's human value rather than focusing purely on extracting their hoarded knowledge.
- *Source:* [[Interview 025 — David Richter (Suprima GmbH, Germany) — Follow-up]]

**Source:** Pattern 35 from [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]], operationally confirmed by [[Interview 022 — Marco Nortmeier (Filigran, Germany)]].

---

## Phase 2 — Maintenance Mechanism (Pattern 40)

The captured artifact decays under temporal pressure from external systems (Microsoft updates, ERP supplier changes, interface partner modifications). Nachdokumentation rarely happens. Any product must include an ongoing capture mechanism beyond the initial 4-6 week engagement.

**Phase 2 closed-loop knowledge system:**
- **Continuous meeting transcription** feeding the knowledge base (Slack, Teams, in-person meetings via voice recorders)
- **Quarterly refresh interviews** with key experts — 30-60 minutes each, structured around recent decisions and changes
- **Computer-use tracking** as passive continuous input (workflow changes, new tools, decision artifacts)
- **Scheduled re-validation cycles** — every 6 months, AI-led pass that flags stale content for human review
- **Proactive alerts** — "Key employee X gave notice → 3 knowledge clusters at risk → immediate extraction session needed"

### Architecture Validation
- SME owners independently visualize and request a technical stack consisting of a structured, markdown-based knowledge layer (e.g., Obsidian) topped with an LLM interaction layer (e.g., Claude) to query the information natively.

**Cross-references:**
- [[MI — Context Farming for Company Second Brain (YouTube)]] — automated context-pull agents from Slack/Notion/Fireflies
- [[MI — Context Engineering Platforms (Atlan 2026)]] — four-layer context architecture (orchestration / retrieval / memory / governance)
- [[1 to 1s — Week 6]] — closed-loop knowledge system framing
- Pattern 40 source: [[Interview 022 — Marco Nortmeier (Filigran, Germany)]], operationally confirmed by [[Interview 025 — David Richter (Suprima GmbH, Germany) — Follow-up]]

---

## Optimal Engagement Timing (Pattern 41)

The retirement window of openness: experts approaching retirement (2-5 year window before exit) are maximally open to knowledge extraction. Earlier engagement hits self-preservation hoarding (Pattern 25). Later engagement loses extractable knowledge to attrition.

**Screening criteria for outreach:**
- Key expert age 55-67
- Has named (even informally) a target retirement / step-back year
- 1-3 successors identified (formal or informal)
- Has experienced at least one "near-miss" event (vacation crisis, illness scare, departure of peer expert)

**Source:** Pattern 41 from [[Interview 024 — Eberhard Müller-Menrad (Eyewear Mittelstand, Germany)]].

---

## The Core Philosophy: The Neutral Mirror

We do not act as consultants. We do not tell a founder how to run his business. We hold up a mirror — documenting exactly what exists, as it exists, without judgment or recommendation.

**What this means in practice:**
- We document the reality of the business, not the ideal version
- Improvements become obvious once documentation exists — we don't have to name them
- The founder never feels critiqued; he feels understood and respected

**The "Gentle" Entry (Change Management)**
- The initial approach should rely on gentle conversation, intentionally avoiding immediate announcements of implementation or systemic change.
- This conversational "seed-planting" ensures employees feel involved from the beginning, turning them into active participants who feel ownership over the transition.

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
### Contextual Shadowing
- Theoretical interviews are often too difficult for experts who rely heavily on intuition or "gut feeling".
- The most effective elicitation method is putting the expert in their operational context and having them explain their actions while actively performing them (shadowing).
- *Source:* [[Interview 025 — David Richter (Suprima GmbH, Germany) — Follow-up]]

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
