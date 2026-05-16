---
title: "MI — Classical Knowledge Elicitation Methods"
tags: [market-intelligence, knowledge-elicitation, expert-systems, methodology]
created: 2026-05-16
---

## Sources

- Shadbolt & Smart — *Knowledge Elicitation* (Evaluation of Human Work, 4th ed., CRC Press, 2015)
- Gavrilova & Andreeva — *Knowledge Elicitation Techniques in a Knowledge Management Context* (JKM, 2012)
- Roth & Binz — *Procedure for Selecting Knowledge Elicitation Methods with Regard to Knowledge Types* (ICED 2013, Stuttgart)
- Carlos III University — *Selecting a Software Elicitation Technique According to Layers of Knowledge and Preciseness* (J.UCS, 2017)

---

## What This Is

Four academic sources covering the canonical knowledge elicitation (KE) literature: techniques, taxonomies, and frameworks for matching elicitation methods to knowledge types. This is the field Solcus implicitly practices — but rarely cites. Understanding KE methodology gives us academic credibility and a richer vocabulary for describing our methodology.

---

## Key Insights Relevant to Solcus

### 1. "The gold is not in the documents"

Shadbolt & Smart cite Hoffman & Lintern (2006) directly:

> *"The gold is not in the documents. Document analysis is useful in bootstrapping researchers into the domain of study... but experts possess knowledge and strategies that do not appear in documents and task descriptions. Cognitive engineers invariably rely on interactions with experts to garner implicit, obscure, and otherwise undocumented expert knowledge."*

**Solcus angle:** This is our value proposition in one sentence. RAG tools (Notion AI, Guru, Tettra) only work on what's already documented. Solcus goes for the gold that isn't in any document — by talking to the expert.

### 2. The knowledge acquisition bottleneck

Shadbolt & Smart: in expert systems research, it consistently took longer to elicit knowledge from experts than to build the actual software. This "knowledge acquisition bottleneck" (Hayes-Roth et al., 1983) is still unresolved — it's now a bottleneck in AI model training.

**Solcus angle:** We are explicitly in the business of solving the knowledge acquisition bottleneck for SMEs. This reframes our service not as "knowledge management" but as "the missing infrastructure for expert knowledge capture."

### 3. Natural vs contrived elicitation techniques

Shadbolt & Smart distinguish:
- **Natural methods:** Expert does what they'd normally do — interviews, observation, think-aloud. Comfortable, but limited to what can be verbalized
- **Contrived methods:** Expert performs an unfamiliar task designed to surface knowledge differently — concept sorting, repertory grid, scenario walkthroughs. Uncomfortable, but often more efficient and surfaces knowledge the expert couldn't articulate in an interview

Key finding: "An expert's own opinion of the worth of a technique is no guide as to its actual value" — meaning experts often resist contrived methods that actually yield the richest knowledge.

**Solcus angle:** The campfire method is natural. Storyboarding and structured scenario walkthrough are contrived. A robust Solcus engagement needs both. Don't let the founder reject the contrived parts because they feel uncomfortable — that discomfort is productive.

### 4. Structured interview with fixed probes (Shadbolt & Smart)

The most practical Solcus takeaway: a proven probe protocol for extracting decision rules from experts:

| Probe | Function |
|-------|----------|
| "Could you tell me about a typical case?" | Domain overview |
| "Why would you do that?" | Converts assertion into rule |
| "How would you do that?" | Generates lower-order rules |
| "When would you do that?" | Reveals generality/scope of rule |
| "What alternatives are there?" | Generates more rules |
| "What if [condition] were not the case?" | Rules for edge cases |
| "Can you tell me about an unusual case?" | Rare cases and special procedures |

**Solcus angle:** These probes should be built into our structured session script. They are particularly powerful in Session 2 (structured extraction) after Session 1 (campfire narrative) has surfaced the raw material.

### 5. Taxonomy: analyst-leading vs expert-leading vs collaborative (Gavrilova & Andreeva 2012)

| Type | Methods | Tacit knowledge yield |
|------|---------|----------------------|
| Analyst-leading | Interview, questionnaire | Low (*** for explicit, * for tacit) |
| Expert-leading | Observation, storytelling, round-table, brainstorming | Medium-High |
| Collaborative | Role game, verbal protocols | Highest (*** for tacit) |

Best methods for tacit knowledge specifically:
- **Role game (****):** Expert acts out decision scenarios; cognitive processes surface naturally
- **Observation (***):** Watch the expert doing actual work; access to routinized, automatized knowledge
- **Brainstorming (***):** Group dynamics surface knowledge through association

**Solcus angle:** Our campfire method is expert-leading (storytelling + brainstorming). For the deepest tacit extraction, we should consider adding a role-game element: "Let's replay the situation where you decided to drop client X — what were you reading in that conversation?"

### 6. Matching methods to knowledge types (Roth & Binz 2013)

9 knowledge types × 11 method abilities matrix. Key finding for Solcus:
- **Business strategy knowledge:** Unstructured interview is the best-matched method
- **Procedural/process knowledge:** Observation and structured interview
- **Causal/relational knowledge:** Concept mapping and knowledge graphs

**Solcus angle:** The founder's strategic knowledge (which markets to enter, which clients to drop, how to read a negotiation) is best surfaced by unstructured interview first — then formalized into structured rules.

### 7. Three knowledge layers (Carlos III, 2017)

| Layer | Type | Best method |
|-------|------|-------------|
| Strategic | Decision-making, judgment, values | Unstructured interview |
| Task | Procedures, activities, workflows | Structured interview |
| Domain | Concepts, relationships, terminology | Concept mapping |

Product Pattern technique achieves 94% preciseness for domain knowledge capture.

**Solcus angle:** Our Phase 1 engagement spans all three layers — but we typically do them in wrong order (domain first, strategic last). Evidence suggests starting at the strategic layer (which only unstructured interview unlocks) and working downward.

---

## What We Can Learn

1. **Academic framing:** Solcus practices knowledge elicitation, not just "knowledge transfer." Using the right vocabulary unlocks academic credibility and investor confidence
2. **The acquisition bottleneck is our pitch:** We solve the oldest unsolved problem in AI — how to get expert knowledge into a machine at scale
3. **Probe script:** Build the Shadbolt & Smart fixed probes into our structured session guide
4. **Role game as upgrade:** Add a replay/role-play element to Phase 1 for accessing the deepest tacit layers (currently missing from our methodology)
5. **Layer sequencing:** Start with strategic (unstructured campfire) → task (structured walkthrough) → domain (concept mapping/graph)

---

## Related

- [[MI — Storytelling and Tacit Knowledge Capture]] — practitioner perspective on same techniques
- [[MI — Knowledge Elicitation for AI and ML]] — applying KE to LLM infusion
- [[MI — Classical Knowledge Elicitation Methods]] — this note
- [[Patterns From Fieldwork]] — Pattern 28 (Campfire), Pattern 35 (three trust thresholds)
- [[MI — Neurofeedback for Corporate Brain Health (KEDAS Clinics)]] — psychological preconditions for knowledge transfer
