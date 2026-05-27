# MI — Contextual Blindness and Knowledge Graphs (LinkedIn)

#market-intelligence #knowledge-graph #technical-architecture #company-brain

> **Source:** LinkedIn post by Sreeram Nudurupati — "Why Your Internal AI Is Blind (And How to Fix the 'Missing Middle')"
> **Published:** ~2024-2025 (no exact date)
> **Date captured:** May 2026
> **Type:** LinkedIn post — technical architecture perspective

---

## What This Says

Short but precise post naming a specific failure mode of enterprise internal AI: **contextual blindness** — when an AI agent finds one piece of the picture but misses the connected whole.

Example: "Who is working on the GPU memory issues for Project Orion?" The agent finds a Slack thread from three weeks ago but misses the Jira ticket with the fix and the GitHub commit that actually resolved it. Each piece of truth lives in a different tool. The AI can't bridge them.

The proposed solution: **Knowledge Graphs** (specifically GraphRAG + ArangoDB) to create a "nervous system" for the enterprise — mapping entity relationships across siloed tools so the AI can walk the full semantic path from conversation to resolution.

Three benefits claimed:
- **Explainable AI (XAI)** — every answer has a provenance trace, no black box hallucinations
- **Operational auditability** — detect gaps between management tools and technical reality
- **Organizational velocity** — eliminate the "Context Tax" (hours lost per week to context fragmentation)

---

## Key Insights Relevant to Solco

### 1. "Contextual blindness" = the SME succession failure mode, named precisely

The example is digital (Slack + Jira + GitHub). The SME succession version is: the successor asks how to handle a difficult supplier — the documents say one thing, the email history shows a different precedent, and the actual answer lives in the founder's head from a conversation 3 years ago. Each piece in a different "tool" (including the founder's memory). No RAG system can bridge these.

- **Solco cross-reference:** Pattern 40 ([[Interview 022 — Marco Nortmeier (Filigran, Germany)]]): documentation entropy — knowledge exists across systems but the connections between pieces decay. Our extraction methodology addresses contextual blindness by surfacing the connections during campfire interviews: "you mentioned the supplier issue — what's the context behind that relationship?"

### 2. "Context Tax" = the quantifiable cost of knowledge fragmentation

Sreeram uses "Context Tax" to name the hours lost per week to engineers bridging siloed knowledge. This is a pitch-ready term for the cost our product eliminates.

- **Solco cross-reference:** The successor's 2-year onboarding is the ultimate Context Tax. Every week they spend asking "why do we do it this way?" and getting partial answers is a Context Tax payment. Solco eliminates the tax by making the context queryable on Day 0.

### 3. Knowledge graph as architecture = long-term Solco technical direction

The knowledge graph approach (entities + relationships) is more powerful than flat RAG for organizational knowledge because it preserves the semantic connections between knowledge pieces. "The nervous system for the enterprise."

- **Solco cross-reference:** Product architecture note. Our current vault (Obsidian + markdown + wikilinks) is already a primitive knowledge graph — wikilinks are edges, notes are nodes. As we move toward a queryable product, the knowledge graph architecture (GraphRAG) is the right direction. Obsidian's graph view is a visual demonstration of this. Worth discussing with CTO candidate.

---

## What We Can Learn

1. **"Contextual blindness"** — add to pitch vocabulary. "Your successor is contextually blind — they have fragments but can't bridge them."
2. **"Context Tax"** — use alongside the 25% time stat (Atlassian) and 2.5 hours/day (Mem) for quantifying the problem.
3. **Knowledge graph as architecture** — plan Solco technical stack around graph-based retrieval, not flat RAG. Start simple (Obsidian wikilinks), evolve toward GraphRAG.
4. **Provenance trace = trust** — every answer from the knowledge base should cite which interview, document, or observation it came from. This is the "explainable AI" property that builds trust with skeptical clients like Marco.

---

## Related
- [[Second Brain Landscape]] — broader landscape
- [[MI — Company Brain Concept (Ability.ai, Falconer, YC)]] — same problem from product perspective
- [[Interview 022 — Marco Nortmeier (Filigran, Germany)]] — Pattern 40: documentation entropy = contextual blindness at Filigran
- [[Interview 014 — Ulrich Bauermeister (Filigran, Germany)]] — failed self-build partly due to knowledge fragmentation
- [[Patterns From Fieldwork]] — Pattern 40 (documentation entropy)
