---
type: concept
status: seed
---
# Group extensions

An extension of $Q$ by $N$ is a short exact sequence of groups

$$1\to N\to G\to Q\to 1.$$

The quotient and normal subgroup alone do **not** always determine $G$. When a group-homomorphic section $s:Q\to G$ exists, the extension **splits**, giving

$$G\cong N\rtimes_\varphi Q,\quad \varphi:Q\to\operatorname{Aut}(N).$$

In general, an extension may be nonsplit, so enumerating actions $Q\to\operatorname{Aut}(N)$ is not enough to classify every extension.

## Examples

- $S_3\cong C_3\rtimes C_2$, with the nontrivial $C_2$ action inverting elements of $C_3$.
- $C_6\cong C_3\times C_2$, where the action is trivial.
- $C_4$ is a nonsplit extension $1\to C_2\to C_4\to C_2\to1$.

## Connections

- [Exact sequences](exact-sequences.md) — the common structural language.
- [Classifying groups of order eight](../explorations/groups-of-order-eight.md) — a practical example where nonsplit cases matter.
