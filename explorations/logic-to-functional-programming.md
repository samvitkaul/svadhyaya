---
type: exploration
status: evolving
source: reconstructed from discussions dated 2026-11-01 and 2026-11-14
---
# From inference-rule fractions to functors, applicatives and monads

## Two questions, one structural instinct

A proof rule is sometimes drawn as a fraction: premises over a line, conclusion beneath it. Later came a question about understanding Haskell's **Functor → Applicative → Monad** hierarchy from algebraic first principles, with concrete examples in powersets and abelian groups.

The common question is: how do we capture valid *compositions* independent of their representation as syntax?

## Functor

A functor preserves identities and composition. The powerset construction can be viewed as a **covariant functor** $\mathcal P:\mathbf{Set}\to\mathbf{Set}$ using the direct-image map on functions. It maps $f:X\to Y$ to $\mathcal P(f):\mathcal P(X)\to\mathcal P(Y)$ with $A\mapsto f[A]$.

In Haskell, `Functor` is the computational manifestation of mapping a function across a context.

## Applicative and Monad

An applicative functor adds a coherent way to combine independent contextual computations. A monad provides a way to sequence contextual computations when the second can depend on the output of the first (`bind`).

For the powerset functor, a monad multiplication $\mu_X:\mathcal P(\mathcal P(X))\to\mathcal P(X)$ is **union** and the unit is **singleton inclusion**. The monad laws express associativity and neutrality of flattening nested sets.

For abelian groups, the *free abelian group functor* $F:\mathbf{Set}\to\mathbf{Ab}$ is left adjoint to the forgetful functor $U:\mathbf{Ab}\to\mathbf{Set}$. Their composite $UF$ is a monad on `Set`; it sends a set to finite formal integer linear combinations of its elements. This is different from saying that every endofunctor on `Ab` is a monad.

## Where adjoints enter

Every adjunction $F\dashv U$ induces a monad $UF$ on the source category of $F$. Conversely, monads can be represented through adjunctions (e.g., their Eilenberg–Moore construction). This puts programming abstractions in a broader algebraic framework.

## Open ends

How do free constructions lead to the monad laws? What changes with effects, laws and evaluation strategy in actual Haskell? How does the Bird–Meertens algebra of programming relate to equational reasoning and fusion?

## Connections

- **Abelian-group foundation:** [Modules](../concepts/modules.md).
- **Broader themes:** [Cross-disciplinary connections](../maps/connections.md).
