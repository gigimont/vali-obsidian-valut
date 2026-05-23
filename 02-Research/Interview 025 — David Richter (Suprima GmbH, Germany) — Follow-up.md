# Interview 025 — David Richter (Suprima GmbH, Germany) — Follow-up

#research #interview #sme-owner #manufacturing #germany #follow-up

> **Date:** May 21, 2026
> **Interviewee:** David Richter — Suprima GmbH
> **Sector:** Manufacturing (Textiles / Specialized apparel)
> **Geography:** Germany
> **Company Size:** ~60 employees total (15-20 in production)
> **Context:** Follow-up meeting after ~2 weeks of sprint. Solcus team presented the updated methodology, new cross-industry patterns, and MVP concepts.
> **Format:** Video call (transcript available)

---

## ⚠️ Significance of This Interview

**David provided the strongest technical and operational validation of the Solcus MVP architecture and the "Planungsleiter" ICP.** As the leader of a 60-person manufacturing SME, he perfectly articulated the dual-threat of knowledge loss: the sudden departure (purchasing department) and the ticking clock of retirement (production planning). 

Crucially, David independently arrived at the exact technical architecture Solcus is building (using Obsidian/Markdown as the normative knowledge layer with an LLM like Claude on top for the judgment layer). He also provided vital feedback on the [[Product Methodology]]: warning about the "job security paradox" (experts hoarding knowledge to remain valuable) and suggesting a "shadowing" approach to elicitation rather than purely theoretical interviews.

**Cross-reference with [[ICP Definition]]:** David confirmed that the "Planungsleiter" role is the universal bottleneck. Wolf cross-validated this during the call, noting that changing yarns in David's textile machines matches the exact complexity of changing steel products in the von Weiler family business. 

---

## The Knowledge Bottlenecks at Suprima

David highlighted two distinct knowledge crises in his company:

**1. The Sudden Loss (Purchasing Department)**
- An employee with 15 years of experience is about to retire in the company. 
- The role relied entirely on "gut feeling" (tacit knowledge) regarding when and what to order. 
- Nothing was documented. 
- **Impact:** The successors failed to manage the supply chain, leading to the company running out of products.

**2. The Ticking Clock (Production Planning)**
- 15-20 employees in the production unit. 
- Planning is handled by one person with 20 years of experience. 
- The role requires balancing highly variable factors: which employees are present, individual skill levels, machine setups, and transition costs (e.g., swapping a white yarn for a red yarn).
- The knowledge is completely undocumented. 
- **The Threat:** This person will retire in 5 years. Documenting everything manually is not cost-effective for a company of 60 people, framing the exact need for an AI-enabled extraction methodology.

---

## Key Quotes

> "We ran out of products because his experience... he had like a gut feeling when and what he needed to order. And nothing was documented." 

> "It's way easier for people to just do their thing and talk about it and view asking questions than to theoretically talk in an interview." 

> "Be aware not everybody wants to share his or her knowledge because that's what makes them valuable... It's very delicate to frame it right. So that people don't think that you just get all their knowledge and then they get ditched." 

> "It's actually Obsidian, right? You could use Obsidian markdown files as a knowledge base... and put Claude on top of it to have like this interaction layer." 

---

## What We Learned

### Contextual Elicitation > Theoretical Interviews
David emphasized that asking an expert to theoretically explain their job is extremely difficult. The methodology should lean heavily into "shadowing" — having the expert perform the task in context and explaining it as they do it. 
* **Product Implication:** Update [[Product Methodology]] to ensure "Campfire storytelling" includes contextual shadowing for operational roles.

### The Job Security Paradox (Trust Thresholds)
Employees often view their undocumented tacit knowledge as their job security. If the extraction process is framed poorly, they will resist out of fear of being "ditched."
* **Strategic Implication:** This perfectly reinforces **Pattern 35 (three trust thresholds)** and Pattern 28. The intervention must be framed around *delegation* (freeing the expert to do higher-value work) rather than *replacement*. 

### Architecture Validation
David, a tech-savvy SME owner who is building prediction models himself, independently suggested the Phase 2 product architecture: local markdown files (Obsidian) acting as the structured knowledge base, with an LLM (Claude) layered on top for natural language querying. This validates that the technical deliverable resonates with the target market.

---

## Patterns Confirmed

- **[[ICP Definition]] (Pattern 42):** The Head of Department / Planungsleiter is the consistent bottleneck across industries. Textile manufacturing behaves exactly like steel manufacturing in this regard.
- **[[Patterns From Fieldwork]] Pattern 41 — Retirement Window:** The 5-year runway for the production planner is the exact "sweet spot" for extraction readiness. 
- **[[Product Methodology]] (Pattern 35 — Trust Thresholds):** Confirmed the psychological resistance to knowledge capture (fear of replacement). 
- **[[Patterns From Fieldwork]] Pattern 40 — Documentation Entropy:** Confirmed that manual documentation is economically unviable for SMEs ("it wouldn't make any sense cost-wise for us").

---

## Action Items

- [ ] Update [[Product Methodology]] to explicitly include "Contextual Shadowing" alongside Campfire Storytelling.

---

## Related

- [[Interview 026 — Eric Quintane (ESMT Professor, Organizational Behavior)]] — next in the chain; academic positioning stress-test after this technical/operational validation
- [[Interview 024 — Eberhard Müller-Menrad (Eyewear Mittelstand, Germany)]] — preceding interview
- [[Patterns From Fieldwork]] — Patterns 35, 40, 41, 42 reinforced here
- [[Product Methodology]] — shadowing addition
- [[ICP Definition]] — Planungsleiter / head-of-department wedge confirmed
- [ ] Refine the GTM messaging to address the "Job Security Paradox" head-on (framing Solcus as a delegation enabler, not a replacement tool).
- [ ] Keep David in the loop as a potential beta tester for the Phase 2 Obsidian+LLM architecture, given his explicit interest in this exact setup.