# Competitors

#research #strategy #competitive-landscape #living-document

> Update as new companies are discovered or positioning sharpens.

---

## The Positioning Frame

We are not a process mining tool. We are not a management consultancy. We are not an ERP vendor. The competitive landscape only makes sense when viewed through the lens of what we actually do: **extract tacit knowledge from organically grown SMEs and experts that comes along with them**

Most tools in this space were built for enterprises with digital event logs. Most services were built for large-company budgets. The gap is the market.

---

## Primary Competitive Reference: Celonis

**Why Celonis matters:** They are Germany's first "Decacorn" (>$10B valuation) and the global leader in process intelligence. Judges, investors, and industry contacts will always ask about them. Understanding Celonis is mandatory.

### Origin Story
Founded in 2011 by three TU Munich students: Bastian Nominacher, Martin Klenk, and Alexander Rinke. Their first insight: companies' IT systems automatically create "digital footprints" (event logs with timestamps) every time a process step is completed. They built software to read those logs and automatically map processes — an academic technique called **Process Mining**.

Their first major customer was **Siemens**. They bootstrapped for 5 years out of a Munich apartment before their first major funding. Today, a third of DAX companies use Celonis. Early business model: multi-million euro B2B enterprise software licenses.

### Why Celonis Cannot Serve Our Market

Celonis's entire technology relies on one fundamental assumption: **the company must have digital event logs**. Process mining requires that every task generates a Case ID, Activity Name, and Timestamp in a connected digital system (typically SAP or Oracle ERP).

Traditional organically grown SMEs do not have this. Their processes run on:
- 30-year-old intuition and habit
- Paper invoices and physical ledgers
- "Shadow IT": WhatsApp groups, personal Excel macros, informal email threads
- Verbal instructions across the warehouse floor

**Celonis cannot read a whiteboard. Celonis cannot interview a 30-year warehouse manager. Celonis cannot extract knowledge that never left someone's head.**

### Why They Won't Pivot to SMEs

Celonis is currently focused on "Enterprise AI" for Fortune 500 supply chains — moving further *upmarket*. To serve our customer, they would need to:
1. Abandon their core technology (event log mining)
2. Rebuild their entire stack for unstructured, analog, human data
3. Redesign their unit economics for €5–20M revenue companies vs. global enterprises

Enterprise software companies do not pivot backward into messy SME markets.

### How to Use This in a Pitch

When asked: *"Have you heard of Celonis? Aren't they doing this?"*

> *"Yes, Celonis is an incredible role model — they prove that unlocking process transparency is a multi-billion-euro market. But Celonis is built for Fortune 500 companies with perfectly integrated SAP systems and digital event logs. Our customers — organically grown European SMEs facing the succession cliff — don't have event logs. Their processes live on paper, in emails, and in the founder's head. Celonis cannot read that. We can. Celonis is for the enterprise whose processes live in servers. We're for the SME whose legacy is trapped in its people."*

---

## Decision Replication / "Clonable" Category

**Clonable** — US startup (identified via [[Interview 003 - Merih (Finance Professor)]]). Works in a similar space but with a sharper technical ambition: not just documenting processes, but **replicating the decision-making expertise itself** — cloning how an expert thinks, not just what they do.

- Conceptual shift from "documentation" to "decision replication"
- Possibly the US competitor raising $5.4M flagged in [[1 to 1s — Week 3]]
- Status: needs deeper research (funding, model, pricing, what they actually built)

**Our position vs. Clonable:** We are currently a documentation product (Neutral Mirror). Decision replication is a potential Phase 3 direction — see [[Interview 003 - Merih (Finance Professor)]] for the "decision replication" framing. Clonable is worth tracking as a technical reference, not yet a direct competitor at our target SME size.

---

## Process Mining Tools (Enterprise, named by Carl in [[Interview 002 - Ex-Banker, BoD of Deutsche Bank, SMEs view]])

| Company | Category | Why it doesn't serve our market |
|---|---|---|
| **Celonis** | Pure process mining | See above |
| **Fluxicon** | Pure process mining | Same event-log dependency as Celonis; smaller |
| **Workfellow** | Process intelligence + automation | Enterprise-grade; requires digital infrastructure |
| **Lucidchart** | Process mapping and visualization | Tool for people who already know their processes; doesn't extract anything |
| **Kissflow** | Workflow automation | Requires structured digital workflows to exist first |
| **Adonis** | Business process management | Same limitation — requires existing formal processes |

Carl's own assessment: *"I am unable to tell you in how far they are realistically applicable for SMEs."* If an informed ex-Deutsche Bank executive doesn't know whether these tools scale down to a 30-person manufacturer, the SME owner certainly doesn't.

---

## Knowledge Graph / Enterprise Knowledge Platforms

These are further from our product but worth monitoring as the market matures:

- **Galaxy by Stardog** (https://www.stardog.com/) — Enterprise Knowledge Graph platform; heavy infrastructure play; enterprise-only
- **eccenca Corporate Memory** (https://eccenca.com/) — Knowledge graph for governed, machine-readable semantic knowledge management; enterprise compliance focus
- **Palantir Foundry** (https://www.palantir.com/platforms/foundry/) — AI-powered operations and object-centric knowledge graphs; government and Fortune 500 scale; far too large for SME market
- **Salesforce Data 360** (https://www.salesforce.com/eu/data/guide/?d=afx) — CRM-adjacent data platform; needs review for SME relevance

None of these are direct competitors. They all assume structured data infrastructure that our market doesn't have.

---

## Management Consultants (Indirect Competitors)

McKinsey, Roland Berger, BCG — traditional management boutiques.

- Too expensive (multi-hundred-thousand-euro engagements)
- Disruptive to operations (weeks of interviews, team on-site)
- Tell founders what they're doing wrong — triggers ego resistance
- No AI-enabled efficiency; all human hours

Our differentiation: passive (not disruptive), neutral (no recommendations), fast, and a fraction of the cost.

---

## Direct AI-for-SME Consultancies (Closest Competitors So Far)

This is the most direct competitive category surfaced to date. These are firms positioning AI as a service for mid-market SMEs in our geography — not enterprise process mining, not management consulting, not ERP. They occupy adjacent space to ours.

### Omnivisor

**Surfaced via:** [[Interview 006 - John Lynch (Lynka)]]. Lynka has been in active conversation with them; they have proposed concrete AI projects but Lynka has not yet pulled the trigger.

**What we know:**

| Detail | Value |
|---|---|
| Founder | Radek Miszkont |
| Location | Warsaw, Poland |
| Approximate revenue | 2–4M PLN/year (under €1M) |
| Team | Small (fewer than ~10 estimated) |
| Customer profile | Small/medium enterprises in CEE |
| Positioning (per John) | "Find very concrete ways to help you save money using AI" |
| Founder background | Several previous startups |
| Sales approach | "Very impressive, good sales approach" — direct, in-person, conference-led |

**How they reached Lynka:** Met John at a conference; John invited them to visit; they proposed projects on-site. This mirrors a sales motion we should learn from.

**Why this matters:**
- **Same problem space.** Per John: *"They're kind of doing something in the same sphere as what you're talking about, but more in AI."*
- **Same geography.** Poland-based, serving Polish/CEE SMEs — directly overlapping our potential wedge if we expand east.
- **Same buyer.** Lynka, a digitally mature mid-market SME, is exactly the kind of company they court — and exactly the kind we are still calibrating against.
- **Already in the market.** Not a stealth startup or a thesis. They have a sales motion, a pitch, and active prospects.

**What we don't yet know (priority research):**
- [ ] What is their actual deliverable? Implementation? Strategy? Software?
- [ ] What is their pricing model and price range?
- [ ] What is their close rate? How many of their proposals like Lynka's actually convert?
- [ ] Do they target succession / M&A readiness, or pure cost reduction / efficiency?
- [ ] Do they capture tacit knowledge or work above the existing system layer?
- [ ] Are they software-led or services-led?

**How to research them:** Start with their website, LinkedIn, Radek Miszkont's profile and prior ventures. Consider an introductory conversation if positioning becomes clearer.

**Provisional differentiation (to validate):** Omnivisor appears to be a generalist AI-for-SME consultancy focused on cost savings and process improvements. Our wedge is more specific — the tacit knowledge and decision-making layer that survives ERP, framed around succession and M&A readiness rather than efficiency. But this differentiation is not yet validated and may collapse on closer inspection.

---

## ERP Vendors (Adjacent, named by [[Interview 006 - John Lynch (Lynka)]])

SAP, Microsoft Dynamics, Sage. They systematize transactions and workflows — but only what's already understood and digital.

**The ERP ceiling:** A company can spend millions on ERP and still have all its critical knowledge in the founder's head. ERP captures processes. We capture expertise.

- "ERP captures your processes. We capture your expertise." — potential positioning line

---

## Flagged for Research (Giuseppe's list)

These were flagged by Giuseppe as potentially relevant. Each needs a category assessment and positioning note before they can be properly placed above.

Search terms to investigate: **"Institutional memory"**, **"AIOS" system**

| Company                 | URL                            | Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----------------------- | ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Remly**               | https://remly.it/              | Remly is a software company that provides a file search and knowledge management tool for teams and individuals. It allows users to search files such as documents, spreadsheets, images, and code by content. The platform includes a feature that answers questions based on stored files and connected tools. It connects with services like cloud storage,<br><br>messaging, and email to gather data in one place. The system indexes files on the user’s device to enable search without uploading data. It provides keyboard shortcuts to access search across files and apps from one interface. The service includes file syncing, indexing, and secure access to stored information.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Noah support**        | https://noah.support/          | In 24 hours, noah interviews your entire team, analyses every pain point, and delivers a ranked list of AI opportunities, with the time and cost savings to back each one up. Not as a one-off report. As a living overview that stays current as your company and the market change.<br>https://youtu.be/W0uoEc5DUSI                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Runeform AI**         | https://www.runeform.ai/       | Runeform is the semantic reasoning infrastructure beneath agentic AI — a workspace where domain experts design, version, and deploy the ontologies that constrain agent behavior, at query-time speed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Simplyasking**        | https://simplyasking.io/       | **Disclaimer: this could be only a landing page and not actually a product**<br><br>A living map of what your company knows.<br>1. Knows what you don't.<br>Automatically detects gaps in your knowledge base. Drafts content to fill them before your team even asks.<br><br>2.Knowledge where people are.<br>Branded Knowledge Stations bring answers to the floor, the counter, and the field. Tap to ask, talk to know.<br><br>3. An agent grounded in your docs.<br>Customer-facing AI that answers from your actual policies. Cites sources. Escalates when it should.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Useyourbrain**        | https://www.useyourbrain.io/   | **Disclaimer: this could be only a landing page and not actually a product**<br><br>Your company's memory. Structured, versioned, and always in context.<br><br>Company Brain is a persistent knowledge infrastructure layer. It captures everything your company knows: decisions, strategies, context, relationships. It makes everything queryable, versioned, and accessible to the right people at the right time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Memory intelligence** | https://memoryintelligence.io/ | 01 · CAPTURE<br>Put something in. A note, a document, a meeting, a decision. MI™ ingests it, structures it, and gives it a cryptographic receipt so you can always prove it existed exactly as written.<br><br>02 · ASK<br>Query your data in plain language. Not keywords. Not file names. Ask what you actually want to know and MI™ finds the answer across everything you have ever captured.<br><br>03 · VERIFY<br>Prove it. Every memory has a three-part hash chain: a fingerprint of the exact words, a fingerprint of the meaning, and a combined chain hash. If anything was changed, the hash will not match. If it matches, nothing changed.<br><br>04 · EXPLAIN<br>See inside the machine. Explain shows you exactly what MI™ understood when it processed a memory: entities extracted, relationships mapped, quality scores assigned. No black box. Full transparency at every stage.<br><br>05 · FORGET<br><br>Remove it. Completely. And get a receipt proving the removal happened at a specific timestamp. You can prove something was deleted without having to keep the thing you deleted. For regulated environments, this is essential. |
| **Runlog AI**           | https://www.runlogai.com/      | Read everything you have<br>PDFs, docs, decks, spreadsheets, audio, video. Atlas takes it all in. Every page, every slide, every message your team works from.<br><br>Build a living picture<br>Atlas maps every customer, contract, deal, and relationship. New information updates everything connected to it. The picture stays current on its own.<br><br>Power the work you do<br>Your team gets answers, scored shortlists, and finished documents. Each output links back to its source. Each portal we build fits the way your team works.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Nexindex**            | https://nexindex.io/           | Document Intelligence<br>Extract signals from contracts, proposals, and emails — not just CRM fields. Surface risks, obligations, and insights no manual entry could capture.<br><br>Custom AI Workflows<br>Build autonomous agents that scan pipelines, draft briefs, and deliver insights on schedule — your AI Chief of Staff.<br><br>Knowledge Graph<br>A compounding intelligence layer that maps people, deals, and documents — growing smarter with every interaction.<br><br>Zero Data Entry<br>One-click sync with Dropbox, OneDrive, SharePoint, Outlook, and Slack. Intelligence from docs and conversations you already have.<br><br>Team Knowledge<br>Share knowledge with role-based access. When someone leaves, their intelligence stays.<br><br>                                                                                                                                                                                                                                                                                                                                                                                              |


---

## Life Book (YPO Company)
- **What they do:** Professionally interview people and write their life stories as physical books. Now integrating AI. Mostly wealthy Americans.
- **Founded by:** Roy Moer (sp?)
- **Pricing:** $10,000-20,000 per book
- **Relevance:** They have already solved "how to harvest stories efficiently" — the exact extraction methodology we need. Their interview technology is the professional implementation of Pattern 28 (campfire method).
- **Relationship:** Armin Struckmeier's sister-in-law Andrea manages it. Armin offered to connect us.
- **Threat level:** Low as direct competitor (they make books for individuals, not business knowledge systems). High as methodology source or partner.
- **Source:** [[Interview 017 — Armin Struckmeier (NUK Novatex, Germany)]]

**Methodology equivalence:** Life Book is the for-profit operationalisation of what knowledge management theory calls "SECI Externalization" (tacit → explicit). They sell this at $10-20K/book. Solco does the same operation for business knowledge at €15-25K/engagement. The methodological parallel is precise — both use structured interviews to harvest experiential knowledge. The difference: Life Book captures life stories; Solco captures business judgment frameworks. (See [[MI — Storytelling and Tacit Knowledge Capture]] for SECI model context.)

---

## Ontora (YC-backed, AI-led employee interviews)

- **Website:** ontora.com — "Read your company like a book"
- **What they do:** Deploy AI agents that interview every employee simultaneously, then synthesise the results into an operational knowledge base — a live map of how work actually happens, where it breaks, and what to fix first. Deliverable includes themed insights, process maps, and an automation roadmap with ROI prioritisation.
- **YC-backed:** Yes — listed on YC launch page (W/S 2025 or S2026 cohort based on discovery date)
- **Model:** AI-led interviews at scale (all employees, parallel); emphasis on speed ("within hours"); focus on operational workflow visibility and automation readiness — not succession
- **How they differ from Solco:**
  - They interview ALL employees (breadth); we go deep on the founder/expert (depth)
  - Their output is a process/automation map; ours is a queryable knowledge brain with tacit context
  - Their AI leads the interviews; ours uses human facilitation (campfire method) because tacit knowledge requires trust and narrative, not structured Q&A
  - No succession angle — they are an operational intelligence product, not a knowledge transfer product
  - Likely targeting tech-adjacent mid-size companies, not Mittelstand manufacturing SMEs
- **Threat level:** Medium-High. The positioning is very close (AI-driven company knowledge extraction). If they pivot toward knowledge transfer or succession use cases, or if they develop a human-facilitated track, the overlap becomes significant.
- **Pitch response when asked:** *"Ontora interviews employees to map operational processes — they're excellent at discovering workflow bottlenecks. We extract the non-verbalisable, non-documentable knowledge that lives only in the expert's head: the judgment, the relationships, the heuristics built over 30 years. That knowledge doesn't surface in a structured AI interview — it requires storytelling, trust, and time. Ontora can read a company. We capture what can't be read."*
- **Source:** Wolf's research, May 2026 — [[1 to 1s — Week 6]]

---

## SAP-Implementation Knowledge-Capture Startup (unnamed, €3.5M raised)

**Surfaced via:** [[Interview 024 — Eberhard Müller-Menrad (Eyewear Mittelstand, Germany)]] (Wolf referenced this in conversation)

**What we know:**

| Detail | Value |
|---|---|
| Funding | €3.5M raised |
| Target customer | Consulting firms running SAP transformations |
| Product | Knowledge capture for SAP implementation methodology — which questions to ask, which decisions to make, how to structure the transformation |
| Long-term direction | Skip the consultants; tools direct to enterprise |

**Why this matters:**
- Same problem space (capturing expert methodology), different wedge (consulting firms vs SMEs)
- Funded knowledge-capture startups exist — validates the category
- The 4-week-engagement structure of SAP transformations is structurally similar to our Phase 1
- Not a direct competitor today (different ICP, different deliverable), but worth monitoring if they expand into mid-market direct sales

**Action:** Research the company name and current product. Add to "Flagged for Research" if identified.

---

## Convergent Pressure: Vertical AI / Expert Intelligence Platforms

The most strategically important market signal from MI research: **vertical AI solutions are growing 400% YoY** ([[MI — Domain Expert Knowledge in AI Systems]]). Companies like Intuit's $1.4B expert intelligence platform, Anthropic's Claude Use API ([[MI — The AI Operating Layer (Anthropic, Google, VentureBeat)]]), and the context engineering platform category ([[MI — Context Engineering Platforms (Atlan 2026)]]) are all converging toward the same insight Solco is built on: **domain expertise + AI architecture > general-purpose models.**

**Where competition is coming from:**
- **Enterprise AI infrastructure (Atlan, Zep, Mem0, Letta)** — context engineering platforms that assume the company already has digital data to ingest. They don't extract from people; they organise what's already digital. Solco operates upstream of where they start.
- **Computer-use AI (Anthropic Computer Use, Google DeepMind, Clicky YC):** screen-resident agents that observe workflows. Parallel to our Pillar 2 (computer-use tracking) but they aim at task execution, not knowledge extraction. Will eventually overlap with Solco's Phase 2 (always-on observation).
- **Big 4 AI consulting practices:** McKinsey/BCG/Deloitte/EY/PwC are all building "AI for Mittelstand" lines. Their disadvantage (per Francis de Vericourt's argument): they cannot get the trust of a Mittelstand founder. Solco's moat is access + methodology, not technology.

**Positioning:**
Solco is structurally positioned at the front of the vertical AI wave but addresses the layer that pure AI infrastructure cannot reach — the human expert whose knowledge has never been digitised. The vertical AI category is the rising tide that lifts our boat; the enterprise AI platforms are not direct competitors but the architecture we will eventually integrate with.

---

## Construction-Vertical AI Platforms (Adjacent / Convergent Signal)

Four construction-vertical AI platforms surfaced in May 2026 desk research. None target SME succession or knowledge transfer — they are project management / document intelligence plays for the AEC industry. They matter to us as a **parallel-industry signal**: the same thesis (organisational knowledge trapped in fragmented tools → AI agents to extract and structure it) is being funded and shipped in a neighbouring vertical, with similar language ("AI brain", "Cognitive Intelligence Layer", "Knowledge and Insights"). Treat as convergent-pressure evidence, not direct competitors. Useful reference for: GTM patterns, agent architecture, pricing anchors, and the "vertical AI 400% YoY" trend ([[MI — Domain Expert Knowledge in AI Systems]]).

### Klutch (Seattle, US)

**Source:** GeekWire article (June 2025), `00-Raw/Klutch.md`. Website: klutch.ai.

| Detail | Value |
|---|---|
| Founders | Xu Rui (CEO, ex-Stripe ML), Tanin Na Nakorn (ex-Stripe ML) |
| Funding | $8M seed (June 2025) — Bling Capital + Bain Capital Ventures lead; Brick and Mortar Ventures, Original Capital, Anthology Fund, Autodesk + BuildZoom angels |
| Team | 12-person team (software engineering + structural/civil engineering) |
| Target customer | Mid-sized residential and commercial builders / GCs ($20–250M annual construction volume) |
| Product | Named AI agents (Archie = permits/zoning, Bob = jobsite data capture, Petra = vendor scoring, Hailey = warranty). Standalone construction management system OR layer on top of existing PM tools. |
| Distribution channel | WhatsApp, SMS, email — agents live in the interfaces field workers already use |
| Output | "Ongoing company-wide knowledge vault based on information the agents gather" |
| Positioning | "Compound startup" (Bling investor frame; Rippling / Palantir / Salesforce comparable) |

**Why this matters to Solco:**
- **Same thesis, different industry.** "Construction teams have huge amounts of data that isn't being used" → identical pattern to Pattern 31 (Bauermeister's failed self-build, €20K-per-forgotten-experiment) but applied to project-level construction data, not generational founder knowledge.
- **Native-interface distribution.** WhatsApp/SMS/email as agent surface is the closest analogue we have seen to Pattern 22 (founder knowledge lives in informal channels). They built FOR that channel rather than trying to migrate users off it.
- **Knowledge vault as side effect.** Their core product is workflow automation, but they generate a "knowledge vault" as a by-product. Mirror image of Solco, where knowledge extraction IS the product and workflow improvement is the by-product.
- **Funding anchor.** $8M seed for "AI coworkers in construction" sets a vertical-AI seed benchmark for adjacent verticals (incl. ours).

**Differentiation vs Solco:** Klutch optimises **active project execution**. Solco extracts **non-transferable expert judgment** before/during a generational handover. Different time horizon, different buyer (project manager vs founder/successor/PE/M&A), different deliverable.

---

### Trunk Tools (US)

**Source:** trunktools.com landing page, `00-Raw/Trunk Tools.md`.

| Detail | Value |
|---|---|
| Target customer | General contractors and their trade partners on large-scale projects |
| Positioning | "The Brain Behind Construction" — "one giant construction brain dedicated to your workflows, your documents, your project" |
| Product modules | TrunkSubmittal (discrepancy detection in spec/submittal review), TrunkReview (drawing revision agent — vision-language models), TrunkText (Q&A over project docs), TrunkRFI (RFI management + dedup), TrunkBid (bid analysis), Submittal Register |
| Buyer pain | "Document hunt consumes a large portion of the workday for Project Managers and Superintendents" — same time-loss frame as [[MI — Why Now Is the Knowledge Management Moment (Atlassian)]] (25% of workweek lost to search) |
| Pricing | Not public |
| Free tool | "Contract Review Agent" as lead magnet |

**Why this matters to Solco:**
- **"Construction brain" is the strongest language convergence so far** with our Solco / "company brain" framing ([[MI — Company Brain Concept (Ability.ai, Falconer, YC)]]). Different vertical, same metaphor.
- **Free contract review agent as wedge.** GTM lesson: a single high-value, low-risk free deliverable creates pull. Direct parallel to our possible Filigran-style first-deliverable wedge.
- **Construction-centric AI vs general AI.** Explicit positioning: "Unlike broader AI tools, TrunkText is laser-focused on construction and trained specifically on your project's data." Same vertical-vs-general argument that [[MI — Domain Expert Knowledge in AI Systems]] makes.

**Differentiation vs Solco:** Trunk Tools indexes already-digital construction documents and makes them queryable. Solco extracts knowledge that has never been written down. They start where digital documentation exists; Solco operates upstream of digital documentation.

---

### KAI / Deep Space (Australia / New Zealand)

**Source:** deepspacegroup.ai/platform/kai, `00-Raw/KAI - AI Assistant for Construction Management.md`.

| Detail | Value |
|---|---|
| Product name | KAI = "Knowledge and Insights" |
| Parent platform | Deep Space — connected construction OS (programme, RFIs, site diaries, defects/safety, procurement, commercial, claims, reporting, client portals) |
| Target customer | Project managers, commercial leads, site teams; mid-tier builders in Australia / NZ |
| Positioning | "Not a chatbot. The AI brain that you need in your projects." Built-in, no-prompt assistant inside the Deep Space platform. |
| Core capabilities | Flags delivery delays, surfaces risks (RFIs, SWMS, variation exposure), suggests actions, reduces noise. Background-resident, not query-driven. |
| Sales motion | Demo via meetings.hubspot.com/deepspace |

**Why this matters to Solco:**
- **Embedded vs standalone.** KAI is not sold as a separate product — it is a layer inside an existing OS. Strong validation of the "second brain as feature, not standalone app" architecture debate ([[MI — Mem (a16z Podcast)]], [[MI — Second Brain Execution Layer (YouTube)]]).
- **"No prompts. No setup. Just helpful signals when they matter most."** This is the **always-on observation** mode our Pillar 2 / Phase 2 is heading toward ([[MI — Computer-Use AI Agents (Clicky, Google DeepMind)]]). Confirms the bet that proactive surfacing beats reactive querying.
- **PM testimonial language is highly transferable.** "It's like having a junior PM who doesn't take breaks." Direct analogue for the role-replacement framing flagged in [[Interview 026 — Eric Quintane (ESMT Professor, Organizational Behavior)]] (Pattern 45 objection cluster: "replacement-framing").

**Differentiation vs Solco:** KAI is a project-execution copilot for builders already using Deep Space. It assumes the company has digital project data. Solco extracts knowledge from companies that don't.

---

### Zepth AI (UAE / India — construction, Dubai-focused)

**Source:** zepth.com/ai, `00-Raw/Zepth AI.md`.

| Detail | Value |
|---|---|
| Positioning | "The Cognitive Intelligence Layer" — proprietary AI orchestration engine; 100,000+ "decisions automated" headline |
| Architecture | State-machine orchestration; multi-stage decision chains; parallel agent coordination; human-in-the-loop gates; workflow resume; iterative refinement loops |
| Agent count | 11 specialised agents across Document Management, Review & Response, Compliance (Dubai-specific: Building Code, Safety Code, Green Building Code), and Analysis (Risk, Specification, Contract) |
| Solutions | 12 production solutions — Co-Pilot, AI Control Room, Program Risk Assessment, Float Exhaustion & Delay Momentum, Submittal Review (95% time reduction claim, 98.5% accuracy claim), RFI Review, AI Nudges, AI Decision Acceleration, Compliance & Audit, Claims Review |
| Integrations | Autodesk Construction Cloud, Oracle P6/Aconex, Procore, SharePoint, Google Drive, Dropbox |
| Regulatory wedge | Dubai Municipality / Civil Defense / Green Building codes baked into dedicated agents — geographic moat through local regulatory specialisation |

**Why this matters to Solco:**
- **Most architecturally mature reference in the set.** 11-agent specialist mesh + state-machine orchestration is the closest published architecture to our Phase 2 vision (specialised extraction + governance agents over a knowledge graph). Useful technical reference for CTO conversations.
- **Geographic regulatory moat as positioning.** Dubai-specific code agents are not portable to Saudi or Singapore. This is the inverse of our "methodology-not-model" moat ([[Interview 022 — Marco Nortmeier (Filigran, Germany)]]) but rhymes structurally: depth-in-one-context beats generality.
- **"Stateful across hours, days, or weeks" is a knowledge-vault property.** Their orchestration engine retains context across long-running workflows — same architectural requirement as the Solco persistent knowledge base. Confirms that production-grade construction AI is already paying the engineering cost for state persistence, which de-risks our equivalent technical bet.

**Differentiation vs Solco:** Zepth automates **construction project decisions** using already-digital project artefacts (drawings, specs, RFIs, submittals). Solco extracts **judgment frameworks** from human experts in companies whose project artefacts may not exist in digital form. Different inputs, different industry, but a shared bet on multi-agent orchestration.

---

### Cross-Cutting Observations from the Construction Set

- **Industry-wide "AI brain" / "Cognitive Intelligence Layer" framing.** Four independent platforms in the same vertical converged on the same metaphor inside ~12 months. Strong signal that the metaphor is **stage-of-market**, not Solco-specific. We should expect the same language to appear in the Mittelstand AI consultancy space within 12–18 months.
- **Vertical AI thesis validated by funding.** Klutch's $8M seed (Bling + Bain Capital Ventures) confirms the [[MI — Domain Expert Knowledge in AI Systems]] "400% YoY vertical AI growth" trend in a concrete deal. Anchors realistic seed-round expectations.
- **All four platforms operate on already-digital project data.** None extract knowledge from human experts. The unsolved layer in construction (and in our Mittelstand market) remains tacit, undocumented founder/master-craftsman knowledge — confirming the Solco wedge.
- **Forbes survey context.** Industry-wide framing in [[MI — AI-Powered Knowledge Management in AEC (Forbes)]] — Autodesk, WSP, AECOM, DPR Construction, ALICE Technologies, Revaka — confirms AEC is one of the most active proving grounds for the "knowledge management + AI" thesis. Two reasons this matters: (a) credibility anchor in pitches ("the AEC industry is already buying this thesis at $1.4B+ scale"), (b) ALICE and Hypar are useful technical reference points for our Phase-2 generative / optimisation layer.

---

## Hubi's AI Consulting Partner (unnamed, near AWW)
- **What they do:** Build custom AI tools for manufacturing use cases — databases, production-grade solutions
- **Location:** ~100km from AWW, southern Germany
- **Relevance:** Hubi ([[Interview 018 — Hubertus von Huelsen (AWW, Germany)]]) is partnering with them to build exactly what we're building — AI-powered knowledge extraction from analog manufacturing processes
- **Threat level:** Unknown — may be a CTO lead, a technical partner, or adjacent competition. Three-way conversation to be scheduled.
- **Status:** Not yet assessed. Open question in [[Open Questions]].
- **Source:** [[Interview 018 — Hubertus von Huelsen (AWW, Germany)]]

---

## Open Questions

- [x] Who exactly is the US competitor raising $5.4M (from [[1 to 1s — Week 3]])? Is it Clonable?
- [ ] What did Prisma's knowledge management system (built with a partner in Wiesbaden) actually consist of? Is it a competitor or a potential technical reference?
- [ ] Is there a German-language equivalent to Clonable that already has Mittelstand traction?
- [ ] Research and categorize all entries in the Flagged for Research table above — especially Memory intelligence and Runeform AI
- [ ] Research Omnivisor (omnivisor.io / Radek Miszkont) — pricing, deliverables, close rate, deliverable type. Surfaced as the closest competitor via Interview 006.
- [ ] Does any construction-vertical AI platform (Klutch / Trunk Tools / Deep Space / Zepth) sell into Mittelstand construction SMEs in DACH? If yes — direct competitor; if no — leave them as adjacent reference.
- [ ] Is there a manufacturing-vertical equivalent of Klutch (named AI agents on WhatsApp/SMS for Mittelstand shop floors)? If yes — closer competitor; if no — wedge confirmed.

---

## Related

- [[Origin Story]] — Celonis analysis first developed during the 5H bootcamp
- [[Product Methodology]] — our methodology is specifically designed to work where Celonis fails
- [[Interview 002 - Ex-Banker, BoD of Deutsche Bank, SMEs view]] — Carl named the process mining competitors
- [[Interview 003 - Merih (Finance Professor)]] — Clonable and decision replication
- [[Interview 006 - John Lynch (Lynka)]] — the ERP ceiling pattern
- [[1 to 1s — Week 3]] — US competitor raising $5.4M flagged here
- [[MI — Domain Expert Knowledge in AI Systems]] — vertical AI 400% YoY context for the construction-AI set
- [[MI — AI-Powered Knowledge Management in AEC (Forbes)]] — Forbes survey of AEC + AI knowledge management; industry context for Klutch / Trunk Tools / KAI / Zepth
