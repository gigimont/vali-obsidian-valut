# Layer 2 — Methodology Learning: Bautechnik

Accumulating observations on extraction methodology and tacit-knowledge patterns specific to this domain. Append entries with a date heading.

## 2026-05-27 — Session 1 ([[2026-05-27_Bautechnik_Meeting-Record]])

- **Atomisierung is the moat, confirmed by a failure.** Bauermeister got a local stack (Ollama + Llama 3 8B / Mistral) chatting fine but failed at persisting documents in a vector DB via Python (LlamaIndex, "Schritt 5"). The build that works ends exactly where SOLCO's value begins: turning heterogeneous docs into context-rich, retrievable *Wissensbausteine*. Brute-force file dump ≈ a searchable folder and is explicitly *not* the product.
- **Corpus shape (Bautechnik):** ~1,500 files / ~2 GB (≈half excludable *Bemessungsprogramme*). Types: external university *Versuchsberichte* (Durchstand/Ermüdung/Brand/Querkraft — text + drawings + photos), *Gutachten*, *Bemessungshilfen* (formulas + diagrams + number tables). Multimodal: a text-only model is insufficient; drawings/tables/photos need handling. Some single docs are 150 pages (*Tonkalenderbeitrag*) — won't chunk into a single table.
- **Documentation-first sequencing validated by the partner.** Marco preferred finishing the concrete ingest and learning from it over broad parallel rollout — independent operator endorsement of the lead-with-documentation-defer-AI principle.
- **Data protection is the binding constraint, not the tech.** Default-deny posture ("alles was nicht erlaubt ist, ist verboten"); transcription + Adobe auto-summary already banned; approval chain Jenny Frank → Scope and Focus (external DPO) → Geschäftsleitung runs 2–4 weeks; the AI guideline itself took ~9 months. Local/data-sovereign models are attractive precisely because they sidestep some of this.
- **Supportability constraint:** one model, not many — because one internal admin (Marco) must support it. Shapes any productization.
- **Method note:** the failed-self-build narrative is itself prime extraction material — capture "we tried X and hit the wall at Y" stories deliberately.
