---
title: "MI — Computer-Use AI Agents (Clicky, Google DeepMind)"
tags: [market-intelligence, AI-agents, computer-use, interface]
created: 2026-05-16
---

## Sources

- YouTube demo — *Clicky (YC startup)* — screen-resident AI agent that controls the computer in the background (clickie.so)
- Google DeepMind — *Reimagining the Mouse Pointer with AI* — research prototype of AI-enhanced pointer with Gemini, understanding fluid user intent across apps

---

## What This Is

Two sources on AI that operates at the OS/interface layer rather than inside a specific app. Clicky is a YC-backed product (free at time of recording) that acts as a screen-resident agent: it sees your screen, takes instructions by voice, and executes multi-step tasks in background. Google DeepMind's prototype embeds Gemini directly into the mouse pointer, enabling cross-app, cross-window contextual understanding. Together they signal a new computing paradigm: AI as the ambient orchestration layer, not a tab you switch to.

---

## Key Insights Relevant to Solco

### 1. Director-vs-doer framing = successor's role with Solco

Clicky explicitly reframes the human role: "You can bring it priorities, goals, what's important. And Clickie becomes a smart buddy that goes and does the work for you. Your role is the director."

The video's concrete use cases — competitive research PDF, file organization + expense dashboard, video editing, Amazon cart — all follow the same pattern: one natural-language instruction → multi-step background execution → result delivered without user managing the process.

**Solco angle:** This is how a successor should interact with the Solco knowledge base in Phase 2. "How would we handle a situation like this?" → agent queries the graph, surfaces the founder's historical pattern, generates a recommendation. The successor never needs to know what's in the system or how it's structured.

### 2. Background parallel execution is the Phase 2 architecture

Clicky runs multiple agents simultaneously in the background: "I normally just have multiple running at a time." User keeps working while agents execute independently, pinging when done.

**Solco angle:** This is exactly the context farming architecture from Phase 2. Multiple agents pulling from Slack, summarizing Fireflies transcripts, tagging email decisions — all running on schedule without successor involvement. Clicky proves this UX pattern works and is ready for non-technical users.

### 3. Computer-use = the farming pipeline we need to build

Clicky's architecture: sees screen → understands context → executes across apps (Descript, Google Sheets, Drive, Amazon, browser). It can open files, scrape data from images (receipts → expense dashboard), push to Google Sheets, all via a single voice command.

**Solco angle:** Our Phase 2 farming agent needs to do exactly this across the apps a German/Italian SME uses: pull Outlook emails, summarize Teams calls, flag decisions in shared drives, push to the knowledge graph. Clicky demonstrates the technical pattern is mature enough to use as a building block. OpenClickie (open-source fork, runs local models) is particularly interesting for privacy-sensitive deployments.

### 4. YC funding = the market believes in this paradigm

Clicky is a YC-backed startup, launched free to build user base. YC placed a bet on the computer-use agent category in the same cohort that named the "company brain" as a missing AI primitive (see [[MI — Company Brain Concept (Ability.ai, Falconer, YC)]]). The category is funded and moving fast.

**Solco angle:** Investor conversations can cite both: YC named the company brain as a missing primitive AND is funding the agent infrastructure (Clicky) to populate it. The stack is assembling.

### 5. Barrier to entry disappearing for non-technical users

"The hardest part has always been the barrier to entry. But the moment I show people Clickie, their lives get instantly easier because for the first time, that learning barrier actually disappears."

**Solco angle:** This is the same shift we count on for Phase 2. The German Mittelstand successor doesn't need to understand how the knowledge graph works — they just ask a question and get an answer. The UI layer (voice, natural language) absorbs all the technical complexity.

### 6. Fluid intent across apps = the knowledge graph problem (Google DeepMind)

DeepMind's research focuses on "fluid user intent" — an AI pointer that understands not just what you're pointing at but *why it matters* and *what you want to do with it*. "All of these windows are going to be communicating with the pointer." Voice + visual understanding + pointing = coherent intent interpretation across the whole screen.

**Solco angle:** This points at the same problem knowledge graphs solve: understanding the *why* behind actions, not just logging *what* happened. An action log without intent is just a diary. A knowledge graph with semantic relationships captures the reasoning — which is what the successor actually needs.

---

## What We Can Learn

1. **Director framing for successor pitch:** "Your role is the director. The AI does the work." Use this language in sales conversations — it reframes the Solco product from "database" to "autonomous assistant"
2. **OpenClickie as building block:** Open-source computer-use agent that can run local models — worth evaluating for privacy-compliant Phase 2 farming agents in European deployments
3. **Parallel execution UX:** Multiple background agents = the right mental model for Phase 2; the user experience is "set and forget," not "manage and supervise"
4. **YC signal to use with investors:** YC funded both the company brain concept and the agent infrastructure in the same cycle — the stack is assembling and capital is moving here

---

## Related

- [[MI — Context Farming for Company Second Brain (YouTube)]] — Phase 2 context farming architecture this enables
- [[MI — Company Brain Concept (Ability.ai, Falconer, YC)]] — YC's "missing primitive" framing; same funding cohort signal
- [[MI — Knowledge Graphs for Enterprise AI]] — the technical substrate agents operate against
- [[MI — Contextual Blindness and Knowledge Graphs (LinkedIn)]] — why agents need structured context, not flat documents
