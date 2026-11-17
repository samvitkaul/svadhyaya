---
type: exploration
status: evolving
source: reconstructed from discussion dated 2026-10-19
---
# Regular representation versus the smallest faithful representation

## Starting point

Associate one basis vector $e_g$ of a vector space to every element of a finite group $G$. Left multiplication gives the **regular representation** on a space of dimension $|G|$. But a cyclic group has one generator and can act through roots of unity. Why should we ever need $|G|$ dimensions?

## The important distinction

A representation $\rho:G\to\operatorname{GL}(V)$ need not be injective. A **faithful** representation has trivial kernel. Its *minimum dimension* over a specified field can be much smaller than $|G|$.

For a cyclic group $C_n$, over $\mathbb C$, a primitive $n$-th root $\zeta_n$ defines a one-dimensional faithful representation $\rho(k)=\zeta_n^k$. The regular representation, on the other hand, contains **all** irreducible characters (each once for an abelian group) and is universal for certain algebraic constructions.

## Another false inference to avoid

A single abstract generator does **not** always imply a one-dimensional faithful representation over every field. Over $\mathbb R$, a faithful representation of $C_n$ for $n>2$ requires at least dimension two (e.g., a rotation representation), because the only finite-order elements of $\mathbb R^\times$ are $\pm1$.

Likewise, asking for a minimal faithful representation is distinct from asking for a *complete decomposition* of the regular representation into irreducibles.

## Why it matters

Symmetry-based system simplification often needs precisely those representation components that act on the particular state space of interest. In Fourier methods on finite abelian groups, all irreducible representations are one-dimensional; in nonabelian settings matrix blocks remain.

## Connections

- **Definition:** [Representations](../concepts/representations.md).
- **Fourier application:** [Fourier from ring multiplication](fourier-from-ring-multiplication.md).
- **Network symmetry:** [Algebraic network topologies](algebraic-network-topologies.md).
