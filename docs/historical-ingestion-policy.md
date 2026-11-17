# Historical conversation ingestion policy

The source for these notes is currently **accessible discussion history and summaries**, not a full export. Narratives are reconstructed; they are not transcripts. Dates describe the original discussion(s) where known. Do not quote a statement as verbatim without checking the original.

## Preserve the epistemic trail

1. **Question / intuition:** what prompted the exploration?
2. **Proposed approach:** what initially seemed plausible?
3. **False start:** preserve the claim as a dated hypothesis, not a fact.
4. **Correction:** give the counterexample or missing assumption precisely.
5. **Consolidation:** state the defensible mathematical result.
6. **Connections:** add explanatory, typed links to concept and exploration pages.
7. **Open ends:** what should be investigated next?

If a prior assistant claim was wrong, mark that explicitly. If there is insufficient history to reconstruct chronology, state uncertainty rather than invent dialogue.

## Privacy boundary

The repo is public. Do not import raw exports or private sources automatically. First ingest to a **separate local or private staging area**; strip identifiers, employment details, confidential network architecture, and nonpublic links. Only reviewed, general mathematical content goes to public Markdown files.

## Suggested source metadata

```yaml
---
type: exploration
status: evolving
source: reconstructed from discussion history, YYYY-MM-DD
source_verified: false
---
```

Use `source_verified: true` only after a source reference or transcript is directly checked and retained in an appropriate private provenance index.

## Quality checks

- Derive, test, or cite mathematical claims. Mark unverified assertions.
- Do not confuse a metaphor (e.g., hyperbola *suggests* hyperbolic rotations) with a theorem.
- Verify relative Markdown links against the checkout.
- Avoid blindly rewriting existing curated concept notes.
- Submit small coherent patches; preserve the correction trail.
