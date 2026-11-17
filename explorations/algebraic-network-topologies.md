---
type: exploration
status: seed
---
# Specifying network topologies algebraically

A graph can be generated from a compact algebraic specification rather than enumerating every edge.

## Candidate lenses

1. **Cayley graphs:** Use a group and generators to specify a homogeneous, vertex-transitive topology.
2. **Coset graphs:** Use group actions on cosets to obtain less-than-regular representations of symmetry.
3. **Voltage graphs:** Build a large covering graph from a smaller base graph labeled with group elements.
4. **Compositional specifications:** Describe repeated local fabrics, package-level transformations, and exceptional edges separately.

## Caution

Real interconnects may have asymmetric port roles, nonuniform links, topology changes from harvested dies, routing constraints, and physical timing requirements. Algebraic elegance does not replace verification. A useful prototype should produce edge lists and routing invariants comparable to an existing testbench.

## Connections

- [Cayley graphs](../concepts/cayley-graphs.md) — symmetric base construction.
- [Representations](../concepts/representations.md) — ways to realize and analyze symmetries.

## Open questions

What is the smallest expressive domain-specific language that captures hierarchy, symmetry breaking, and exceptional wiring while still permitting automatic consistency checks?
