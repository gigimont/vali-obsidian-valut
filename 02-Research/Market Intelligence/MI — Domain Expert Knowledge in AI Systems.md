---
title: "MI — Domain Expert Knowledge in AI Systems"
tags: [market-intelligence, expert-knowledge, ai, machine-learning, vertical-ai, informed-ml]
created: 2026-05-20
---

## Sources

- **Lamarr Institute (Gabriella Moreira, 2021)** — "Informed Machine Learning — Learning from Data and Prior Knowledge" — framework for integrating prior knowledge into ML models
- **Sundberg & Holmström, Umeå University / SCDI (Journal of Strategic Information Systems, 2024)** — "Fusing Domain Knowledge with Machine Learning: A Public Sector Perspective" — three mechanisms for linking domain knowledge to ML in organisations; open-access empirical study
- **Hansen & Quinon (Synthese, 2023)** — "The Importance of Expert Knowledge in Big Data and Machine Learning" — philosophical and IS argument that expert knowledge remains essential despite the "end of theory" narrative
- **Kuusisto, Dutra, Elezaby, Mendonça, Shavlik & Burnside, University of Wisconsin (AMIA 2015)** — "Leveraging Expert Knowledge to Improve Machine-Learned Decision Support" — ABLe (Advice-Based Learning) framework; empirical test in clinical decision support
- **Virtasant (Humberto Moreira)** — "The New AI Workforce: How Domain Experts Are Training NexGen AI Models" — vertical AI practitioner perspective; 400% YoY growth; expert intelligence as competitive differentiation

---

## What This Is

Five sources from different disciplines all converging on one thesis: general AI without domain expert knowledge is insufficient for specific, high-stakes applications. The "end of theory" prediction — that big data would make human expertise obsolete — is empirically wrong. Expert knowledge is not just helpful but architecturally necessary for producing reliable, domain-specific AI. This directly underpins the Solco thesis: the reason companies need to extract expert knowledge is not just for succession planning but because that knowledge is the input that makes their AI future-ready.

---

## Key Insights Relevant to Solco

### 1. The "end of theory" myth debunked — expert knowledge is architecturally necessary

Hansen & Quinon (Synthese 2023): the popular belief that big data + ML can replace expert theory is empirically wrong. Algorithms can find correlations, but without domain expert knowledge to frame the problem, validate the output, and embed context:
- Models produce spurious correlations
- Feature selection is uninformed
- Output fidelity degrades on rare-but-critical edge cases
- Outputs cannot be trusted without interpretability grounded in expert knowledge

"The human contribution to scientific progress is deemed to be non-essential and replaceable" — this view is wrong, and they demonstrate it.

**Solco angle:** The same argument applies to business AI. General LLMs can answer general questions. But a company's specific decision-making patterns, relational history, and operational judgment are NOT in the training data. Without extraction, the company's AI is generic. With extraction, it's specific. This is the fundamental "why" behind the product.

### 2. Vertical AI growing 400% YoY as general AI hits a plateau

Virtasant: vertical AI solutions (domain-specific models built on expert intelligence) are growing at **400% year-over-year** as companies discover that general-purpose models "do an okay job about 80% of the time" but fail at the 20% of high-stakes, domain-specific decisions that matter most.

The evolution of AI training: basic RLHF (any human feedback) → expert RLHF (expert human feedback) → Expert Intelligence (EI). The "cognitive stack" is moving up. The same way self-driving cars need expert driving judgment, not just crowd-sourced data, domain AI needs expert practitioners, not just public data.

Intuit's $1.4B expert intelligence platform is the enterprise proof point. Google and Anthropic are partnering with Turing specifically for expert-trained specialised models.

**Solco angle:** The Solco knowledge base is an expert intelligence layer — the same thing Intuit built for $1.4B, applied to Mittelstand SMEs. We're not building "AI for SMEs" in a generic sense; we're building the expert context layer that makes their AI useful. This is the right frame for any technical investor conversation.

### 3. Informed ML: prior knowledge compensates for small datasets

Lamarr Institute: "Informed Machine Learning" integrates prior expert knowledge (analytical models, simulations, knowledge graphs, expert feedback) into ML processes. Key benefit: **compensates for small datasets**. You don't need 10 million labelled examples if you have a domain expert's prior knowledge encoded as a constraint or regularisation term.

For SMEs with limited digital history: the Planungsleiter's 30 years of decision-making experience IS the prior knowledge. Encoded correctly, it allows an AI model to perform at near-expert level even when training data is sparse. This is the technical architecture argument for why knowledge extraction matters before AI deployment.

**Solco angle:** When a company asks "why do we need to extract knowledge before deploying AI?" — this is the answer. Without the prior, the model is generalised. With the prior (extracted via Solco), the model is expert-calibrated. We're not competing with AI tools; we're the prerequisite for making AI tools actually work in their specific context.

### 4. Domain knowledge + machine knowledge fusion requires process — not just data

Sundberg & Holmström (JSIS 2024) studied two Swedish public sector ML implementations and identified three mechanisms:
- **Consolidation:** aligning domain expert understanding and ML expert understanding so they share a problem frame
- **Algorithmic mediation:** the ML model is iteratively refined by expert feedback until it produces results the domain expert trusts
- **Naturalisation:** the ML output becomes accepted as standard practice — experts stop second-guessing it and start relying on it

The paper makes a critical point: **AI initiatives fail to generate value not because the technology is wrong but because the processes of knowledge production are poorly understood.** Knowledge must be co-produced through conversation and iteration, not extracted in a one-off session.

**Solco angle:** The three-phase engagement model (campfire → structured extraction → validation) maps directly to consolidation → algorithmic mediation → naturalisation. This academic framing validates why a structured methodology and multiple sessions are required — not as a commercial convenience, but as a technical necessity.

### 5. Human-in-the-loop expert feedback improves model quality measurably

ABLe framework (Kuusisto et al., clinical decision support): incorporating expert clinical advice into ML models achieved a **statistically significant 24% improvement in specificity** without missing a single malignancy. The expert's prior knowledge compensates for incomplete training data, directly improving precision in a safety-critical domain.

The framework is iterative: machine generates initial model → expert reviews and provides advice → machine generates revised model → expert refines advice → repeat. Each cycle improves the model's alignment with expert judgment.

**Solco angle:** This is the validation that human expert knowledge genuinely improves AI output quality — not as a general claim, but as a measurable empirical result. The "expert intelligence" is not optional decoration; it's the mechanism that achieves the last 20% performance gap general models can't close.

---

## What We Can Learn

1. **Expert knowledge is not just succession-relevant — it's AI-prerequisite.** For companies deploying AI, Solco's extraction is the prerequisite step that makes their AI investments work. This expands the sales conversation from "succession planning" to "AI readiness."
2. **The vertical AI frame (Virtasant) reframes the Solco value proposition.** We're building the expert intelligence layer, not a documentation service. This is the $1.4B Intuit comparison.
3. **Knowledge co-production requires multiple sessions** (Sundberg & Holmström). The three mechanisms (consolidation → algorithmic mediation → naturalisation) map to our session sequence. This validates our multi-session model as technically necessary, not commercially inflated.
4. **Informed ML = the technical architecture of what Solco builds.** The extracted expert knowledge is the prior. The knowledge base is the informed ML input layer. This is the technical pitch for CTOs and AI-literate buyers.

---

## Related

- [[MI — Context Engineering Platforms (Atlan 2026)]] — context layers; AI failures = context failures; MCP; governance
- [[MI — Knowledge Graphs for Enterprise AI]] — GraphRAG; tribal context as the fourth context type; provenance trace
- [[MI — Knowledge Elicitation for AI and ML]] — practical KE for LLM infusion; rationalisation trap; AI hallucination rates
- [[MI — Company Brain Concept (Ability.ai, Falconer, YC)]] — enterprise convergence on same thesis; 4-property framework
- [[Patterns From Fieldwork]] — Pattern 22 (ERP ceiling); Pattern 32 (motivated insider blocked at build step)
