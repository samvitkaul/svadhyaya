# Svādhyāya · स्वाध्याय

*A living, Git-native notebook for mathematical self-study and exploration.*

This repository is a **graph of ideas**, not a transcript archive or a textbook. It separates canonical concepts, meandering explorations, cross-disciplinary structural motifs, and open questions.

## Navigation

- [Algebra map](maps/algebra.md)
- [Connections map](maps/connections.md)
- [Open questions](questions/open-questions.md)
- [Surprises](surprises.md)
- [Agent maintenance instructions](AGENTS.md)

## Seed concepts

- [Exact sequences](concepts/exact-sequences.md)
- [Modules](concepts/modules.md)
- [Group extensions](concepts/group-extensions.md)
- [Representations](concepts/representations.md)
- [Cayley graphs](concepts/cayley-graphs.md)
- [Field extensions](concepts/field-extensions.md)

## Explorations

- [Classifying groups of order 8](explorations/groups-of-order-eight.md)
- [Convolution and polynomial multiplication](explorations/convolution-and-polynomials.md)
- [Algebraic network topologies](explorations/algebraic-network-topologies.md)
- [Quadratic norms and Pell equations](explorations/quadratic-norms.md)

## Editing conventions

Markdown is canonical, with `$...$` and `$$...$$` for mathematics. Use **relative Markdown links** so GitHub renders notes and Obsidian can load the directory as a vault. Add structured *Connections* sections, explaining the nature of each link (generalizes, special case, analogy, application, prerequisite). Prefer one concept per file; one exploration can involve many concepts.

**Evidence hygiene:** The initial notes are reconstructed summaries inspired by prior discussions, **not verbatim transcripts**. Don't invent conversation citations, proof attributions, or sources. New notes should distinguish proved claims, examples, intuitions, and open conjectures.

**Privacy:** Keep personal transcripts and confidential architecture details out of a public repository. The current GitHub repository was observed to be public at initialization time.

Automated ingestion and historical chat imports are not configured yet.
