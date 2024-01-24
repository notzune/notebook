a relation $R$ that is a partial order relation is reflexive, antisymmetric, and transitive. the notion of a partial order relation allows for the possibility that some elements may not be comparable to each other, unlike a [[Total order relation|total order relation]] where every pair of elements is comparable.

it satisfies:
- [[Reflexive relation|reflexivity]]: every element is related to itself. formally, $\forall a \in S, (a,a) \in R$. this means that each element is considered to be at least as large as itself.
- [[Antisymmetric relation|antisymmetry]]: if one element is related to another, and vice versa, then the two elements are the same. formally, $\forall\space a,b \in S,\space\text{ if } (a,b) \in R \wedge (b,a) \in R \implies a = b$.
- [[Transitive relation|transitivity]]: if an element $a$ is related to a second element $b$, and $b$ is related to a third element $c$ then $a$ is also related to $c$. formally, $\forall\space a,b,c \in S, \text{ if } (a,b) \in R \wedge (b,c) \in R \implies (a,c) \in R$.

the subset relation among sets ($\subseteq$) is a classic example of partial order relation.

- [[Reflexive relation|reflexivity]]: every set is a subset of itself. $\forall S,\space S\subseteq S$.
- [[Antisymmetric relation|antisymmetry]]: if a set $A$ is a subset of a set $B$ and $B$ is a subset of A, then $A$ and $B$ must be the same set. $(A\subseteq B\wedge B\subseteq A \implies A = B\space)$
- [[Transitive relation|transitivity]]: if set $A$ is a subset of set $B$, and $B$ is a subset of set $C$ then set $A$ must also be a subset of set $C$. $(A\subseteq B\wedge B\subseteq C\implies A\subseteq C\space)$.

in these cases, not all elements (sets in this example) are directly comparable. for instance, two distinct sets may not be subsets of each other therefore this relation is only considered "partial" and not a "total" order relation.