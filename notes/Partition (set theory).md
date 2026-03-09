in [[Set theory|set theory]], a partition of a [[Sets|set]] is a grouping of its elements into [[Empty set|non-empty]] [[Subset|subsets]] in such a way that every element is included in exactly one subset.

every equivalence relation on a set defines a partition of this set, and every partition defines an equivalence relation. a set equipped with an equivalence relation or a partition is sometimes called a [[Setoid|setoid]], typically in [[Type theory|type theory]] and [[Proof theory|proof theory]].

## Definition and notation

a partition of a set $X$ is a set of non-empty subsets of $X$ such that every element $x$ in $X$ is in exactly one of these subsets. (i.e. the subsets are non-empty mutually [[Disjoint sets|disjoint sets]]).

a [[Family of sets|family of sets]] $P$ is a partition of $X$ if and only if all of the following hold:

- the family $P$ does not contain the [[Empty set|empty set]] 
	- $\emptyset\notin P$.
- the [[Union|union]] of the sets in $P$ is equal to $X$ 
	- $\cup_{A\in P}A=X$
- the [[Intersection|intersection]] of any two distinct sets in $P$ is empty 
	- $(\forall A,B\in P)A\neq B\implies A\cap B=\emptyset$