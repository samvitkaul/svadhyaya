---
type: exploration
status: evolving
source: reconstructed from discussion dated 2026-09-17
---
# The surprise: polynomial multiplication is convolution

## Initial realization

Multiplying polynomials already implements a discrete convolution:

$$\left(\sum_i a_ix^i\right)\left(\sum_j b_jx^j\right)=\sum_k\left(\sum_{i+j=k}a_i b_j\right)x^k.$$

Why, then, do we traditionally teach frequency-domain analysis separately from rings and algebras?

## Follow the abstraction

The polynomial ring $F[x]$ contains finite coefficient sequences, with multiplication corresponding to linear convolution. The quotient $F[x]/(x^n-1)$ implements **cyclic convolution** on length-$n$ sequences (subject to the coefficient field/ring).

For a finite group $G$, the group algebra $F[G]$ replaces powers of $x$ by formal basis symbols $e_g$ satisfying $e_g e_h=e_{gh}$. Coefficients multiply via **group convolution**:

$$(a*b)(k)=\sum_{gh=k}a(g)b(h).$$

If $G$ is finite abelian and the coefficient field has suitable roots of unity and characteristic not dividing $|G|$, characters diagonalize convolution. A Fourier transform maps convolution to pointwise multiplication.

## The caveat that matters

For nonabelian groups, irreducible representations need not be one-dimensional: Fourier transform turns convolution into **blocks of matrices**, not scalar diagonal entries. In characteristic dividing $|G|$, semisimplicity can fail. Infinite formal power series also require care: multiplication is algebraically well-defined coefficientwise, but analytic Fourier convergence is a separate issue.

## The new questions

- How much signal processing is representation theory of groups?
- How do NTTs arise from finite fields and rings with suitable roots of unity?
- Where do topology, norms and convergence enter when moving to infinite sequences?

## Connections

- **Earlier exploration:** [Convolution and polynomials](convolution-and-polynomials.md).
- **Symmetry linearized:** [Representations](../concepts/representations.md).
- **Algebraic roots:** [Field extensions](../concepts/field-extensions.md).
- **Map:** [Cross-disciplinary connections](../maps/connections.md).
