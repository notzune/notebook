in math, a probability measure is a [[Real numbers|real-valued]] [[Function|function]] defined on a set of [[Events|events]] in a [[σ-algebra]] that satisfies [[measure]] properties such as countable additivity. the difference between a probability measure and the more general idea of a measure is that a probability measure must assign value 1 to the entire σ-algebra (since all [[Probability|probability values]] must add to 1).

formally, the requirements for a [[Set function|set function]] $\mu$ to be a probability measure on a σ-algebra are that:

- $\mu$ must return results in the unit interval $[0,1]$, returning $0$ for an [[Empty set|empty set]] and $1$ for the entire space.
- $\mu$ must satisfy the countable additivity property that for all countable collections $E_1,E_2,\dots$ of pairwise [[Disjoint sets|disjoint sets]]:$$\mu\left(\bigcup_{i\in\mathbb{N}}E_i\right)=\sum_{i\in\mathbb{N}}\mu(E_i)$$
