---
type: concept
status: seed
---
# Cayley graphs

Given a group $G$ and generating set $S$, a (directed) Cayley graph has vertices $g\in G$ and edges $g\to gs$ for each $s\in S$. If $S=S^{-1}$ and excludes the identity, we can forget edge direction to obtain an undirected simple graph (assuming duplicate edges are collapsed).

The construction makes algebraic generators visible as a regular, symmetric connectivity pattern.

## Example

For $C_n=\langle r\rangle$ and $S=\{r,r^{-1}\}$, the undirected Cayley graph is an $n$-cycle for $n\ge3$.

## Connections

- [Representations](representations.md) — both provide concrete realizations of abstract group structure.
- [Algebraic network topologies](../explorations/algebraic-network-topologies.md) — Cayley and coset graphs can specify repeated symmetric fabrics, subject to physical constraints.
