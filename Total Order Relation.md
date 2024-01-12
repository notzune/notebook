a total order relation, also known as a linear order relation, extends the concept of a [[Partial Order Relation|partial order relation]] by also including the additional requirement that every pair of elements must be comparable.

a total order relation is a type of [[Binary relation|binary relation]].

a relation $R$ on a set $S$ is a total order relation if it satisfies all the properties of a [[Partial Order Relation|partial order relation]]—reflexivity, antisymmetry, transitivity—plus an additional property, [[Comparability (Totality)|comparability (totality)]].

a total order relation satisfies:
- [[Reflexive Relation|reflexivity]]: every element is related to itself. formally, $\forall a \in S, (a,a) \in R$. this means that each element is considered to be at least as large as itself.
- [[Antisymmetric Relation|antisymmetry]]: if one element is related to another, and vice versa, then the two elements are the same. formally, $\forall\space a,b \in S,\space\text{ if } (a,b) \in R \wedge (b,a) \in R \implies a = b$.
- [[Transitive Relation|transitivity]]: if an element $a$ is related to a second element $b$, and $b$ is related to a third element $c$ then $a$ is also related to $c$. formally, $\forall\space a,b,c \in S, \text{ if } (a,b) \in R \wedge (b,c) \in R \implies (a,c) \in R$.
- [[Comparability (Totality)|comparability]]: for all elements $a$ and $b$ in a set $S$, either $(a,b) \in R$ or $(b,a) \in R$ (or both, if $a=b$). formally, $\forall\space a, b \in S, (a,b) \in R \vee (b,a) \in R \vee (a,b) \wedge (b,a) \in R \leftarrow (a = b)$

## The Usual Order of Numbers

an example of a total order relation is the usual ordering of real numbers, denoted by $\leq$.

- [[Reflexive Relation|reflexivity]]: for any real number $a$, $a\leq a$. more formally, $\forall a \in\mathbb{R}, a\leq a$.
- [[Antisymmetric Relation|antisymmetry]]: if $a\leq b \wedge b\leq a, \implies a=b$.
- [[Transitive Relation|transitivity]]: if $a\leq b \wedge b\leq c, \implies a\leq c$.
- [[Comparability (Totality)|comparability]]: for any two real numbers $a$ and $b$, either $a\leq b\vee b\leq a$ is true.

in a total order, there are no two distinct elements where one is not related to the other in some way. this makes them useful for sorting algorithms, [[Number Theory|number theory]], and whenever a strict linear hierarchy is required.