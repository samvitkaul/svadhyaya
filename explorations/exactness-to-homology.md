---
type: exploration
status: evolving
source: reconstructed from discussions dated 2026-08-28 to 2026-08-30
---
# Exactness: from linear algebra to homological algebra

## Motivating surprise

Kernels, images, quotients, and annihilators kept reappearing while studying linear operators and invariant subspaces. Why is an exact sequence so central instead of just a convenient diagram?

At $B$ in $A\xrightarrow{f}B\xrightarrow{g}C$, exactness means $\operatorname{im}f=\ker g$: *everything killed by the next map came from the previous one*.

## First intuition: a decomposition machine

For vector spaces, a short exact sequence

$$0\to A\to B\to C\to0$$

splits noncanonically, giving $B\cong A\oplus C$. It is tempting to treat exact sequences as a universal notation for direct sums.

**Correction.** Splitting is an additional property. For abelian groups or modules the sequence $0\to\mathbb Z\xrightarrow{2}\mathbb Z\to\mathbb Z/2\to0$ is exact but not split. For groups, even a **split** extension usually yields a semidirect product, not necessarily a direct product.

## Why duality was appealing

For a vector space $V$ and subspace $U$, the annihilator

$$U^\perp=\{\varphi\in V^*: \varphi(u)=0\ \forall u\in U\}$$

identifies $(V/U)^*$ with $U^\perp$ under the natural pullback. Dualizing short exact sequences of vector spaces remains exact, even in arbitrary algebraic dimension. Caution: this algebraic statement differs from dualizing sequences in other module categories or topological vector spaces without further assumptions.

## The conceptual leap

In a chain complex with $d_{n-1}d_n=0$, we know $\operatorname{im}d_{n+1}\subseteq\ker d_n$. The quotient

$$H_n=\ker d_n / \operatorname{im}d_{n+1}$$

**measures failure of exactness.** This reframes homology as a precise obstruction, not an unrelated new construction.

Extension classes similarly encode how an object can assemble from subobject and quotient without decomposing as a direct sum. In a suitable abelian category, $\operatorname{Ext}^1(C,A)$ classifies extensions of $C$ by $A$ up to the relevant equivalence.

## Connections

- **Prerequisite:** [Exact sequences](../concepts/exact-sequences.md).
- **Why not every sequence splits:** [From vector spaces to modules](from-vector-spaces-to-modules.md).
- **Nonabelian analogue:** [Group extensions](../concepts/group-extensions.md).
- **Concrete classification exercise:** [Groups of order eight](groups-of-order-eight.md).

## Open ends

How does the long exact sequence in homology arise from a short exact sequence of chain complexes? How do the algebraic dual and continuous dual differ?
