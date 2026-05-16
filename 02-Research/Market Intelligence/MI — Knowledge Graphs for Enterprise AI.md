---
title: "MI — Knowledge Graphs for Enterprise AI"
tags: [market-intelligence, knowledge-graph, enterprise-AI, architecture]
created: 2026-05-16
---

## Sources

- Atomicwork Blog — *Enterprise Knowledge Graphs: Why in the Age of AI Agents, Context Is King* (n.d.)
- Glean Blog (Rob Stets) — *How Knowledge Graphs Work and Why They Are the Key to Context for Enterprise AI* (n.d.)
- Althire AI — *LLM-Powered Knowledge Graphs for Enterprise Intelligence and Analytics* (arXiv 2503.07993, 2025)

---

## What This Is

Three practitioner and research sources on knowledge graphs as the technical infrastructure for enterprise AI. These sources explain why flat document stores fail, what knowledge graphs add, and how LLMs can help build them. Directly relevant to Solcus Phase 2 architecture — the graph is the long-term technical substrate, not just a nice-to-have.

---

## Key Insights Relevant to Solcus

### 1. Four context types enterprise AI needs (Atomicwork)

Modern enterprise AI agents need four types of context to function as "informed insiders":

| Context type | What it contains |
|-------------|-----------------|
| **People context** | Who knows what, relationships, org chart, expertise map |
| **Asset context** | Documents, files, projects, systems |
| **Knowledge context** | Decisions, policies, processes, FAQs |
| **Tribal context** | Unwritten rules, institutional memory, "how we do things here" |

The tribal context is what document-first tools completely miss — and what Solcus specialises in capturing.

**Solcus angle:** Our Phase 1 extraction directly targets the tribal context — the category AI agents need most and can get least from existing documents. This framing positions Solcus as "tribal context infrastructure" rather than document indexing.

### 2. AI agents as "informed insiders, not external assistants"

Atomicwork: the difference between a useful AI agent and a generic chatbot is whether the agent has organisational context. Without the knowledge graph, the agent is a stranger who just arrived. With it, the agent is the person who's been there for 20 years.

"When you onboard the knowledge graph, the agent becomes oriented" — same as a new employee who gets the full briefing.

**Solcus angle:** Our product isn't just for the founder's memory — it's for training the AI agent that will work alongside the successor. The graph we build in Phase 1 is the agent's onboarding document. This is a strong Phase 2 pitch: "the knowledge we extract in Phase 1 becomes the brain of your AI assistant."

### 3. Knowledge graph structure: triplets (Glean)

All knowledge graphs are built on the same primitive: **subject → predicate → object**

Examples:
- `Founder → always_calls → key clients before holidays`
- `Client X → requires → invoice by 25th of month`
- `Tender in Bavaria → needs → personal relationship with municipal official`

This structure enables multi-hop reasoning: "Who knows how to handle clients in the public sector?" → AI traverses: person → expertise → client type → sector → relationship.

Flat document stores can answer: "What does our CRM say about client X?" Knowledge graphs can answer: "What do we know about how we win in this kind of situation?"

**Solcus angle:** Our extraction process should explicitly capture triplet-form relationships, not just narrative. The campfire method produces stories. The structured session should convert stories into (subject, predicate, object) triples — that's what makes the knowledge graph machine-queryable.

### 4. LLMs struggle with the queries knowledge graphs solve (Glean)

LLMs are trained for next-token prediction. They fail at:
- Multi-hop reasoning ("who in our team knows X, and what projects did they work on?")
- Deterministic queries ("what's the exact client list for this territory?")
- Provenance ("where did this knowledge come from, and is it still valid?")

Knowledge graphs solve all three. The combination of LLM (for understanding language, generating responses) + knowledge graph (for structured, verifiable context) is now called **GraphRAG**.

**Solcus angle:** Our Phase 2 architecture should be GraphRAG, not flat RAG. Flat RAG (Notion AI, Guru) works on documents but fails on relationships. GraphRAG works on relationships — which is exactly what founder knowledge is made of.

### 5. LLM-powered knowledge graph construction (Althire AI, arXiv 2503.07993)

Althire AI built a framework for automatically constructing activity-centric knowledge graphs from enterprise data using LLMs. Key capabilities:
- **Entity extraction:** People, skills, projects, relationships from unstructured data (92% accuracy in 6-month pilot)
- **Relationship inference:** Inferring connections not explicitly stated
- **Semantic enrichment:** Adding context and metadata to entities

Pilot (finance + healthcare, 6 months): entity extraction at 92% accuracy. Used for expertise discovery, task prioritization, and team analytics.

**Solcus angle:** This is the Phase 2 automated pipeline. Phase 1 = human-assisted extraction (our engagement). Phase 2 = Althire-style automated construction from ongoing organizational data (Slack, emails, call transcripts). The 92% accuracy stat means the automated layer needs human validation — we remain in the loop.

### 6. Enterprise privacy is a structural moat (Glean)

Public knowledge graphs (DBpedia, Wikidata) are built on open data. Enterprise knowledge graphs require handling confidential data — client relationships, internal decisions, pricing strategies, personnel information. Privacy constraints mean enterprises cannot use public graph-building infrastructure.

This creates a structural barrier: you can't just "plug in" a commodity graph service. Someone has to build the graph in a trust-first environment.

**Solcus angle:** Our on-site engagement model (founder trusts us because we're present, not because we're a SaaS tool) is exactly right for the privacy-sensitive layer. The knowledge that matters most — who you fired and why, which deals you killed, how you actually structured that partnership — will never enter a cloud-based tool voluntarily. Our high-touch model is the privacy moat.

---

## What We Can Learn

1. **Architecture direction = GraphRAG:** Not flat document retrieval but graph-based reasoning over extracted knowledge
2. **Tribal context as category:** We extract "tribal context" — the fourth and most valuable context type that document-first tools can't reach
3. **Triplet extraction:** Structured sessions should explicitly capture (subject, predicate, object) relationships, not just narrative summaries
4. **Phase 1 → Phase 2 pipeline:** Phase 1 extraction (human-assisted) creates the seed graph; Phase 2 automation (LLM pipeline) maintains and extends it
5. **Privacy moat:** The most valuable knowledge is privacy-sensitive and will only be captured in a trust-first, on-site engagement model — this is our competitive moat vs. SaaS-first competitors

---

## Related

- [[MI — Contextual Blindness and Knowledge Graphs (LinkedIn)]] — "Context Tax" and provenance trace
- [[MI — Knowledge Elicitation for AI and ML]] — bridging extracted rules to AI-usable format
- [[MI — Context Farming for Company Second Brain (YouTube)]] — Phase 2 automated maintenance layer
- [[MI — Company Brain Concept (Ability.ai, Falconer, YC)]] — four-property framework for company knowledge
- [[Competitors]] — Glean, Guru, Tettra as flat-RAG competitors
