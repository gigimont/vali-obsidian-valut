# Competitors

#research #strategy #competitive-landscape #living-document

> Update as new companies are discovered or positioning sharpens.

---

## The Positioning Frame

We are not a process mining tool. We are not a management consultancy. We are not an ERP vendor. The competitive landscape only makes sense when viewed through the lens of what we actually do: **extract tacit knowledge from organically grown SMEs and deliver it as a structured Organizational Report**.

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

| Company | URL | Notes |
|---|---|---|
| **Remly** | https://remly.it/ | Italy-specific; category unclear |
| **Noah support** | https://noah.support/ | Unknown; possibly knowledge/support tooling |
| **Runeform AI** | https://www.runeform.ai/ | Unknown; AI category unclear |
| **Theblankcollar** | https://www.theblankcollar.com/ | Unknown |
| **Simplyasking** | https://simplyasking.io/ | Possibly interview/survey tooling |
| **Useyourbrain** | https://www.useyourbrain.io/ | Unknown |
| **Memory intelligence** | https://memoryintelligence.io/ | Directly relevant name — priority to research |
| **Runlog AI** | https://www.runlogai.com/ | Unknown; possibly workflow/ops logging |
| **Nexindex** | https://nexindex.io/ | Unknown |
| **Unoy** | https://unoy.io/ | Unknown |

---

## Open Questions

- [ ] Who exactly is the US competitor raising $5.4M (from [[1 to 1s — Week 3]])? Is it Clonable?
- [ ] What did Prisma's knowledge management system (built with a partner in Wiesbaden) actually consist of? Is it a competitor or a potential technical reference?
- [ ] Is there a German-language equivalent to Clonable that already has Mittelstand traction?
- [ ] Research and categorize all entries in the Flagged for Research table above — especially Memory intelligence and Runeform AI
- [ ] Research Omnivisor (omnivisor.io / Radek Miszkont) — pricing, deliverables, close rate, deliverable type. Surfaced as the closest competitor via Interview 006.

---

## Related

- [[Origin Story]] — Celonis analysis first developed during the 5H bootcamp
- [[Product Methodology]] — our methodology is specifically designed to work where Celonis fails
- [[Interview 002 - Ex-Banker, BoD of Deutsche Bank, SMEs view]] — Carl named the process mining competitors
- [[Interview 003 - Merih (Finance Professor)]] — Clonable and decision replication
- [[Interview 006 - John Lynch (Lynka)]] — the ERP ceiling pattern
- [[1 to 1s — Week 3]] — US competitor raising $5.4M flagged here
