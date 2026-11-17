---
type: concept
status: seed
---
# Group representations

A representation of a group $G$ on a vector space $V$ over $K$ is a homomorphism

$$\rho:G\to\operatorname{GL}(V).$$

It need **not** be injective. An injective representation is called **faithful**.

The left regular representation acts on a vector space with basis $\{e_g:g\in G\}$ by $h\cdot e_g=e_{hg}$. It is faithful and has dimension $|G|$, but is often not minimal.

## Example: cyclic groups

Over $\mathbb C$, $C_n$ admits a faithful one-dimensional representation $k\mapsto e^{2\pi i k/n}$.

## Connections

- [Modules](modules.md) — a representation corresponds to a module over $K[G]$.
- [Cayley graphs](cayley-graphs.md) — both arise from group actions, but express different structures.
- [Convolution](../explorations/convolution-and-polynomials.md) — multiplication in group algebras generalizes coefficient convolution.
