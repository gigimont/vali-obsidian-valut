# Interview 022 — Marco Nortmeier (Filigran, Germany)

#research #interview #internal-it #filigran #internal-network #manufacturing #germany #pilot-enabler

> **Date:** May 13, 2026
> **Interviewee:** Marco Nortmeier — Head of IT, Filigran (German operations)
> **Sector:** Steel / construction (Filigran lattice girders for precast concrete elements)
> **Geography:** Germany (Filigran HQ in Lese, Niedersachsen)
> **Connection:** Introduced via Joerg von Weiler ([[Interview 015 — Joerg von Weiler (Filigran Poland)]]); pre-call between Joerg and Marco two days before this interview established context
> **Format:** Video call in German, switched to du-form mid-call at Wolf's suggestion (transcript available)
> **Follow-up:** Wolf in Lese / Blenhorst over Pfingsten weekend (May 22-24); potential in-person meeting to demonstrate Obsidian setup; Wolf to discuss approach with Joerg in parallel

---

## ⚠️ Significance of This Interview

**Marco is the first internal-IT-lead voice in the dataset, and his interview completes the internal stakeholder alignment at Filigran.** Filigran has now produced three converging internal endorsements:
- **Strategic level:** Stefan Weiler (CEO, [[Interview 012 — Stefan Weiler (Filigran, Germany)]]) — explicit "we have no plan to preserve knowledge"
- **Technical-domain level:** Ulrich Bauermeister (engineer, [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]]) — failed self-build of local LLM + vector DB; concrete €20K-per-forgotten-experiment ROI
- **Internal-IT/operational level:** Marco Nortmeier (this interview) — head of IT, methodological alignment with our approach, verbal endorsement of starting small with a Bauermeister recording-and-transcription pilot

This is the first time in the dataset that all three of Pattern 35's trust thresholds have been positively aligned within a single company. Filigran is no longer a hypothetical sandbox — it is a verbally-greenlit pilot site pending only logistical sequencing.

**Marco also delivered the second independent confirmation of Francis's transformation-gap insight from inside an operating company.** Francis ([[Interview 020 — Francis de Vericourt (ESMT Professor)]]) said the methodology bridge between raw data and useful knowledge is the unarticulated moat. Marco, unprompted, described exactly how Filigran builds that bridge in practice: rather than dumping data into AI, he and his programmer decide what information is needed and structure it at the data-source level, with the AI essentially "already in his head" when he frames the data architecture. This is methodological confirmation from a practitioner that the moat lives in the framing, not in the model.

**Finally, Marco unprompted articulated the demonstration value of the Obsidian second-brain approach.** When Wolf showed the live Obsidian graph view, Marco immediately understood and named the cross-source verification benefit: "wenn ich es nur einmal drin stehen habe, dann ist es vielleicht ein Einzelfall... je mehr Überschneidung ich habe, desto mehr kann ich davon ausgehen, dass es relevant ist." This is *external validation of the pitch deck Slide 7 thesis* (we walk the walk; the methodology is the demo) — articulated by a customer-side viewer who reached the framing himself.

---

## Context

Marco is Head of IT at Filigran's German operations. The conversation was set up by Wolf's father Joerg, who had a preliminary discussion with Marco two days prior to align on context. Joerg framed the topic to Marco as: (1) AI for efficiency and production planning at Filigran, and (2) the broader Wissenstransfer concept from Wolf's project.

The interview itself ran ~45 minutes. Wolf and Marco switched from Sie to du early on at Marco's invitation, signaling Marco was comfortable with informal peer-to-peer engagement despite the age and authority gap. The conversation moved through Marco's general AI views, his specific work at Filigran, the methodology Wolf and Giuseppe are developing, a live Obsidian demonstration, and ended with a verbal yes to a Filigran-Bauermeister pilot start plus a potential in-person meeting over Pfingsten.

Marco's role is structurally distinct from the other Filigran interviewees: Stefan is the strategic authorizer, Bauermeister is the bottleneck domain expert, Marco is the operational enabler. He is the person who would actually integrate any pilot into the existing systems landscape, navigate the GDPR question, and provide the data-architecture context.

---

## Key Quotes

> "Grundsätzlich ist das Thema KI ja immer so ein bisschen Fluch und Segen zugleich... KI schmeißt einem immer genau das Ergebnis raus, was man denn vielleicht auch gerade hören will." *(opening, on critical engagement with AI outputs)*

> "Was uns die ganze Geschichte grundsätzlich noch ein bisschen erschwert, ist natürlich das Thema Datenschutz und europäische Datenschutzgrundverordnung... eigentlich ein eher zu vernachlässigendes Thema, meine Meinung, also es erschwert mehr als dass es hilft." *(pragmatic acknowledgment of GDPR as a friction, not a blocker)*

> "Information schadet nur demjenigen, der sie nicht hat."

> "Ich sehe eigentlich nur zu, dass ich mit den vorhandenen Systemen einfach möglichst viel abbilde... die KI hat dann quasi schon — ich sag das jetzt mal überspitzt — bei mir im Kopf angesetzt, wo ich unserem Programmierer gesagt habe: pass auf, in meinem ERP-System hätte ich gerne die und die Informationen abrufbar." *(the methodology-not-model framing — independent confirmation of Francis's transformation-gap argument)*

> "Damit kommen wir raus aus 'Ich schmeiß die Informationen in eine KI und die KI wertet es mir aus', sondern ich habe mir Gedanken drüber gemacht, was brauchen wir, und die Informationen als Auswertung letztendlich bereitgestellt."

> "Wenn dann an irgendeiner Stelle mal irgendein Systemupdate kommt, sei es von Microsoft, sei es vom ERP-Anbieter, sei es von den Schnittstellen-Dienstleistungen, wie auch immer, dann muss es natürlich nachdokumentiert werden. Und das ist in der Regel das, was dann eher am wenigsten stattfindet." *(documentation entropy under external system change — new pattern)*

> "Speichere ich im Kopf ab, aber ist halt leider für die Nachwelt nirgendwo dann dokumentiert. Und das findet leider viel zu häufig statt, egal in welchen Unternehmen."

> "Wenn der und derjenige sich gleich mit seiner Aussage zu dem Thema mit dem und demjenigen deckt, je mehr Überschneidung ich habe, desto mehr kann ich davon ausgehen: ja, das ist halt überall dasselbe und es ist ein relevantes Thema." *(unprompted articulation of the cross-source verification value — external validation of pitch Slide 7 framing)*

> "Also machen wir's." *(verbal yes to starting a Filigran pilot)*

---

## What We Learned

### The internal-IT-lead's methodology mirrors the transformation-gap solution (PRODUCT-DESIGN VALIDATION)

Marco described his actual working approach at Filigran:
1. He identifies what information he needs at the business level
2. He briefs his programmer to make that information accessible inside the ERP system
3. The AI (where used) consumes pre-structured data — "die KI hat dann bei mir im Kopf angesetzt"
4. He does not dump unstructured data into a model and ask the model to figure it out

This is — independently and from an operational position — the answer to Francis de Vericourt's "transformation gap" challenge ([[Interview 020 — Francis de Vericourt (ESMT Professor)]]). Francis said: between three-pillar data collection and "second brain" output, there is an unarticulated transformation step. Marco's working method *is* that transformation step expressed practically. The methodology lives in the framing of the question and the structuring of the data sources, not in the model.

**Implication:** Marco is methodologically aligned with the direction Francis pointed us toward, before either of them have spoken to each other. This is the strongest signal yet that the transformation-gap framing is correct and that the methodology — not the AI — is the moat. The product positioning shift to "specialized consulting practice with proprietary AI-enabled methodology" (Francis's Challenge 1) is reinforced.

### The internal stakeholder alignment at Filigran is complete

Pattern 35 from [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]] identified three distinct trust thresholds within a single ICP-fit company: technical, commercial/operational, strategic. Filigran now has all three positively aligned:

| Level | Person | Interview | Status |
|---|---|---|---|
| Strategic / Ownership | Stefan Weiler (CEO) | [[Interview 012 — Stefan Weiler (Filigran, Germany)]] | "We have no plan to preserve knowledge" — explicitly named the problem |
| Technical-domain | Ulrich Bauermeister | [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]] | Failed self-build; €20K/forgotten-experiment ROI; introduced Bergerhoff externally |
| Internal-IT/operational | Marco Nortmeier | This interview | Methodological alignment; verbal yes to pilot start; offered private mobile contact |

**Implication:** Filigran is the first company in the dataset where all three layers of Pattern 35 have produced positive signals. This is a meaningful project-state change. Filigran is no longer hypothetical — it is a verbally-greenlit pilot site pending only logistical sequencing.

**Reservation:** Wolf's note in earlier strategic discussions had been to *avoid* Filigran as the beta site for credibility reasons (independence preferred). That principle remains valid. But the question now is different: not "should Filigran be the beta?" but "should Filigran be the first internal proof-of-concept (low-stakes, exploratory) while an independent beta is sought in parallel?" Two-track approach worth discussing with Giuseppe.

### Documentation entropy: external system changes break internal documentation

Marco articulated something sharper than prior versions of Pattern 22 (ERP ceiling). He said: when external systems change (Microsoft updates, ERP supplier updates, interface partner changes), the internal documentation that was once accurate becomes stale — and the nachdokumentation that should follow is the thing that almost never happens.

> "Okay, war die letzten drei Jahre so, das und das ändert sich jetzt, speichere ich im Kopf ab, aber ist halt leider für die Nachwelt nirgendwo dann dokumentiert. Und das findet leider viel zu häufig statt, egal in welchen Unternehmen."

This is a temporal dynamic that prior patterns have not captured. Pattern 2 (knowledge trapped) is static. Pattern 22 (ERP ceiling) is structural. Marco's observation is dynamic: even well-documented knowledge decays under change pressure because the maintenance discipline breaks down. The product must address not just initial capture but ongoing capture under external-system pressure.

**Implication:** Any pilot must explicitly include a maintenance mechanism — passive (AI-driven incremental updates) or active (scheduled re-validation). This is exactly the kind of methodology question the Hubi-three-way conversation should explore. It is also a real product constraint that will surface in every paid engagement.

### GDPR as friction, not blocker (pragmatic internal-IT view)

Marco — the person who would have to navigate GDPR if a Filigran pilot proceeded — was explicit:

> "Was uns die ganze Geschichte grundsätzlich noch ein bisschen erschwert, ist natürlich das Thema Datenschutz und europäische Datenschutzgrundverordnung... eigentlich ein eher zu vernachlässigendes Thema, meine Meinung."

His pragmatism is useful but specific to his role. The deal-breaker hypothesis #2 in [[Problem Statement]] (data access) remains real for external prospects who do not have this disposition. Marco's view is one data point in favor; it does not retire the concern.

**Implication:** GDPR will surface differently with different internal stakeholders. Pragmatic IT leads will see it as friction. Risk-conscious legal departments and works councils (Betriebsrat) will see it as a blocker. The product methodology needs a clean GDPR story before any external pilot proceeds. For the Filigran internal proof-of-concept, Marco's pragmatism is sufficient — but we cannot generalize from it.

### Unprompted articulation of the Obsidian-as-demo value

When Wolf showed Marco the live Obsidian graph view of the project's research vault, Marco immediately articulated the cross-source verification value without being prompted:

> "Wenn ich es nur einmal drin stehen habe, dann ist es vielleicht ein Einzelfall... je mehr Überschneidung ich habe, desto mehr kann ich davon ausgehen: ja, das ist halt überall dasselbe und es ist ein relevantes Thema."

This is the pitch deck Slide 7 thesis ("we walk the walk; we built a queryable second brain ourselves") said back to us by a customer-side viewer who reached the framing himself. It is the strongest external validation we have for the "methodology is the demo" framing.

**Implication for [[Pitch Deck Content]]:** The Slide 7 framing is empirically working with technically-fluent customer-side viewers. Marco's unprompted articulation is a quote we could use, in anonymized form, on the deck or in supporting materials.

### A verbal yes to a Filigran-internal pilot

Wolf proposed an explicit starting point: Marco sits with Bauermeister, has a recorded conversation, the conversation is transcribed, and starts to feed the early version of an internal Filigran knowledge artifact. Marco's response: *"Also machen wir's."*

This is a verbal commitment to start, made by the person who has operational authority to enable it. It is not yet a written commitment, not yet scheduled, and explicitly contingent on Wolf's Pfingsten visit and a parallel discussion with Joerg. But it is more than any prior pilot conversation has produced.

**Implication:** The next step is not another interview. It is the operational kickoff of an internal Filigran exercise. This is the project's first meaningful state change from research mode to delivery mode (even if exploratory and low-stakes).

---

## Patterns Confirmed and New

### Confirmed
- **[[Patterns From Fieldwork]] Pattern 2 — Knowledge trapped:** Marco's "speichere ich im Kopf ab" line is a precise self-aware admission of the pattern at the IT-lead level.
- **[[Patterns From Fieldwork]] Pattern 22 — ERP ceiling:** Marco's framing of the ERP as captured-information-but-not-judgment is the operational version of this pattern, viewed from inside.
- **[[Patterns From Fieldwork]] Pattern 25 — Under-advised on AI:** Marco explicitly avoids generic AI tools (ChatGPT, Gemini, Copilot) in favor of bespoke data structuring — implicit acknowledgment that off-the-shelf AI doesn't fit the SME use case.
- **[[Patterns From Fieldwork]] Pattern 29 — Tech must not feel like tech:** Marco articulates this from the IT side — he doesn't pitch his work as "AI" internally, he pitches it as "information available where needed."
- **[[Patterns From Fieldwork]] Pattern 35 — Three trust thresholds within one company:** All three thresholds at Filigran now positively aligned across Interviews 012, 014, and 022. First fully aligned case in the dataset.
- **[[Patterns From Fieldwork]] Pattern 39 — Partial-capture honesty principle:** Marco's "99,9999% aber nie 100%" framing is a practitioner's version of Francis's honesty principle.

### New

**Pattern 40 — Documentation entropy under external system change**
Even well-documented organizational knowledge decays under temporal pressure from external systems. When Microsoft, ERP suppliers, or interface partners push updates, the internal documentation that was once accurate becomes stale — and the nachdokumentation that should follow almost never happens, because the maintenance is high-effort and triggered by external rather than internal events. Distinct from static knowledge-trapped patterns: this is a dynamic decay pattern. Any product must address not just initial capture but ongoing capture mechanism under external-change pressure. Passive (AI-driven incremental updates) or active (scheduled re-validation) — both are open methodology questions.
- **Source:** [[Interview 022 — Marco Nortmeier (Filigran, Germany)]]
- **Strength:** Strong — articulated by an internal IT lead from direct operational experience; consistent across "egal in welchen Unternehmen" framing

---

## Strategic Implications

### Filigran becomes the first internal proof-of-concept candidate (not the beta)

This is a meaningful project-state change. The three internal stakeholders at Filigran are now positively aligned, and Marco has given a verbal yes to start small. The original decision to seek an independent beta partner for credibility reasons remains valid for the *external* proof of concept that we'll show investors and prospects. But Filigran is now usable as a parallel, lower-stakes internal proof of concept — a place to develop the methodology and stress-test the approach without external visibility.

**Recommended two-track approach:**
- **Track 1 — Filigran internal exploration.** Bauermeister × Marco conversation, recorded and transcribed, fed into an early version of the artifact. Low stakes. Methodology development. No external claims.
- **Track 2 — Independent external beta search.** Continue sourcing an unrelated beta partner for the credibility-grade proof of concept. Hubi/AWW is the leading candidate. Bergerhoff/BWB and Hubi's AI buddy form parallel technical partnerships.

These two tracks can run simultaneously and inform each other. The internal Filigran exploration may surface methodological insights that strengthen the external beta proposition.

### Parallel pilot pathways: Filigran and AWW have structurally similar setups

The Hubi-three-way meeting framing (use case + technical + methodology, [[Interview 018 — Hubertus von Huelsen (AWW, Germany)]]) and the Filigran configuration (Stefan + Bauermeister + Marco) are structurally analogous:

| Component | Filigran | AWW |
|---|---|---|
| Strategic authorization | Stefan Weiler (CEO) | Hubi himself (CEO returning) |
| Bottleneck domain expert | Ulrich Bauermeister (engineer) | Tool-making shop senior |
| Technical implementation pathway | Marco Nortmeier (internal IT) | Hubi's external AI consulting buddy |
| Methodology layer | Wolf + Giuseppe | Wolf + Giuseppe |
| Narrow, bounded use case | Engineering archive | Tool-making knowledge |
| Verbal yes status | "Also machen wir's" (Marco) | Three-way meeting proposed and agreed |

We now have **two parallel candidate pilot configurations**, structurally similar, with different technical-partner pathways (internal IT for Filigran, external AI consultant for AWW). This is a project asset: we don't have to bet on one. We can develop both and let the timing and pull determine which materializes first.

### The methodology-not-model framing has independent triple confirmation

Three sources have now independently arrived at the same conclusion:
- **Francis de Vericourt ([[Interview 020]]):** The transformation gap is the moat. Methodology, not technology.
- **Roland Wübbe ([[Interview 021]]):** Atrophy critique implicitly demands methodology that scaffolds rather than substitutes — the model is not the answer.
- **Marco Nortmeier (this interview):** Practitioner version — "Die KI hat schon bei mir im Kopf angesetzt." Architecture, framing, and data structuring are the work.

This is now a confirmed strategic direction. The [[Pitch Deck Content]] identity reframe (Francis's Challenge 1 — "specialized consulting practice with proprietary AI-enabled methodology") is reinforced by an independent practitioner voice.

---

## ICP Relevance

Filigran fits the primary ICP. Marco's role (internal IT lead, ~110 employees, organically grown family manufacturing) is structurally adjacent to the Pattern 35 multi-buyer model. This interview does not change ICP — but it confirms that the role-based ICP question first raised by Bergerhoff (Interview 016) is the right framing. The motivated technical insider profile (Pattern 32) generalizes across both engineering experts and internal IT leads.

**Action:** When updating [[ICP Definition]] to reflect the role-based vs size-based question, include "internal IT lead with operational authority" as a profile alongside "domain technical expert (engineer, planning leader, tool-maker)."

---

## Action Items

- [ ] **PRIORITY:** During Wolf's Pfingsten weekend in Lese (May 22–24), arrange in-person meeting with Marco. Demonstrate Obsidian setup live. Discuss Bauermeister × Marco recorded-conversation pilot logistics.
- [ ] **PRIORITY:** Discuss with Giuseppe: formally adopt the two-track approach (Filigran internal exploration + independent external beta search). Document in [[Pivot History]] or equivalent.
- [ ] Discuss with Joerg in parallel: Filigran-internal proof of concept positioning. Joerg's buy-in is the strategic enabler for Marco and Bauermeister to coordinate operationally.
- [ ] Update [[Pitch Deck Content]] Slide 7 with Marco's unprompted articulation of the cross-source verification value (anonymized quote).
- [ ] Update [[Problem Statement]] deal-breaker hypothesis #2 (data access) to reflect Marco's pragmatic IT-lead view as a positive data point — without retiring the concern for external prospects.
- [ ] Add "ongoing maintenance under external system change" (Pattern 40) to [[Product Methodology]] as an explicit methodology requirement, not an open question.
- [ ] In the Hubi-three-way conversation, raise Pattern 40 (documentation entropy) as a methodology question to explore jointly with the AI consulting partner.
- [ ] Develop a clean GDPR positioning statement before any external paid pilot. Marco's pragmatism is internal-IT-specific and not generalizable.

---

## Open Questions Raised

- [ ] What is the maintenance mechanism for the captured artifact under external system change (Pattern 40)? Passive AI-driven incremental updates? Scheduled re-validation? Hybrid? This is a methodology question that must be answered before any paid engagement.
- [ ] Should "internal IT lead with operational authority" be a named role profile in [[ICP Definition]] alongside the domain technical expert profile?
- [ ] Should the Filigran internal proof-of-concept (Track 1) be formally documented and version-controlled in Obsidian as it develops, even if not shared externally? If yes, where in the vault structure does it sit?
- [ ] What is the right framing for an internal Filigran exercise that is *not* a paid beta but *is* methodology development? Pricing, scope, ownership of any artifact produced, and use rights all need to be thought through before starting.

---

## Related
- [[Interview 012 — Stefan Weiler (Filigran, Germany)]] — strategic authorization for the Filigran configuration
- [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]] — bottleneck domain expert; introduced Bergerhoff externally; the natural counterpart for Marco in the proof-of-concept pilot
- [[Interview 015 — Joerg von Weiler (Filigran Poland)]] — introducer; ongoing strategic enabler for any internal Filigran activity
- [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]] — Pattern 35 (three trust thresholds) source; now empirically validated by Filigran's complete alignment
- [[Interview 018 — Hubertus von Huelsen (AWW, Germany)]] — parallel pilot configuration with structurally similar setup; the AI-consulting-buddy three-way is the external analogue of the Filigran internal exploration
- [[Interview 020 — Francis de Vericourt (ESMT Professor)]] — the transformation-gap thesis that Marco's working methodology independently confirms; the identity reframe to "consulting practice with proprietary methodology" gains a third reinforcement
- [[Interview 021 — Roland Wübbe (H&W Tiefbau, Germany)]] — atrophy critique implicitly demands the methodology-not-model framing that Marco operationally embodies
- [[Patterns From Fieldwork]] — Pattern 40 added; Patterns 2, 22, 25, 29, 35, 39 confirmed
- [[ICP Definition]] — internal IT lead profile to be added alongside domain technical expert
- [[Pitch Deck Content]] — Slide 7 framing validated by Marco's unprompted articulation; identity reframe further reinforced
- [[Product Methodology]] — Pattern 40 (ongoing maintenance) needs to be added as an explicit methodology requirement; the Marco "KI im Kopf angesetzt" framing should be incorporated as a working principle
- [[Problem Statement]] — deal-breaker hypothesis #2 (data access) has its first positive internal-IT view; concern not retired for external prospects
