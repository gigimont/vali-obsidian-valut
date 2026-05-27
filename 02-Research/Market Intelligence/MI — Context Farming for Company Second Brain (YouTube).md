# MI — Context Farming for Company Second Brain (YouTube)

#market-intelligence #second-brain #product-development #context-farming

> **Source:** YouTube video — "I Turned My Second Brain Into a Company Brain"
> **Speaker:** Brad (go-to-market engineer, AI systems builder)
> **Date captured:** May 2026
> **Type:** Video transcript — practitioner demonstration
> **Related source:** [[MI — Second Brain Execution Layer (YouTube)]] — companion video by same creator

---

## What This Is

A practitioner walkthrough of "context farming" — automated agents that pull context from business tools (Slack, Fireflies, Notion, etc.) into an Obsidian second brain on a scheduled basis, before the user logs in each morning.

**The core architecture:**
- **Business tools** (Slack, Fireflies, Notion, etc.) connected via MCP
- **Context farming agents** — scheduled Claude Code tasks that pull new information nightly
- **Obsidian vault** — unified knowledge layer where everything lands as linked markdown files
- **GitHub repo** — the sync layer; cloud farmers, Obsidian edits, and Claude Code all converge here
- **Query layer** — Claude reads the unified vault to brief you on any project, customer, or decision on demand

The result: a briefing on deals, decisions, and meetings you were never in — automatically, before you open Slack.

---

## Key Insights Relevant to Solco

### 1. "Things are just getting lost between the stakeholders" = the COO version of our problem

The speaker quotes a COO at a multi-tool company: "It's not a lack of tools, it's a lack of connected context." Context farming solves this by creating one unified knowledge layer that pulls from all sources.

- **Solco cross-reference:** This is the SME succession problem stated in operational language. Our ICP founders don't have Slack and Fireflies — their context lives in their heads, not in digital tools. The problem is the same (knowledge lost between stakeholders, across time) but the source is different. Context farming is the digital-native equivalent of what we do with the campfire method. The hard problem — and our moat — is that we extract from PEOPLE, not from APIs.

### 2. Context farming = the maintenance layer Solco is missing

After the initial extraction engagement, what keeps the knowledge base current? This video describes exactly that pattern: once the context layer is seeded, farming agents maintain and extend it automatically without human intervention. The system feeds itself.

- **Solco cross-reference:** Lorenz's "always-on monitoring" challenge ([[Interview 019 — Lorenz Essing (EMH Partners, Germany)]]). His objection was that a one-time extraction goes stale. Context farming is the technical answer: post-engagement, Solco could deploy lightweight farming agents on whatever digital signals the SME does have (email threads, simple meeting notes, WhatsApp exports) to keep the knowledge base alive. This is a product evolution path — extraction engagement (Year 1) → farming agents as SaaS retention (Year 2+).

### 3. "The system has started to feed itself" = flywheel that justifies SaaS pricing

"Your context gets deeper and your agents get smarter... this is what context engineering looks like in practice." Once a critical mass of context exists, the value of adding more context compounds — each new piece connects to more prior knowledge.

- **Solco cross-reference:** This is the retention mechanism we need. The first engagement creates the context layer (via extraction). Every subsequent update via farming agents increases the value of the knowledge base — making it harder to cancel. This justifies a SaaS model on top of the service engagement. Aligns with the MI — Mem insight on cost trajectory: build the service now, evolve to always-on SaaS as costs drop.

### 4. Proactive briefing without being in the meeting = our product's killer demo

The speaker walks into a $280K customer renewal meeting fully briefed — without reading a single Slack message or watching any recording. Claude surfaces the full account context on demand.

- **Solco cross-reference:** Direct analogue to our product demo scenario. The Filigran successor (or new Planungsleiter) asks: "How do we handle customer complaints about delivery schedules?" and gets the founder's 30-year judgment on demand — without ever having been in the room. This is the demo we need to build for Pfingsten. The briefing use case is more visceral and immediate than the succession use case — consider leading with it.

### 5. GitHub as the sync layer = what we already use

Everything converges through GitHub: cloud farming agents push from outside, Obsidian syncs local edits, Claude Code reads and writes — all through one repo. This is exactly our current vault architecture.

- **Solco cross-reference:** Our vault already runs on this pattern (vault ↔ GitHub ↔ Claude Code). We're not building from scratch — we're extending an architecture we already have operational. For the Filigran PoC, the GitHub repo is already the right foundation. The farming agents would be additive, not a rebuild.

### 6. MCP as the universal integration standard

"This works with any software that has an MCP." The pattern is: connect an MCP → run create farmer → schedule it → done. The same skill generates context farmers for any tool.

- **Solco cross-reference:** Product architecture implication. For SMEs that do have some digital touchpoints (email, basic CRM, simple project management), MCP-based farming agents could capture those signals automatically as part of the Solco maintenance layer. We don't need to build custom integrations — MCP is the open standard that handles it.

---

## What This Source Does NOT Solve

- **The headspace extraction problem:** Brad's system assumes context already exists in digital tools. Filigran's knowledge is not in Slack. Armin's is not in Fireflies. The founding generation's judgment has never been typed into any system. Context farming can maintain and extend a knowledge base once it's seeded — but it cannot create the seed. That's what Solco's extraction methodology does. The hard problem is still ours to own.
- **The SME user experience:** This system requires technical setup (GitHub, MCP, Claude Code). Our ICP (founders in their 50s-70s, non-technical successors) cannot and should not touch any of this. Our product must hide all of it.

---

## Product Implication: Two-Phase Solco Model

This video, combined with the execution layer video, suggests a clear two-phase product architecture:

| Phase | What | How | Revenue |
|-------|------|-----|---------|
| **1. Extraction** | Seed the context layer from human expertise | Three-pillar methodology (campfire + tracking + documents) | €15-25K service engagement |
| **2. Farming** | Maintain and extend the context layer from digital signals | Lightweight MCP-based farming agents running on schedule | €2-5K/month SaaS retention |

Phase 1 is our moat (nobody else can do the extraction). Phase 2 is the retention mechanism that turns a one-time engagement into recurring revenue.

---

## What We Can Learn

1. **Name the two phases explicitly** — "extraction engagement" (what we sell now) and "always-on farming" (what we sell next). Gives investors and clients a roadmap.
2. **Lead demos with the briefing use case** — "walk into a meeting fully briefed without being in any of the calls" is more visceral than "preserve institutional knowledge for succession." Both are true; the briefing lands faster.
3. **GitHub repo is already the right foundation** — our current vault architecture is not a prototype; it's the production pattern.
4. **MCP farming as the maintenance layer** — post-engagement, deploy MCP agents on whatever digital signals the SME has. No new infrastructure, just scheduled Claude tasks pulling from email/calendar/simple CRM.
5. **"Context compounds"** — use this framing with clients. The knowledge base gets more valuable over time, not less. It's not a one-time deliverable; it's a growing asset.

---

## Related
- [[Second Brain Landscape]] — overview of the AI knowledge management space
- [[MI — Second Brain Execution Layer (YouTube)]] — companion video: context layer + execution layer architecture
- [[MI — Mem (a16z Podcast)]] — proactive surfacing insight (same direction)
- [[MI — HAIC-MM (Ortolano & Gallegos, INCOSE 2026)]] — AI adoption maturity; farming agents = AI-Embedded maturity level
- [[Interview 019 — Lorenz Essing (EMH Partners, Germany)]] — "always-on monitoring" challenge; context farming is the technical answer
- [[Interview 020 — Francis de Vericourt (ESMT Professor)]] — transformation gap; extraction is the bridge from nothing to a seedable context layer
- [[Interview 022 — Marco Nortmeier (Filigran, Germany)]] — Obsidian-as-demo; GitHub vault architecture confirmed viable
- [[Patterns From Fieldwork]] — Pattern 28 (campfire method), Pattern 29 (tech must not feel like tech)
