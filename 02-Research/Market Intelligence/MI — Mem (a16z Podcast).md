# MI — Mem (a16z Podcast)

#market-intelligence #second-brain #consumer-ai

> **Source:** a16z podcast — interview with Mem founders Kevin Moody and Dennis Zoo
> **Date of source:** ~2023 (pre-dates our project)
> **Date captured:** May 14, 2026
> **Type:** Podcast transcript analysis

---

## What Mem Is

Mem is a consumer AI company building a personal knowledge management tool — a "second brain" powered by LLMs. Their core thesis: information should not need to be manually organised. Instead, AI should match every piece of information to the context and situation in which it would be best used, eliminating the folder structure entirely.

They are consumer-focused (individual knowledge workers), subscription-based (free + premium), and positioning as a "personal EA" rather than a note-taking app.

---

## Key Insights Relevant to Solco

### 1. The 2.5-hour stat
Knowledge workers spend 2.5 hours per day (~30% of their workday) searching for information. This is from 2016 and likely worse now. On top of search time, there's "hidden reinvention" — people recreating work that already exists because they didn't know to look for it.
- **Solco cross-reference:** This validates the Planungsleiter bottleneck ([[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]]). The 130 planners don't just escalate to Bergerhoff — many of them waste time reinventing solutions he already found. Our product makes his knowledge findable without him being present.

### 2. "The folder is a skeuomorphic filing cabinet from the 1950s"
The organisational structure we rely on is 60+ years old. It was a metaphor for physical filing cabinets translated to computers. AI eliminates the need for this intermediate layer entirely.
- **Solco cross-reference:** This is why we should NOT build a traditional knowledge base with categories and folders. Our product should be a contextual retrieval system — ask a question in natural language, get the relevant knowledge. No browsing, no filing, no maintenance. Aligns with our "campfire method" (Pattern 28) — capture messy stories, let AI structure them.

### 3. "The missing ingredient was contextual understanding of human language"
Before LLMs, computers could store and retrieve but couldn't REASON about what they stored. LLMs marry reasoning capabilities with vast storage — the unlock for a true second brain.
- **Solco cross-reference:** This is why the timing is right (our "Why Now" slide). Five years ago, you could capture stories but couldn't turn them into queryable knowledge. Now you can. The three-pillar methodology (storytelling + tracking + document ingestion) produces raw data; the LLM is what transforms it into a usable second brain.

### 4. "Same search, different results for different people"
Personalisation is not just "access my data." It's "adapt to WHO I am and HOW I think." The AI should model the user and adjust its responses accordingly.
- **Solco cross-reference:** Direct product design implication. The queryable knowledge base should respond differently based on who's asking. The new hire gets step-by-step. The experienced planner gets exception cases. The successor gets strategic context. Same underlying data, role-adapted presentation.

### 5. Proactive intelligence > reactive search
The real value is not "I search and find." It's "the system surfaces what I need before I know to ask." Like a good EA who prepares your briefing before the meeting.
- **Solco cross-reference:** Aligns with Lorenz's "always-on monitoring" suggestion ([[Interview 019 — Lorenz Essing (EMH Partners, Germany)]]). The product shouldn't just answer questions — it should proactively flag: "Key employee X gave notice. Here are the 3 knowledge clusters at risk and what needs to be captured before they leave."

### 6. Cost trajectory makes this viable at scale
Compute costs dropping by orders of magnitude every few months. What's expensive now will be cheap soon.
- **Solco cross-reference:** Our €15-25K service engagement is viable now. The SaaS version (always-on monitoring at €2-5K/month) becomes economically viable as costs drop. The business model evolution is: high-touch service today → hybrid service+software → pure SaaS long-term.

### 7. "People spend more time organising their second brain than using it"
The irony of current knowledge management tools: the maintenance burden defeats the purpose. If our product requires SME employees to maintain it, it will fail.
- **Solco cross-reference:** Critical design principle. Our product must be ZERO MAINTENANCE for the customer after the initial extraction. The knowledge base should self-organise. No tagging, no filing, no curation by the user. If we build something that requires ongoing human maintenance, we've built another ERP — and we've lost our differentiation.

---

## How Mem Differs From Solco

| Dimension | Mem | Solco |
|-----------|-----|--------|
| Customer | Individual knowledge workers | SME organisations (whole company) |
| Data source | User's own digital notes, emails, files | Extracted from people's HEADS through interviews + observation + documents |
| The hard problem | Organising existing digital information | Extracting information that was NEVER digital |
| Business model | Consumer SaaS subscription | Service engagement (€15-25K) → SaaS retention |
| Moat | AI personalisation + user habit | Trust + extraction methodology + SME domain expertise |

**The key distinction:** Mem assumes the data already exists in digital form and needs to be organised. Solco starts further upstream — the data doesn't exist yet. We CREATE the digital knowledge layer from human expertise that was never written down. Mem is "organise what you have." Solco is "capture what you don't have yet, then make it usable."

---

## What We Can Learn From Mem

1. **Zero-organisation principle:** Don't make users file things. Let AI handle structure.
2. **Role-adaptive responses:** Same knowledge, different presentation based on who's asking.
3. **Proactive surfacing:** Don't wait for questions. Alert when knowledge is relevant.
4. **The "personal EA" framing:** Resonates more than "knowledge base" or "documentation tool."
5. **Cost trajectory awareness:** Build the service model now, plan for the SaaS model as costs drop.

---

## Related
- [[Second Brain Landscape]] — overview of the space
- [[Interview 016 — Stefan Bergerhoff (BWB-Gruppe, Germany)]] — Planungsleiter bottleneck validates the "hidden reinvention" problem
- [[Interview 019 — Lorenz Essing (EMH Partners, Germany)]] — "always-on monitoring" aligns with proactive intelligence
- [[Interview 020 — Francis de Vericourt (ESMT Professor)]] — Francis's "something missing in the middle" = the transformation methodology that turns raw capture into queryable knowledge
- [[Competitors]] — Mem as an adjacent (not direct) competitor
- [[Patterns From Fieldwork]] — Pattern 28 (campfire method), Pattern 29 (tech must not feel like tech)
