# Interview 016 — Stefan Bergerhoff (BWB-Gruppe / FDU, Germany)

#research #interview #expert #planning-leader #manufacturing #germany #precast-concrete #customer-side

> **Date:** May 2026
> **Interviewee:** Stefan Bergerhoff — Planungsleiter & Prokurist, BBT (planning arm of BWB-Gruppe / FDU)
> **Sector:** Precast concrete elements — Elementdecken, Doppelwände, konstruktive Fertigteile
> **Geography:** Germany, multi-site (24–25 Betonwerke)
> **Group structure:** Family business owned by Brinkhege family. FDU = sales/Faktura. BWB = production (24–25 plants). BBT = planning/technology. Bergerhoff sits in BBT.
> **Scale:** 130 internal planners + external offices. ~600–700 employees across the group (plus second-shift subcontractors). Active customer of Filigran (lattice girders).
> **Connection:** Introduced via Ulrich Bauermeister (see [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]). Bauermeister flagged Bergerhoff as facing the same archive-and-knowledge problem from the customer side.
> **Format:** Video call in German (transcript available)
> **Follow-up:** Bergerhoff offered to forward Wolf to Herr Grass (Geschäftsführer, kaufmännischer Bereich) for the operational/commercial-side perspective. Wolf to send 3-sentence summary for Bergerhoff to forward.

---

## ⚠️ Significance of This Interview

**Bergerhoff is the customer-side analogue to Bauermeister, validating that the same archival-knowledge problem repeats up the construction value chain.** Filigran sells lattice girders to BWB/FDU, who then engineer Elementdecken and Doppelwände for end customers. The technical questions Bauermeister fields about Filigran's products turn into the technical questions Bergerhoff fields from his 130 planners about how to apply those products in real designs. The knowledge-loss problem doesn't stay inside one company — it propagates downstream through the entire technical supply chain.

This interview also significantly sharpens [[Patterns From Fieldwork]] Pattern 22 (ERP ceiling): **BWB/FDU is fully digitalized — ERP, CAD-to-production, automated invoicing, even mid-ERP-migration — and yet Bergerhoff is still the single human bottleneck for the technical knowledge layer.** Digital maturity has not solved the tacit-knowledge problem; it has only made the contrast sharper. This contradicts our working ICP assumption that high digital maturity = exclusion, and adds the role-vs-size ICP question to our strategic to-do list.

Finally, Bergerhoff offered an unprompted GTM framing — **knowledge capture as the foundation for further AI implementation** — that aligns almost word-for-word with our internal "second brain → ecosystem upsell" vision. This is the first time a customer-side prospect articulated the upsell logic for us, not the other way around.

---

## Context

BWB-Gruppe is a structurally larger version of the Filigran customer profile. It is family-owned (Brinkhege), operates 24–25 precast concrete plants across Germany, and runs a dedicated 130-person planning arm (BBT). The group is one of the largest precast concrete groups in the German market.

Bergerhoff is Planungsleiter and Prokurist at BBT. His daily work involves fielding technical questions from his 130 internal planners (plus external offices) about how to correctly apply Stahlbetonbau norms, Brandschutznormen, WU-Richtlinien, product approvals (Zulassungen), and a steady stream of Fachberichte to specific design problems involving Filigran's lattice girders and BWB's own precast products.

He has thought about the documentation problem for years. He attempted a partial documentation effort himself — a focused write-up of one narrow technical sub-topic (Expositionsklassen und Betondeckung) — and produced an 8-9 page document. The exercise convinced him both that capturing this knowledge has real value and that doing it manually at scale is not viable. He had a prior exploratory conversation two years ago with someone in Switzerland who proposed a 20-programmer Hackathon to automate the work; nothing came of it.

---

## Key Quotes

> "Ich beschäftige mich eigentlich seit Jahren mit Zulassung, Normung, Entwicklung... immer wenn da jemand an ein technisches Problem gestoßen ist, ruft er mich an, schreibt mir eine Mail oder sagt: ja, wie funktioniert das denn eigentlich noch mal, oder wo steht dies oder jenes."

> "Ich mache mir eigentlich schon seit Jahren Gedanken darüber, wie man das auch alles mal aufschreibt. Aber das alles aufzuschreiben, mit allen Verzweigungen, ist relativ komplex."

> "Ich hab tatsächlich mal mit angefangen... um ein kleines Thema, Expositionsklassen und Betondeckung... habe ich, glaube ich, acht oder neun Seiten zusammengeschrieben."

> "Allein dieses wirklich das Wissen festzuhalten, aber auch einfach eher dann mit KI die Möglichkeit zu haben, weil da kann ich ja wirklich eine Frage stellen. Welche Betondeckung muss ich jetzt einhalten oder solche Sachen über eine KI. Was mich die Leute heute fragen, was mich Zeit und Aufwand kostet."

> "Ich bin natürlich für das Unternehmen quasi, wenn ich nicht da bin, fehlt irgendwas, weil das Wissen nicht da ist. Ich könnte mich auch mit anderen Sachen beschäftigen."

> "Ich kann dadurch Personalkosten reduzieren, das ist ja heute das höhere Problem. Wenn ich sowas kann's schneller abrufbar machen und besser zugreifbar für andere Mitarbeiter an der Stelle. Problem ist natürlich auch in dem Bereich Fachkräftemangel, zukünftige Wirtschaftlichkeit."

> "Eigentlich ist ja die Frage, ob ich das nicht schon als Grundlage brauche, um auch weitere KI-Prozesse zu implementieren, um weitere Sachen zu machen."

> "Ich glaube das ist das i-Tüpfelchen auf der KI an der Stelle... aber ich müsste ja erstmal gut für mich gedanklich erstmal die Basis haben, die mir erstmal schon mal die Grundlage beantwortet, warum mache ich das so, weshalb mache ich das so und wie mache ich das."

> "Wir sind im Prinzip auch ein gesellschaftergeführtes Familienunternehmen." *(on BWB-Gruppe)*

> "Das ist natürlich wichtig, wenn Sie es weitergeben wollen... aber das will ja ungern jemand, dass irgendwie da drauf zugreift." *(on data sensitivity for the business-model layer of company knowledge)*

---

## What We Learned

### On the "Standardgrundlage zuerst, Sonderfälle später" framing (PRODUCT-DESIGN INSIGHT)

When Wolf described the "campfire / storytelling" extraction method ([[Patterns From Fieldwork]] Pattern 28), Bergerhoff did not reject it — but he reframed it sharply: "Das verfeinert ja dann glaube ich erstmal das System. Ich glaube die Grundlage ist ja erstmal daraus, dass das System ja diesen Standard beantworten kann."

In other words: for technical-domain SMEs, the **standard-questions layer must be answered first**. Capturing the rare exceptions and judgment calls (the i-Tüpfelchen) is valuable but secondary. The first job of the product is to handle the routine technical queries that consume the expert's time today — only then does the layered Sonderfall capture become relevant.

**Implication:** This suggests a sequenced delivery model — not "campfire stories from day one," but **(1) ingest the normative/document layer first, (2) build the standard-answer capability, (3) layer the storytelling-extraction on top to capture the judgment edges**. This is a meaningful refinement of [[Product Methodology]] for engineering-heavy customers and may differ from the methodology for relational/decision-heavy customers like [[Interview 011 — Dairy Chemicals Commercial (Italy)]].

### On the digitalization-ceiling paradox (sharpens Pattern 22)

BWB/FDU is far more digitally mature than Filigran. They have: a working ERP, automated CAD-to-production data flow, two CAD systems pulling parameters from a database, full digital production with machine-level control, automated invoicing including special charges and shortfalls, even mid-migration to a more modern ERP. By any reasonable measure, this is a digitalized company.

**And yet Bergerhoff is still the single human bottleneck for the technical knowledge layer.** Phone calls, emails, "ruf mich kurz an." The ERP captures transactions and production parameters; it does not capture *why a particular Betondeckung is required for a given Brandschutzklasse in an Elementdecke design*. The volldigitalisiert layer and the tacit-knowledge layer are completely orthogonal.

**Implication:** This is a direct extension of [[Patterns From Fieldwork]] Pattern 22 (ERP ceiling), but with a sharper edge: **digital maturity does not just leave the tacit-knowledge layer untouched — it may make it more visible, because everything else has been industrialized**. Our ICP definition currently treats "basic digital maturity" as a fit indicator and "high digital maturity" as an exclusion. Bergerhoff suggests this exclusion criterion is wrong or incomplete. Worth revisiting [[ICP Definition]] — see Action Items.

### On unprompted articulation of the ecosystem-upsell logic

The most strategically significant moment of the interview: Wolf had not yet introduced the "second brain as foundation for further AI implementation" framing when Bergerhoff said:

> "Eigentlich ist ja die Frage, ob ich das nicht schon als Grundlage brauche, um auch weitere KI-Prozesse zu implementieren, um weitere Sachen zu machen."

This is our Phase 2 ecosystem story said back to us by a customer-side prospect, unprompted. It is the strongest endorsement we have received of the product's strategic positioning — not because Bergerhoff agreed with us, but because he arrived there on his own.

**Implication:** The "captured knowledge base = foundation for everything else" framing has traction with technically-fluent customer-side stakeholders. It may be the right opening framing for engineering and planning leaders, even if it is the wrong framing for founders (who hear "AI implementation" and shut down — see Pattern 29).

### On scope sensitivity — the kaufmännischer Bereich is a separate conversation

Bergerhoff was explicit about the limits of his own scope: he runs technical planning, not commercial operations. When Wolf asked about other roles within BWB that might benefit from a similar knowledge base, Bergerhoff named the Vertrieb (also needs technical answers on the road) and then named **Herr Grass, the Geschäftsführer with the kaufmännischer Bereich**, as the right person for the broader operational/commercial perspective. He offered to forward an introduction.

He also flagged a sensitive boundary: pure technical content is shareable; the **business-model layer** of company knowledge ("womit die natürlich auch ihr Geld verdienen") is not, and customers will resist any tool that touches it. This is a real product-design constraint.

**Implication:** Within a single ICP-fit company, there are at least three distinct buyers with three distinct trust thresholds — technical (Bergerhoff: high openness), commercial (Grass: TBD), and strategic/proprietary (likely the family/owner: low openness). The product must be packageable to the technical entry-point without immediately threatening the commercial layer.

### On the "I would be freed up to do better things" framing

Bergerhoff articulated something close to the founder-freedom framing of the One-Pager v2/v3, but in his own context: *"Ich könnte mich auch mit anderen Sachen beschäftigen."* He sees himself as a 130-planner-supporting bottleneck and would prefer to spend his time on higher-value technical work. This is the same emotional driver as the founder framing but expressed by a Prokurist, not an owner.

**Implication:** The "freed-up capacity" message generalizes beyond founders. It works for any senior technical role where the person is being used as a human Q&A system. Worth testing in the outreach copy for engineer- and Prokurist-level prospects.

### On Personalkosten / Fachkräftemangel as the commercial driver

When Wolf asked how Bergerhoff would package the concept commercially, his first answer was *not* succession or M&A — it was **labor cost reduction and the Fachkräftemangel**: making expert knowledge accessible to less senior staff so that the company can operate with fewer expensive specialists in a tight labor market. This echoes [[Patterns From Fieldwork]] Pattern 26 (labor scarcity makes knowledge protection more valuable) and Pattern 27 (onboarding speed as universally-valued).

**Implication:** For the customer-side / planning-leader segment, the headline value proposition is closer to "leverage your scarce experts further" than to "preserve knowledge for handover." Same product, different opening.

---

## Patterns Confirmed and New

### Confirmed
- **[[Patterns From Fieldwork]] Pattern 2 — Knowledge trapped at two levels:** Bergerhoff explicitly is the single human source for normative/technical knowledge across 130 planners.
- **[[Patterns From Fieldwork]] Pattern 5 — Irreplaceability myth (real version):** *"Wenn ich nicht da bin, fehlt irgendwas, weil das Wissen nicht da ist."* Confirmed at the Prokurist level, not just at the founder level.
- **[[Patterns From Fieldwork]] Pattern 8 — Neutral mirror:** Bergerhoff's Standardgrundlage-first framing aligns with the "document what exists before suggesting what should change" principle.
- **[[Patterns From Fieldwork]] Pattern 22 — ERP ceiling (SHARPENED):** BWB is fully digitalized at the transactional layer (ERP, CAD-to-production, automated invoicing, mid-ERP-migration) and still entirely dependent on Bergerhoff for the judgment layer. Digital maturity does not protect against the tacit-knowledge bottleneck — it may even make it more visible. This contradicts the working ICP assumption that high digital maturity = exclusion, and adds an open strategic question about role-based vs size-based ICP.
- **[[Patterns From Fieldwork]] Pattern 25 — Under-advised on AI:** Bergerhoff's two-year-old Swiss-Hackathon conversation that went nowhere is a textbook example. Motivated, internally credible, no usable advisory path.
- **[[Patterns From Fieldwork]] Pattern 26 — Labor scarcity makes knowledge protection more valuable:** Bergerhoff led with this as the commercial framing.
- **[[Patterns From Fieldwork]] Pattern 27 — Onboarding speed:** Implicit in his Personalkosten / scarce-expert framing.
- **[[Patterns From Fieldwork]] Pattern 31 — Forgotten institutional knowledge has measurable cost:** Confirmed at a different scale — for Bergerhoff the cost is his own time across 130 planners, not €20K experiments.
- **[[Patterns From Fieldwork]] Pattern 32 — Motivated technical insider blocked at the build step:** Bergerhoff is the exact pattern — knows the problem, started solo (8–9 pages), engaged an external party (Swiss Hackathon), got nowhere.
- **[[Patterns From Fieldwork]] Pattern 33 — Trade-association as GTM channel:** Bergerhoff is exactly the kind of person who would benefit from the Fachvereinigung shared-chatbot model Bauermeister proposed.

### New

**Pattern 34 — Standardgrundlage first, Sonderfall layer second**
For technical-domain SMEs, the standard-answers layer must be in place before the judgment-extraction (storytelling) layer adds value. Customers will not see the value of capturing rare exceptions until the routine technical Q&A is automated. This suggests a sequenced delivery: (1) ingest the normative document layer, (2) build standard-answer capability, (3) layer storytelling-extraction on top for the judgment edges. May differ for relational/decision-heavy domains (e.g. Interview 011, Italian dairy commercial) where the judgment layer IS the standard.
- **Source:** [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]]
- **Strength:** Strong — explicit pushback when offered the campfire-first framing, with clear reasoning

**Pattern 35 — Multiple buyers within one company, with three distinct trust thresholds**
Within a single ICP-fit company there are typically three distinct internal stakeholders: the technical lead (high openness, eager for tooling), the commercial/operations lead (moderate openness, focused on Personalkosten), and the strategic/ownership lead (low openness, protective of the business-model layer). The product must be packageable to enter at the technical layer without prematurely activating resistance at the strategic layer. Confirms and structures the "multi-buyer, one captured asset" framing from the pitch deck.
- **Source:** [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]], with cross-reference to [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]
- **Strength:** Moderate — emerging pattern, second confirmation within Filigran/BWB context; needs testing in non-engineering ICP companies

---

## Which sub-problem did this touch?

- [ ] **Matching** — not directly
- [x] **Readiness** — strongly. Bergerhoff's bottleneck is the readiness problem at the technical-supply-chain layer.
- [ ] **Emotional** — not in this conversation. Bergerhoff is pragmatic.
- [x] **Deal-structuring** — indirectly, via the BWB-as-customer-of-Filigran relationship. The same knowledge problem propagates through the supply chain.

---

## Upstream or downstream?

**Upstream and operational, with explicit ecosystem framing.** Bergerhoff is not facing succession. He is facing operational scarcity (Fachkräftemangel) and a personal time bottleneck. The product enters his world through the standard-questions layer and expands into the AI-foundation framing he articulated himself. This is a different entry-point than the founder-side succession framing — and it's notable that Bergerhoff arrived at the ecosystem framing unprompted. Strong evidence that the upstream-operational entry is viable independently of the succession narrative for technical decision-makers.

---

## ICP Relevance

BWB-Gruppe is **larger than the current ICP wedge** (24–25 plants, 600–700 employees, 130 planners alone). This places them adjacent to the Lynka exclusion ([[Interview 006 - John Lynch (Lynka)]]) rather than within the 20–100 employee, €5–25M revenue wedge.

However, Bergerhoff's *role* and *pain* match the ICP-relevant profile perfectly: he is exactly the kind of motivated technical insider Pattern 32 describes. This raises a real question about ICP definition: **are we targeting companies of a certain size, or roles within companies of a certain profile?** Bauermeister at Filigran (110 employees, ICP fit) and Bergerhoff at BWB (700 employees, ICP miss on size) have nearly identical pain profiles. The role is consistent across size.

**Implication for [[ICP Definition]]:** The current size-based ICP may be over-restrictive. The role-based ICP (motivated technical insider with documentation pain, in a knowledge-heavy traditional sector, under labor pressure) generalizes across company sizes. **This is now on the strategic to-do list for joint discussion with Giuseppe (see Action Items).**

---

## Action Items

- [ ] **Priority:** Send 3-sentence summary to Bergerhoff for him to forward to Herr Grass (Geschäftsführer, kaufmännischer Bereich). Wolf committed to this on the call.
- [ ] **Priority:** Schedule follow-up call with Herr Grass once introduction lands. This is the commercial/operational counterpart to the Bergerhoff technical view — completes the picture within BWB-Gruppe.
- [ ] **STRATEGIC TO-DO — Discuss with Giuseppe:** Does the BWB observation (digital maturity does not protect against the tacit-knowledge bottleneck; role-based ICP fit despite size-based miss) require us to revise [[ICP Definition]]? Specifically: (a) should the ERP-maturity exclusion be dropped or reframed, and (b) should the ICP be defined role-based (motivated technical insider in knowledge-heavy traditional sector under labor pressure) rather than purely size-based? Cross-check the Pattern 22 sharpening against [[Interview 006 - John Lynch (Lynka)]] — does the digitalization-ceiling paradox hold there too?
- [ ] Test the Standardgrundlage-first sequencing (Pattern 34) in the next 2-3 technical-domain interviews. Does it hold for non-precast engineering companies?
- [ ] Update the pitch deck "multiple buyers, one captured asset" framing to reflect the three-distinct-trust-thresholds structure (Pattern 35).
- [ ] Bauermeister explicitly asked to be kept in the loop on the Fachvereinigung idea (Pattern 33) — Bergerhoff confirming the same pain in a customer-side context strengthens the case. Worth a joint follow-up message.

---

## Open Questions Raised

- [ ] How do we package a Standardgrundlage-first sequenced delivery? Is this a different product line from the campfire-first methodology, or the same methodology with a different entry-point depending on industry?
- [ ] Where exactly is the line between "technical knowledge" (Bergerhoff shareable) and "business-model knowledge" (protected)? Can we draw this line cleanly enough to give technical-layer customers confidence?
- [ ] Should we have a separate ICP definition for the role-based wedge (technical lead under labor pressure) vs the size-based wedge (founder-led 20–100 employee company)? Or is one a subset of the other?
- [ ] Is the "ecosystem foundation" framing safe to lead with for technical-buyer conversations, even though it would be wrong for founder conversations? How do we tell which framing to use without asking?

---

## Related
- [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]] — the introducing interview; same pain profile (engineer with archive problem, motivated, internally credible, blocked at build); Bergerhoff confirms the propagation of the same problem one step down the supply chain
- [[Interview 006 - John Lynch (Lynka)]] — both are mid-ERP-migration, both digitally sophisticated, both feel the tacit-knowledge ceiling; cross-check the Pattern 22 sharpening here
- [[Interview 011 — Dairy Chemicals Commercial (Italy)]] — "chiavi di lettura" framing vs Bergerhoff's "Standardgrundlage zuerst" — both right for different industries, different starting points; key contrast point for Pattern 34
- [[Interview 012 — Stefan Weiler (Filigran, Germany)]] — same supply chain (Filigran → BWB), different layer (CEO with succession problem vs Planungsleiter with operational bottleneck); together they triangulate the full Filigran-BWB knowledge value chain
- [[Interview 013 — David (Textile Manufacturing, Germany)]] — David's campfire method (Pattern 28) is the layer-3 method; Bergerhoff says layer-1 (standard normative ingestion) must come first for technical industries
- [[Patterns From Fieldwork]] — Patterns 34, 35 added; Pattern 22 sharpened; Patterns 2, 5, 8, 25, 26, 27, 31, 32, 33 confirmed
- [[ICP Definition]] — Pattern 22 sharpening challenges the ERP-maturity exclusion; Pattern 35 structures the multi-buyer framing
- [[Product Methodology]] — Pattern 34 suggests a sequenced delivery model for technical-domain ICPs that differs from relational/decision-heavy ICPs
- [[Pitch Deck Content]] — Pattern 35 maps directly to the "multiple buyers, one captured asset" framing in the deck
- [[Outreach Strategy]] — Herr Grass referral is a warm next step; Pattern 33 Fachvereinigung channel strengthened by second engineering-customer confirmation
