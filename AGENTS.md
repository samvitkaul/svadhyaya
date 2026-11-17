# Instructions for coding and writing agents

Purpose: Maintain Svādhyāya as a mathematically accurate, interconnected, Git-native knowledge base.

## Invariants

1. Never ingest a chat transcript or private work material into a public repository without explicit approval.
2. Markdown and LaTeX are canonical. Preserve working relative links.
3. A concept note describes a coherent mathematical object or theorem; an exploration describes a question-driven path.
4. Do not overwrite the author's perspective or questions with a generic textbook exposition.
5. Clearly label **Theorem / Proof / Example / Intuition / Open question** where appropriate.
6. Verify all claimed results. If not verified, mark *to verify* rather than invent a proof.
7. Record conceptual relationships in prose; link with descriptive phrases, not bare 'see also'.
8. Avoid duplication: prefer updating a canonical note and linking back to it.
9. Never fabricate citations to conversations. Only add source URLs when provided and verified.
10. Propose logical edits in small commits or a pull request with a concise summary.

## Ingestion workflow

- Identify source and date where known. Separate user-authored insights from assistant explanations.
- Extract definitions, theorems, proofs, counterexamples, motivating problems and open questions.
- Search the repository for existing concepts before creating files.
- Add a minimal but explicit set of bidirectional links where they provide context.
- Do a proof-check and link-check pass; surface ambiguities to the author.
- When a new note challenges an old one, preserve the correction trail in Git history.

## Suggested metadata (optional)

```yaml
---
type: concept # concept | exploration | map
status: evolving # seed | evolving | reviewed
---
```
