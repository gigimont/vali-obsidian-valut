# Filigran — Methodology Summary

Living pilot-level synthesis. Curated periodically from the per-domain Layer-2 files. Not auto-generated.

## Pilot status (as of 2026-05-27)

- **Kickoff:** 2026-05-22 cross-domain launch ([[2026-05-22_Kickoff_Meeting-Record]]). Four domains scoped: Bautechnik, Produktionsplanung, Vertrieb, Geschäftsleitung. Bautechnik chosen as first build; Produktionsplanung named the biggest lever.
- **Bautechnik Session 1:** 2026-05-27 ([[2026-05-27_Bautechnik_Meeting-Record]]). Diagnosed Bauermeister's failed Dec-2025 self-build; SOLCO owns the ingest/model research; summary + strategy due Fri 2026-05-29.

## Cross-domain methodology learnings so far

1. **Atomisierung / Wissensbausteine is the core value and the proven hard step.** A motivated internal expert reached a working local LLM chat but failed at vector-DB ingest of real documents. The product lives in context-rich chunking + retrieval over mixed formats (text, drawings, tables, photos), not in file storage.
2. **Lead with documentation, defer AI.** Sells better to operators and reduces the data-protection surface; independently endorsed by Filigran's IT lead.
3. **Data protection is the binding adoption constraint in regulated Mittelstand.** Default-deny posture + a multi-step DPO approval chain (internal coordinator → external DPO → Geschäftsleitung, 2–4 weeks; the AI policy itself took ~9 months). Local / data-sovereign models (Mistral, Ollama-hosted) are attractive specifically because they reduce this friction.
4. **Obsidian-as-demo works.** The live vault was the most persuasive artifact in the kickoff.
5. **Supportability shapes design:** one model, supportable by one internal admin.

## Per-domain Layer-2 files

- [[Bautechnik/Layer-2-Methodology-Learning|Bautechnik Layer-2]] — has a 2026-05-27 entry.
- Produktionsplanung / Vertrieb / Einkauf / Geschäftsleitung — not yet started.
