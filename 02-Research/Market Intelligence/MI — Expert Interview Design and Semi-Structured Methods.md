---
title: "MI — Expert Interview Design and Semi-Structured Methods"
tags: [market-intelligence, methodology, interview-design, qualitative-research, semi-structured-interviews]
created: 2026-05-20
---

## Sources

- **Maryayaqin (Mary Ayaqin, 2024)** — "Mastering the Art of Expert Interviews" — overview of expert interview methodology: principles, benefits, step-by-step design; product design / UX research perspective
- **MAXQDA (Alexis Chavez, 2026)** — "Semi-Structured Interviews (2026): The Comprehensive Guide" — comprehensive academic and applied reference on semi-structured interview design, from history through execution

---

## What This Is

Two practical methodology guides on how to design and conduct expert interviews and semi-structured interviews. While the academic KE literature ([[MI — Classical Knowledge Elicitation Methods]]) and qualitative sociology ([[MI — Elicitation Methods in Qualitative Research (Vanessa May)]]) cover the theoretical underpinnings, these sources provide the practitioner design layer: how do you write good questions, what makes an interview semi-structured rather than structured, what are the known failure modes, and how do you ensure comparability across multiple interviews while preserving the flexibility to follow unexpected insights?

Directly applicable to: the Filigran session design, Interview Guide updates, and the AI-led interview chatbot prompt engineering (Kempten study in [[MI — Silver Tsunami and AI Knowledge Capture]]).

---

## Key Insights Relevant to Solco

### 1. The interview guide is a roadmap, not a script

MAXQDA's central principle: semi-structured interviews are guided by a flexible set of questions (the interview guide) but leave room to probe, follow up, and adapt based on the respondent's answers. The interview guide:
- Ensures key topics are consistently covered across participants (comparability)
- Leaves freedom to explore what the participant considers important (depth and authentic insight)
- Acts as a "roadmap rather than a script"

The error pattern in over-structured interviews: you get consistent data but miss the unexpected insights that often contain the most value. The error pattern in under-structured interviews: you get depth for one participant but can't compare across participants, and you may miss critical topics.

**Solco angle:** Our Interview Guide should be semi-structured by design. The campfire session is intentionally conversational, but there are specific knowledge categories we need to cover in every session (decision-making, key relationships, historical crises, rules of thumb). The guide defines the floor; the conversation determines the ceiling.

### 2. Expert interview failure modes — and how to avoid them

Maryayaqin identifies the key limitations:
- **Subjectivity bias:** experts' opinions are shaped by their personal experiences; they may present their way as the only way
- **Limited generalisability:** a small number of experts may not represent all relevant stakeholders — in KE, this is the rationalisation trap
- **Expert availability:** high-value experts are busy; securing their time requires clear value exchange
- **Misinterpretation risk:** researchers must be skilled enough to interpret responses correctly in real time

Counter-strategies from both sources:
- Establish clear research objectives BEFORE writing questions
- Stakeholder analysis first — identify ALL relevant experts, not just the most visible ones
- Use probes and follow-up questions specifically to surface the "why" beneath the "what"
- Build rapport explicitly — semi-structured interviews work better when the expert feels respected and understood
- Document immediately — interpretation degrades rapidly after the interview

**Solco angle:** The campfire method already addresses most of these risks by design (storytelling = bypasses rationalisation; multiple sessions = builds rapport; co-founder present = cross-check interpretations). The specific counter-strategy we're missing: a post-session structured debrief protocol where we immediately document what was surprising, what contradicted our priors, and what questions we failed to ask. This prevents misinterpretation at the note-creation stage.

### 3. Semi-structured interview design principles

MAXQDA's practical design framework:
- **Open-ended questions first** — let the expert define the territory before narrowing
- **Probes are the real extraction tool** — "can you tell me more about that?", "what happened next?", "why did you decide that way?" — these are where tacit knowledge surfaces
- **Funnel structure** — start broad (what is your experience with X?) → narrow (what specifically do you do when Y happens?) → concrete (can you give me an example of when Z occurred?)
- **Pilot the guide** — run a test interview with a colleague to check question clarity and timing
- **Avoid yes/no questions** — they close the conversation
- **Order matters** — rapport-building questions first; challenging or sensitive questions after trust is established

For technical knowledge extraction specifically:
- Ask for a recent critical incident ("tell me about the last time something went wrong with X")
- Ask for "typical day/process" walkthrough — exposes steps the expert considers too obvious to mention
- Ask what they would teach a new hire in their first week — surfaces the tacit "essentials" that experts take for granted

**Solco angle:** Three prompts specifically validated for tacit knowledge extraction that we should add to the Interview Guide:
1. "Tell me about the last time something went seriously wrong with [domain]. What happened and how did you handle it?"
2. "Walk me through a typical [project/decision/client interaction]. What's happening at each step?"
3. "If you were training someone to replace you in week one, what would you tell them that isn't in any manual?"

### 4. Semi-structured interviews are the dominant format in knowledge management research

MAXQDA's survey of the literature: semi-structured interviews are "one of the most widely used qualitative data collection strategies in social science research" and are specifically suited to:
- Exploring complex phenomena (expert knowledge is complex)
- Capturing unique perspectives and stories (tacit knowledge is individual)
- Combining consistency across participants with space for exploration
- Programme evaluation and implementation analysis (which is what our methodology validation is)

This is not just anecdotal — it is the methodological consensus of qualitative research across education, psychology, sociology, anthropology, and business strategy. The Solco methodology isn't unusual; it's aligned with decades of validated practice.

### 5. Expert selection is as important as question design

Maryayaqin on stakeholder analysis for expert interviews: the quality of an expert interview is determined first by selecting the right expert. Criteria for expert selection:
- **Educational and professional background** relevant to the domain
- **Hands-on experience** (not just theoretical knowledge)
- **Publications or industry reputation** as a proxy for being at the frontier
- **Willingness to reflect** — not all experts can articulate their knowledge; some just do it

For Solco, the relevant selection criteria for a Planungsleiter or equivalent:
- 10+ years in role (experience threshold)
- Single point of contact for multiple junior staff (confirms bottleneck status)
- Operationally active (not already in transition out)
- Ideally: self-aware about what they know that others don't

**Solco angle:** Add an expert selection checklist to the Interview Guide — not just "who is the bottleneck" but "who has the profile to produce good tacit knowledge in a conversational format."

---

## What We Can Learn

1. **Add three explicit extraction prompts to the Interview Guide:** critical incident, process walkthrough, "week one" training list. These are the three questions validated for tacit knowledge surfaces.
2. **Post-session debrief protocol:** immediately after each session, record (a) what surprised us, (b) what contradicted our priors, (c) what we forgot to ask. Prevents interpretation decay.
3. **Expert selection checklist:** refine Interview Guide to include a pre-session expert selection filter — not just seniority and bottleneck status, but reflective capacity.
4. **The interview guide structure:** broad → narrow → concrete. Open with landscape questions; end with scenario-specific follow-ups. Sensitive succession topics last.

---

## Related

- [[MI — Classical Knowledge Elicitation Methods]] — KE engineering tradition; fixed probe; role game; layer sequencing
- [[MI — Elicitation Methods in Qualitative Research (Vanessa May)]] — photo/object elicitation; artefact as trust mechanism; campfire upgrade
- [[MI — Silver Tsunami and AI Knowledge Capture]] — Kempten empirical study on LLM-led semi-structured interviews; depth/summary quality findings
- [[Interview Guide]] — living document to update with prompts from this source
- [[Patterns From Fieldwork]] — Pattern 28 (campfire method); Pattern 34 (Standardgrundlage-first)
