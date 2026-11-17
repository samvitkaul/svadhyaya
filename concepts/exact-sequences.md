---
type: concept
status: seed
---
# Exact sequences

For homomorphisms $A\xrightarrow{f}B\xrightarrow{g}C$, **exactness at $B$** means

$$\operatorname{im}f=\ker g.$$

A **short exact sequence** is

$$0\longrightarrow A\xrightarrow{i}B\xrightarrow{p}C\longrightarrow 0.$$

Thus $i$ is injective, $p$ surjective, and $C\cong B/i(A)$ in categories such as modules or groups (where the relevant normality is automatic from the kernel).

## Vector spaces versus modules

For vector spaces over a field, a short exact sequence always splits: choose a basis of $C$, lift it to $B$, and extend linearly to a section $s:C\to B$ with $p\circ s=1_C$. Then $B\cong A\oplus C$.

Over $\mathbb Z$, consider

$$0\to\mathbb Z\xrightarrow{\times 2}\mathbb Z\to\mathbb Z/2\mathbb Z\to 0.$$

This does **not** split as a sequence of abelian groups: a homomorphism $\mathbb Z/2\mathbb Z\to\mathbb Z$ must send its nonzero element to an element of order dividing $2$, hence to zero.

## Connections

- [Modules](modules.md) — exact sequences need not split over general rings.
- [Group extensions](group-extensions.md) — short exact sequences are the language of extensions, but a split group extension is generally a *semidirect*, not necessarily direct, product.

## Questions

How do derived functors and $\operatorname{Ext}$ detect the failure of a short exact sequence to split?
