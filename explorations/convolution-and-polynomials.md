---
type: exploration
status: seed
---
# Polynomial multiplication is convolution

Let $a(x)=\sum_i a_i x^i$ and $b(x)=\sum_j b_j x^j$. Multiplication gives

$$a(x)b(x)=\sum_k\left(\sum_{i+j=k}a_i b_j\right)x^k.$$

Thus the coefficient sequence of the product is the **discrete convolution** $c_k=\sum_i a_i b_{k-i}$.

## Why this matters

The same pattern appears in formal power series and group algebras. Fourier transforms diagonalize certain convolution operations, converting them into pointwise multiplication under suitable analytic or finite-group hypotheses.

For $\mathbb C[C_n]$, coefficients are indexed cyclically and multiplication is **circular** convolution. Its characters give the discrete Fourier transform.

## Connections

- [Representations](../concepts/representations.md) — characters of finite abelian groups provide the spectral basis.
- [Connections map](../maps/connections.md) — the same algebra appears in signal processing.
