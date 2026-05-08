# Interview 014 — Ulrich Bauermeister (Filigran, Germany)

#research #interview #expert #engineer #manufacturing #germany #filigran #internal-network

> **Date:** May 2026
> **Interviewee:** Ulrich Bauermeister — engineer / technical leadership at Filigran (Wolf's family steel manufacturing business)
> **Sector:** Steel / construction (Gitterträger / lattice girders for precast concrete elements)
> **Geography:** Germany (Filigran HQ; Filigran Polen also referenced)
> **Connection:** Introduced via Stefan Weiler ([[Interview 012 — Stefan Weiler (Filigran, Germany)]]), Wolf's uncle and Filigran CEO
> **Format:** Video call in German (transcript available)
> **External relationships:** Active member at CBI in Aachen (industrial-academic consortium); regular contact with planning leaders at customer concrete plants (named: Stefan Bergerhoff, BWB-Gruppe)

---

## ⚠️ Significance of This Interview

**Ulrich is the strongest direct product validation in the dataset.** He is not describing a problem we then propose to solve — he is describing a solution he has already tried to build himself, hit obstacles on, and given up on. Specifically: a locally-installed LLM with a local vector database to ingest Filigran's archive of test reports and project documentation from the 1960s onward, so that engineers can query 60 years of accumulated knowledge instead of repeating €20,000 experiments because the original report cannot be found.

He has actually attempted the technical implementation. He hit Python errors on the PDF chunking step before Christmas and stopped. He was disappointed when the Aachen CBI consortium did not provide the "Kochrezept" (cookbook) he was hoping for and instead pointed him toward purchasable software licenses.

When Wolf described the Obsidian + local-Claude setup live on screen, Ulrich's response was: *"Aber das wäre ja genau das, was wir eigentlich auch bei Filigran bräuchten."* This is not "interesting concept" — this is "this is the thing I have been trying to build."

This is also a **second-source confirmation of the Filigran problem from inside the company**, complementing Stefan Weiler's view from the CEO chair. Stefan sees the succession and structural problem; Ulrich lives the daily knowledge-loss problem at the technical layer.

---

## Context

Filigran is Wolf's family business (third generation, ~110 employees, Bavaria, founded 1949 — see [[Interview 012 — Stefan Weiler (Filigran, Germany)]]). Ulrich is the engineering / technical authority on the Filigran ceiling system — the structural product itself. His daily work involves answering technical questions about the product's behavior (e.g., fire resistance, load assumptions, joint behavior), which routinely requires retrieving test reports, project documentation, and decision rationales from decades-old archives.

The technical problem he describes is unusually well-defined. The institutional memory of Filigran exists almost entirely as paper and PDF documents, scattered across two physical relocations and three relocations of the regulatory body (Deutsches Institut für Bautechnik) that originally certified the products. The original professors are dead. The original colleagues are gone. The PDFs that survived are searchable only if you already have them; if you do not, the knowledge is effectively lost — and the company pays €20,000 to repeat experiments that were already conducted thirty years ago.

He requested permission internally to build a local AI knowledge base for this archive, was given a green light, attempted the technical implementation, and got blocked at the Python PDF-chunking step.

---

## Key Quotes

> "Ich wollte gerne mir lokal so ein Large Language Model installieren. Das habe ich auch hingekriegt. Und dann wollte ich zuzüglich dazu mir eine lokale Datenbank erstellen, eine Vektordatenbank, wo ich dann letztendlich diese Dokumente einlese."

> "Vor Weihnachten, wo die Abgabe des Berichtes oder des Artikels immer näher rückte, [habe] ich es nicht zum Laufen bekommen... beim Anpassen des Python-Codes, wo dann die PDF-Datei in Chunks aufgesplittet werden sollte und abgespeichert werden sollte, da bekam ich dann Fehlermeldungen."

> "Da wurde gesagt, das gibt's doch alles schon als fertige Software, sollen wir auch bitteschön die Lizenz kaufen. Ja, insofern glaube ich, dass es das alles gibt, vielleicht auch so, wie ich es haben will, aber ich hätt's ja auch gerne ohne Lizenzkosten gemacht."

> "Wir sind ja alle sparsam bei Filigran, ne." *(on cost sensitivity for tooling)*

> "Sagen wir mal, jetzt fragt jemand, warum funktioniert die Filigran-Decke auch bei Brandbeanspruchung? [...] Dann müssen wir wohl jetzt Versuche machen für 20.000 Euro, weil jemand anzweifelt, dass diese Annahme richtig ist."

> "Doppeluntersuchungen zu vermeiden, weil die Versuchsergebnisse gegebenenfalls vorliegen, auf die man sich berufen kann, das wäre gut, überhaupt davon zu wissen. Und gegebenenfalls weiß ich's jetzt nicht, gehe in den Keller, wühle 20 Ordner durch, bin zwei Tage beschäftigt und hab sie doch nicht gefunden."

> "Die alten Professoren sind weggestorben, die alten Mitarbeiter, die die Projekte betreut haben, auch. Und insofern hat man nur das Wissen, was überhaupt in Schriftform vorliegt — eine andere Wissensquelle haben wir gar nicht."

> "Auch Filigran ist zweimal umgezogen, auch da liegt nicht mehr alles vor, was es mal gab. Und es wird einfach höchste Zeit, jetzt mal anzufangen, mit diesem Papierwust, den wir haben, verfügbar zu machen. Ansonsten wird er verloren gehen über die Jahre."

> "[Bei der Produktionsplanung] sind das auf einmal drei Parameter, wo der Mitarbeitende nicht sagen kann, welchen priorisiere ich wie. Weil das jedes Mal situationsbezogen ist."

> "Aber der hatte gerade gestern Geburtstag, deswegen kriegt er es jetzt ganz schnell, und das nächste Mal, aber mit dem hab ich vorgestern Bier getrunken. Und das sind dann alles Faktoren, die überhaupt gar nicht verfügbar sind."

> "Es ist nicht so, dass man einfach sagt, ich hab hier mein rotes Notizbüchlein, da habe ich die 25 Sonderfälle aufgeschrieben und die müssen wir jetzt nur digitalisieren."

> "Alles was es an Hintergrundwissen gibt und nicht dokumentiert ist, das geht zwangsläufig verloren von einer Generation zur nächsten."

> "Aber das wäre ja genau das, was wir eigentlich auch bei Filigran bräuchten." *(on seeing the Obsidian + Claude Code setup)*

---

## What We Learned

### On the failed self-build (PRODUCT VALIDATION)

Ulrich is not a hypothetical customer — he is an actual prosumer who attempted the build. His sequence:

1. Got internal approval to install a local LLM and a local vector database for Filigran's archive
2. Got the LLM running locally
3. Got the database installed
4. Failed at the PDF-to-chunks ingestion step (Python error, no support, deadline pressure, gave up)
5. Hoped CBI Aachen would publish a "Kochrezept" — a no-license, pragmatic implementation guide for industrial members
6. Was instead pointed toward commercial software licenses, which he does not want

**Implication:** There is a real, unmet, articulated demand in mid-sized German industrial firms for *exactly* the technical setup we are using ourselves. Ulrich's repeated emphasis on doing it without license costs ("ich hätt's ja auch gerne ohne Lizenzkosten gemacht") tells us where the price ceiling sits for this kind of internal tooling: meaningfully below standard enterprise software pricing. The product question becomes: do we sell the *implementation* (we set it up for them) or the *Kochrezept* (we publish how to do it themselves)? The first is more revenue per customer; the second is more market.

### On the cost of forgotten institutional knowledge

The most quantifiable claim in the interview: a single forgotten test report can cost Filigran €20,000 to repeat. This number does not include the time cost of two days in the basement looking through twenty folders. It does not include the regulatory friction of justifying old assumptions to today's reviewers. It does not include the lost optionality of being able to defend an old design choice against a customer challenge.

This compares directly to [[Interview 008 — Antonio Rizza (M&A)]]: Antonio measured documentation completeness against deal price; Ulrich measures it against repeated R&D cost. Two completely different metrics, both mapping to the same underlying value.

**Implication:** For technically-driven SMEs, the immediate, in-period ROI of knowledge capture is measurable in repeated-experiment costs avoided. This is a stronger near-term sales angle than succession framing for engineering-heavy firms.

### On the limits of structured documentation

Ulrich is clear that PDFs cannot just be ingested raw — they need to be transformed into structured intermediate documents (keyword lists, top-down logical lists) for AI to retrieve efficiently. He understands the technical constraint at a level most prospective customers don't.

He also makes a sharp distinction between two kinds of knowledge:

1. **Engineering knowledge** — testable, defensible, attached to specific test reports. Can be digitized with effort. ("Bautechnik")
2. **Production-planning judgment** — situational, contextual, dependent on factors that "are not even available." ("...aber mit dem hab ich vorgestern Bier getrunken.") Cannot be reduced to a rulebook.

The first is the immediate Phase 1 wedge for Filigran-type firms. The second is the harder, deeper layer of [[Patterns From Fieldwork]] Pattern 13 (decision-making gap).

### On why CBI Aachen disappointed him

Ulrich went to the industrial-academic consortium hoping for a shared, license-free Kochrezept. The Maschinenbau Impulsvortrag he heard described forward-looking AI-assisted development modeling — sophisticated, future-oriented, modeling-heavy. When Ulrich said his actual need was simpler — a backward-looking knowledge database for Phase 1 — he was told this is already a commercial product and pointed to a contact who has not yet followed up.

**Implication:** Industrial consortia and university research programs are oriented toward novel research and forward-modeling, not toward the basic, unsexy archival problem mid-sized industrial firms actually have. There is a gap between what academia is interested in and what the Mittelstand needs. Our positioning sits in that gap.

### On the BWB-Gruppe network and the trade-association angle

Ulrich named Stefan Bergerhoff, planning leader at BWB-Gruppe — one of the largest concrete-plant groups in Germany, a Filigran customer (not a competitor). Bergerhoff faces the same problem at the customer side: planning leaders need access to product technical history when answering questions from their own clients about Filigran-supplied components.

Ulrich is already considering proposing this as a project inside the *Fachvereinigung Betonbauteile mit Gitterträgern* — the trade association of concrete-element manufacturers using lattice girders. A shared chatbot, fed once, available to all member companies for technical reference.

**Implication:** This is a potential **trade-association GTM channel** that has not appeared in any prior interview. One sale to a Fachvereinigung gives access to many member firms. Worth investigating as a parallel channel to direct-to-founder outreach. Comparable to commercialisti as an Italian channel ([[Outreach Strategy]]), but for German industrial sectors.

### On Filigran as an MVP sandbox (re-confirmed)

Ulrich's enthusiasm at the end ("das wäre ja genau das, was wir eigentlich auch bei Filigran bräuchten") combined with Stefan's existing buy-in ([[Interview 012 — Stefan Weiler (Filigran, Germany)]]) gives Filigran a usable internal sandbox at multiple levels:

- **CEO level (Stefan):** strategic, succession-facing, willing to host
- **Engineering level (Ulrich):** technical, archival-knowledge-facing, has already attempted self-build
- **External network (Bergerhoff at BWB):** customer-side, downstream beneficiary

This is a real opportunity to deliver a first end-to-end engagement on a friendly site with a knowledgeable internal counterpart who will not be confused by the technical mechanics.

---

## Patterns Confirmed and New

### Confirmed
- **[[Patterns From Fieldwork]] Pattern 2 — Knowledge trapped at two levels:** "Alles was es an Hintergrundwissen gibt und nicht dokumentiert ist, das geht zwangsläufig verloren."
- **[[Patterns From Fieldwork]] Pattern 13 — Decision-making gap:** Production-planning judgment with three parameters that nobody can articulate as a priority rule.
- **[[Patterns From Fieldwork]] Pattern 22 — ERP ceiling:** The kaufmännische Software covers the standard cases but not the production-planning judgment.
- **[[Patterns From Fieldwork]] Pattern 25 — Under-advised on AI:** Ulrich is technically capable, internally green-lit, motivated, and still couldn't get help. The CBI told him to buy software.
- **[[Patterns From Fieldwork]] Pattern 28 — The campfire method:** Wolf and Ulrich converge unprompted on the storytelling/situational nature of the production-planning knowledge ("dann muss man sich zusammen hinsetzen und irgendwie mal anfangen, Geschichten zu erzählen").

### New

**Pattern 31 — The €20,000 forgotten experiment**
Technically-driven mid-sized firms can quantify the in-period cost of lost institutional knowledge in repeated R&D. Filigran reports a single forgotten test report can cost €20,000 to repeat, plus days of basement archive search that often returns nothing. This is a direct, near-term, measurable ROI for Phase 1 knowledge capture — independent of succession or M&A framing. For engineering-heavy SMEs, this may be the cleanest sales angle.
- **Source:** [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]
- **Strength:** Strong — specific numbers from an in-house technical lead; aligns conceptually with Antonio Rizza's documentation-to-deal-price mapping in [[Interview 008 — Antonio Rizza (M&A)]]

**Pattern 32 — The motivated technical insider blocked at the build step**
Mid-sized industrial firms increasingly have technically-capable internal staff who *want* to build local AI knowledge bases, *get internal approval*, and *fail at implementation* — not because the concept is wrong but because the last 10% (PDF chunking, vector DB integration, Python plumbing) requires expertise they don't have and can't get cheaply. Industrial consortia point them toward commercial licenses they don't want. Universities offer forward-modeling research, not pragmatic backward-looking implementations. The gap is real and articulated.
- **Source:** [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]
- **Strength:** Strong — first-person account of the failed-build sequence with specific failure mode

**Pattern 33 — Trade-association as GTM channel for German industrial Mittelstand**
A single sale into a Fachvereinigung (trade association of sector-specific manufacturers) provides access to many member firms with a shared technical context. Ulrich is already considering proposing this for the lattice-girder concrete trade association. This complements but is distinct from the Italian commercialisti channel — same logic of "warm-multi-customer-via-trusted-aggregator," different sector.
- **Source:** [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]
- **Strength:** Moderate — single source, hypothesis-stage, but concrete and immediately testable through Filigran

---

## Which sub-problem did this touch?

- [x] **Matching** — not directly, though the BWB-Gruppe / trade association angle is an indirect "matching" of solution to multiple buyers
- [x] **Readiness** — strongly. The archival-knowledge problem IS the readiness problem at the engineering layer.
- [ ] **Emotional** — not in this conversation. Ulrich is pragmatic and technical; no visible emotional charge around the knowledge loss beyond mild frustration.
- [x] **Deal-structuring** — indirectly via the Pattern 31 ROI framing. Repeated-experiment cost is a cousin of due-diligence cost.

---

## Upstream or downstream?

**Upstream and operational, not succession-driven.** Ulrich is solving a daily-work problem, not a generational handover. Filigran is structurally facing a succession problem (Stefan's interview), but Ulrich's pain is independent of that — he would want this knowledge base if Stefan were 35 and just took over, or if Stefan were 75 and selling. This validates that the product has standalone operational value separate from the succession narrative — which expands the addressable use case.

This is also a strong data point for the [[Upstream vs Downstream]] question: there exists a non-succession entry-point into engineering-heavy firms that may be *easier* to sell against than the succession framing, because the ROI is in-period and quantifiable rather than long-tail and emotional.

---

## ICP Relevance

Filigran fits the ICP cleanly — 110 employees, third-generation, German, manufacturing, basic ERP, no sophisticated digital tools. Ulrich's role within Filigran is also informative: he is the kind of "internal champion" Prisma identified as a prerequisite for engagement ([[Patterns From Fieldwork]] Pattern 6). He is technically literate, internally credible, motivated, and frustrated. If we were to pilot at Filigran, Ulrich is the natural counterpart on the technical side and Stefan on the strategic side.

For ICP definition: this interview confirms that within a single ICP-fit company there can be **multiple buyers with different value framings** — the CEO buys succession protection, the engineer buys repeated-experiment savings, the M&A advisor (downstream) buys deal-price defense. The product needs to be packageable to each framing without redesign.

---

## Action Items

- [ ] **Priority:** Evaluate Filigran as the first end-to-end pilot site. Combine Stefan's strategic buy-in with Ulrich's technical engagement to design a scoped Phase 1 deliverable around the engineering archive specifically.
- [ ] **Priority:** Get the contact for Stefan Bergerhoff (BWB-Gruppe planning leader). Schedule the conversation. Ulrich will warn Bergerhoff in advance.
- [ ] Follow up with Ulrich in 2–3 weeks with a status update — he asked to stay in contact and to receive updates.
- [ ] Investigate the Fachvereinigung Betonbauteile mit Gitterträgern as a potential trade-association sales channel (Pattern 33).
- [ ] Capture the "€20,000 forgotten experiment" framing for the pitch deck — concrete, quantifiable, near-term ROI.
- [ ] Decide product/service split: do we sell the implementation, or do we publish a Kochrezept that consortium members can use themselves?

---

## Open Questions Raised

- [ ] What is the right Phase 1 deliverable for an engineering-archive use case specifically — is it a different product than the founder-decision-extraction case, or the same methodology with different inputs?
- [ ] Is the "without license costs" preference a temporary cost-sensitivity or a structural ceiling on what Mittelstand technical teams will pay for internal tooling?
- [ ] Is trade-association sales (Pattern 33) more efficient than direct-to-founder outreach for German industrial sectors? How would we pilot it without burning the relationship?
- [ ] Does the engineering-archive use case have different competitive dynamics than the founder-decision-extraction case? Different incumbents, different pricing, different sales cycle?
- [ ] How do we package the product so the CEO buys succession protection and the engineer buys archive search, without confusing either of them about what they're getting?

---

## Related
- [[Interview 012 — Stefan Weiler (Filigran, Germany)]] — same company, CEO view; Stefan sees succession, Ulrich sees daily knowledge loss; together they triangulate the Filigran case
- [[Interview 008 — Antonio Rizza (M&A)]] — documentation-to-deal-price mapping is the M&A-side analogue of Ulrich's repeated-experiment cost
- [[Interview 010 — Newton Campos (Search Fund)]] — Newton's prospective vs retroactive distinction maps directly: Ulrich wants retroactive (60 years of test reports), and his readiness to use the deliverable is high
- [[Interview 011 — Dairy Chemicals Commercial (Italy)]] — "chiavi di lettura" framing aligns with Ulrich's distinction between engineering knowledge (capturable) and production-planning judgment (situational)
- [[Interview 013 — David (Textile Manufacturing, Germany)]] — both are technically literate insiders in German manufacturing; David framed the soft layer (campfire stories), Ulrich frames the hard layer (test report archives)
- [[Patterns From Fieldwork]] — Patterns 31, 32, 33 added; Patterns 2, 13, 22, 25, 28 confirmed
- [[ICP Definition]] — confirms Filigran fits and surfaces multi-buyer dynamic within a single ICP-fit company
- [[Outreach Strategy]] — Pattern 33 (Fachvereinigung channel) is a German analogue of the Italian commercialisti channel
- [[Problem Statement]] — Ulrich's failed-self-build is the most direct product validation in the dataset to date
- [[Competitors]] — CBI Aachen recommended commercial licenses; worth tracking what those vendors are
