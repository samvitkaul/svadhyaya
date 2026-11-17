---
type: exploration
status: evolving
source: reconstructed from discussion history, 2026-08-28 through 2026-09-10
---
# From vector spaces to modules: what stops working?

## Initial intuition

A free abelian group looks suspiciously like a vector space: choose generators and write finite linear combinations, now with integer coefficients. So how much linear algebra—bases, operators, exact sequences, decompositions—survives if the scalars form a ring rather than a field?

This question arose after working with arbitrary-dimensional vector spaces, dual spaces, invariant subspaces, and exact sequences.

## The tempting but false extrapolation

> Every module should have a basis, perhaps by an argument resembling the axiom of choice used for vector spaces.

**Correction.** The axiom of choice does not repair the absence of inverses for nonzero scalars. The $\mathbb Z$-module $\mathbb Z/2\mathbb Z$ is not free: if it had a nonempty basis, multiplying a basis vector by $2$ would not give zero. Vector-space basis theorems depend on division by nonzero field elements, not just selection of generators.

Even a submodule of a free module need not be a direct summand. Consider

$$0\to\mathbb Z\xrightarrow{\times 2}\mathbb Z\to\mathbb Z/2\mathbb Z\to 0.$$

It is exact but not split: a homomorphism $\mathbb Z/2\mathbb Z\to\mathbb Z$ must be zero. Contrast the corresponding short exact sequence of vector spaces, which always splits (over a field).

## A fruitful reformulation: operators are modules

A linear operator $T:V\to V$ equips a vector space with an $F[x]$-module structure by setting $x\cdot v=T(v)$. This translates invariant subspaces to submodules and cyclic decompositions to module decompositions. Jordan blocks express *indecomposable pieces*: the extension information is not always captured by an eigenvalue list.

Thus module theory is not merely weakened linear algebra; it is a language for simultaneously studying vector spaces **with additional algebraic structure**.

## A second surprising example

On a smooth manifold $M$, vector fields form a module over $C^\infty(M)$, not in general a globally free module. Locally, vector fields have frames; globally, the tangent bundle may obstruct one. This connects the algebra of modules to geometry and topology.

## Consolidation

- Field scalars guarantee every vector space has a basis and every subspace a complement.
- Ring scalars permit torsion, relations among generators, nonfree projective modules, and nonsplit extensions.
- Splitting and projectivity are structure-sensitive properties, not merely set-theoretic selection problems.

## Connections

- **Formal statement:** [Modules](../concepts/modules.md).
- **Explains failure of splitting:** [Exact sequences](../concepts/exact-sequences.md).
- **Group analogue:** [Group extensions](../concepts/group-extensions.md).
- **Next question:** [From exactness to homology](exactness-to-homology.md).

## Open ends

How do projective modules generalize free modules? Which geometric vector bundles correspond to projective modules? What changes for infinite-dimensional operator theory?
