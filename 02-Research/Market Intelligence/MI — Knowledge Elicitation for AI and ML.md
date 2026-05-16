---
title: "MI — Knowledge Elicitation for AI and ML"
tags: [market-intelligence, knowledge-elicitation, LLM, AI-methodology]
created: 2026-05-16
---

## Sources

- Persson & Svensson — *Expert Knowledge Elicitation for Machine Learning: Insights from a Survey and Industrial Case Study* (Jönköping University Master's Thesis, Aug 2023)
- van den Bent, Pernisch, Schlobach (VU Amsterdam) — *Investigating Knowledge Elicitation Automation with Large Language Models* (Transportation Research Record, 2025)
- Lance Eliot — *Using Knowledge Elicitation Techniques To Infuse Deep Expertise And Best Practices Into Generative AI* (Forbes, Nov 2025)

---

## What This Is

Three sources examining how to get expert knowledge into AI systems — from ML pipelines (Persson & Svensson) to LLM infusion (Forbes/Eliot) to LLM-assisted elicitation (van den Bent). Together they map the technical landscape Solcus is operating in: the problem of transforming tacit expert knowledge into a form AI can use.

---

## Key Insights Relevant to Solcus

### 1. "Secret sauce locked in experts' brains" = exact Solcus problem

Lance Eliot, Forbes (Nov 2025):

> *"The secret sauce of best practices in a domain is often locked away in the brains of those steeped in that domain. The question arises as to how to surface that hidden knowledge and make it tangible and visible so that you can get it into an LLM."*

He frames the challenge identically to Solcus: existing documents capture the commoditized knowledge. The competitive advantage lives in the head. The gap is surfacing it.

**Solcus angle:** This is the Forbes-level confirmation that our problem statement is real. Quote Eliot in pitch decks and investor one-pagers.

### 2. Human-to-human bootstrapping → human-to-AI verification

Eliot's recommended workflow:
1. First extract knowledge through human-to-human sessions (expert + analyst)
2. Codify the rules
3. Have the AI echo back the rules to the expert for verification and augmentation
4. AI often triggers the expert to think of additional rules they hadn't articulated

He explicitly warns: "The icing on the cake then happens when the domain expert does the follow-up work with the AI. The experts are usually pleased to see how their rules have been codified and echoed back to them."

**Solcus angle:** This is our Phase 1 workflow: campfire session (human-to-human) → structured extraction (codification) → validation with AI summary read-back to founder. The read-back step is underutilized in our current process — it's where the second layer of rules emerges.

### 3. Rationalisation trap: extracted rules may not be the real rules

Eliot raises a critical warning: when experts verbalize their reasoning, they may provide socially acceptable rationalizations rather than their actual decision-making process. If their real method involves gut feeling or guesswork, they may substitute a more respectable-sounding rule.

> *"The expert might make up fake rationalizations and tell you that's how they do their work. You are then going to falsely or mistakenly rely upon something that isn't the true state of the matter."*

**Solcus angle:** This is why historical validation matters. Don't just ask "how do you decide?" — ask "let's look at the last 20 decisions you made and I'll tell you what the data says." Cross-referencing verbalized rules against actual historical behavior surfaces the real rules. Our storyboard session should include this retrospective step.

### 4. Rules can be encoded as JSON/YAML for RAG injection

Eliot demonstrates encoding extracted rules as structured data:

```json
{ "name": "Earnings Momentum Rule",
  "if": ["Company has >= 3 consecutive quarters of earnings growth", "Growth rate is accelerating"],
  "then": "Consider as buy candidate",
  "unless": "Price-to-earnings ratio > 30" }
```

These can be fed directly into LLMs via RAG or system prompts.

**Solcus angle:** Our knowledge graph isn't just for human retrieval — it's training data for the AI layer. The output of Phase 1 (structured rules + decision trees) becomes the RAG corpus for Phase 2 (the farming agent). Rules as JSON bridges Phase 1 and Phase 2 technically.

### 5. LLMs can surface rules from data — if you know how to ask

Eliot collected trading data and prompted ChatGPT to find patterns and compare them to the expert's verbalized rules. The AI identified a new rule the trader hadn't articulated: "If a stock drops more than 8% below purchase price, sell automatically." The trader confirmed it after reflection.

**Solcus angle:** This is the Phase 2 agent behavior. After extraction, the farming agent can analyze behavioral data (emails, decisions, outcomes) and surface latent rules the founder never articulated. Phase 2 isn't just maintenance — it's continued discovery.

### 6. AI-led KE: faster but shallower (van den Bent et al. 2025)

VU Amsterdam study comparing human-led vs LLM-led knowledge elicitation for ontology building (transportation domain):
- AI-led interviews: ~10 minutes vs ~35 minutes for human-led
- Human engineers: produced richer, more complete ontologies
- AI-generated ontologies: 19–32% hallucination rate in relationships
- **Hybrid is best:** AI for interview execution (speed, consistency), human for ontology structuring (quality, validation)

**Solcus angle:** Don't fully automate Phase 1. AI-assisted interviews are viable for routine extraction but insufficient for the strategic and cognitive tacit layers. Use LLMs to transcribe, summarize, and pattern-match — not to lead the high-stakes founder sessions.

### 7. Informed Machine Learning: the formalization challenge (Persson & Svensson 2023)

Jönköping Master's thesis (43 articles, 97 elicitation paths): the core challenge of incorporating expert knowledge into ML is **formalization** — the more tacit the knowledge, the harder it is to represent formally.

Three formalization factors:
1. Is it in writing?
2. How structured is the writing?
3. How formal is the language (equations vs natural language)?

Expert intuition sits at the lowest formalization level — it must be converted through KE before it can be used in any ML pipeline.

**Solcus angle:** Our Phase 1 deliverable is formalization. We move founder knowledge up the formalization ladder: unstructured narrative → structured story → decision rules → JSON/graph representation. Each step up makes the knowledge more AI-usable and more transferable.

---

## What We Can Learn

1. **Forbes quote for pitch decks:** "The secret sauce of best practices is often locked away in the brains of those steeped in that domain" — Eliot, Forbes Nov 2025
2. **Add read-back step to Phase 1:** After codifying rules, read them back to the founder and ask "what's missing?" — this surfaces the second layer that interview alone won't catch
3. **Historical validation prevents rationalisation:** Cross-check verbalized rules against actual historical decisions. Where they diverge, the data wins
4. **Rules as JSON = technical bridge:** Phase 1 output should include machine-readable rule format, not just narrative summaries
5. **Don't automate Phase 1 founder sessions:** AI-assisted is fine; AI-led loses the quality. Reserve human facilitation for strategic and cognitive tacit extraction

---

## Related

- [[MI — Classical Knowledge Elicitation Methods]] — the academic methodology underlying this
- [[MI — Storytelling and Tacit Knowledge Capture]] — tacit knowledge externalization theory
- [[MI — Knowledge Graphs for Enterprise AI]] — technical architecture for structuring extracted knowledge
- [[MI — Context Farming for Company Second Brain (YouTube)]] — Phase 2 continuous extraction
- [[Patterns From Fieldwork]] — Pattern 28 (Campfire), Pattern 35 (trust thresholds)
