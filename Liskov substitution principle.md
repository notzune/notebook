the Liskov substitution principle (LSP) is a particular definition of [[Subtyping|subtyping]] relation, called [[Behavioral subtyping|strong behavioral subtyping]]. it is based on the concept of "substitutability" which is a concept in [[Object-Oriented Programming|OOP]] stating that an [[Object (computer science)|object]] (such as a [[Class (computer programming)|class]]) may be replaced by a sub-object (such as a class that extends the first class) without breaking the program. it is a [[Semantics (programming languages)|semantic]] rather than a syntactic relation, because it intends to guarantee semantic interoperability of [[Data type|types]] in a hierarchy, object types in particular.

let $\phi(x)$ be a property provable about objects $x$ of type $T$, then $\phi(y)$ should be true for objects $y$ of type $S$ where $S$ is a subtype of $T$.

$$
S\leq T\rightarrow(\forall x:T.\phi(x)\rightarrow\forall y:S.\phi(y))
$$

that is, if $S$ subtypes $T$, what holds for $T$-objects holds for $S$-objects.