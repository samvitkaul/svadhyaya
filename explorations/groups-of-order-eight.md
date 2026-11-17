---
type: exploration
status: seed
---
# Why are there exactly five groups of order eight?

The familiar conclusion is that, up to isomorphism, the groups of order $8$ are

$$C_8,\quad C_4\times C_2,\quad C_2^3,\quad D_8,\quad Q_8,$$

where $D_8$ denotes the dihedral group of order $8$ (symmetries of the square).

## Outline of a proof

Every group of order $p^n$ has nontrivial center. If $G$ is abelian, the classification of finite abelian groups yields precisely the three abelian cases above.

Suppose $G$ is nonabelian of order $8$. The center is nontrivial and cannot have order $4$ (since $G/Z(G)$ would be cyclic, forcing $G$ abelian). Therefore $|Z(G)|=2$, and $G/Z(G)\cong C_2\times C_2$. In particular, $G$ must contain an element of order $4$ (otherwise exponent two forces commutativity). Let $a$ have order four. Its subgroup $\langle a\rangle$ is normal of index two. Take $b\notin\langle a\rangle$; conjugation by $b$ must send $a$ to $a^{-1}$, since trivial conjugation would make $G$ abelian. Also $b^2\in\langle a\rangle$ is fixed by inversion, so $b^2=1$ or $a^2$. Those cases yield $D_8$ and $Q_8$, respectively.

## Structural lesson

An action $C_2\to\operatorname{Aut}(C_4)$ alone does not determine the extension. The relation $b^2=1$ versus $b^2=a^2$ distinguishes two nonabelian groups with the same inversion action.

## Connections

- [Group extensions](../concepts/group-extensions.md) — a concrete demonstration of split and nonsplit extensions.
- [Exact sequences](../concepts/exact-sequences.md) — the normal subgroup and quotient organize the classification.
