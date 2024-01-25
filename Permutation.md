in mathematics, a permutation of a [[Sets|set]] is an arrangement of its [[Element|members]] into a [[Sequence|sequence]] or a [[Total order|linear order]], or if the set is already ordered, a rearrangement of its elements.

the study of permutations of [[Finite set|finite sets]] is an important topic in [[Combinatorics|combinatorics]] and [[Group theory|group theory]].

in [[Computer science|computer science]], they are used for analyzing [[Sorting algorithms|sorting algorithms]].

the number of permutations of $n$ distinct objects is $n$ [[Factorial|factorial]], usually written as $n!$, which means the product of all positive [[Integer|integers]] less than or equal to $n$.

formally, a permutation of a set $S$ is defined as a [[Bijection|bijection]] from $S$ to itself.

that is, it is a [[Function|function]] from $S$ to $S$ for which every element occurs exactly once as an [[Image|image]] value.

such a function $f:S\rightarrow S$ is equivalent to the rearrangement of the elements of $S$ in which each element $i$ is replaced by the corresponding $f(i)$. 

for example, the permutation (3,1,2) is described by the function $\sigma$ defined as 

$$
f(1)=3,\space f(2)=1,\space f(3)=2
$$

the collection of all permutations of a set form a [[Group|group]] called the [[Symmetric group|symmetric group]] of the set.

the group operation is the [[Function composition|composition]] of functions (performing one rearrangement after the other), which results in another function (rearrangement).

## In probability and combinatorics

in [[Probability theory|probability theory]], more specifically in [[Combinatorics|combinatorics]], permutations are used to calculate how many ways a series of distinct $k$ objects can be drawn from a pool of $n$ objects.

if the drawings are performed [[Replacement|with replacement]] then the $k$ drawings are all identical [[Events|events]], each with $n$ possible [[Outcome|outcomes]] and the [[Multiplication rule of combinatorics|multiplication rule]] shows that there are $n^k$ possible ways to draw $n$ objects, but if they are made *without replacement*, then the outcome is said to be a permutation of $k$ objects from the original $n$. 

a permutation is then denoted as $P^n_k$ and is formally defined as an ordered sequence of $k$ objects selected without replacement from the group of $n$ objects.

the number of possible permutations of $k$ objects from $n$ objects is

$$
P^n_k=n\times(n-1)\times(n-2)\times\dots\times(n-k+1)=\frac{n!}{(n-k)!}
$$

if $k=n$ then the number of permutations is simply

$$
P^n_n=n\times(n-1)\times(n-2)\times\dots\times1=n!
$$

sometimes when $k$ objects are chosen from a group of $n$ objects, the focus is on which $k$ objects are chosen but not their order.

such a collection is called a [[Combination|combination]] of $k$ objects from $n$ objects.

$$
C^n_k=\frac{n!}{(n-k)!\space k!}
$$

the formula for the number of combinations follows from the fact that each combination of $k$ objects can be associated with the $k$! permutations that consist of those objects.

$$
P^n_k=k!\times C^n_k
$$

so that,

$$
C^n_k=\frac{P^n_k}{k!}=\frac{n!}{(n-k)!\space k!}
$$

suppose that a company has four different kinds of products and wishes to compare them through product testing. a tester is given four different types of products and told to rate it. this procedure simply provides an ordering of the four products, and the number of possible ways in which it can be performed is

$$
P^4_4=4!=4\times3\times2\times1=24
$$

in a different test, each tester samples eight products and is asked to pick the best, the second best, and the third best. the number of possible answers to the test is then

$$
P^8_3=8\times7\times6=336
$$

notice that the order of the sequence is important. for example if the eight products in the taste test are labeled $A–H$, then the permutation $ABC$ (in which product $A$ is best, $B$, second best, and $C$ third best) is different from the permutation $ACB$.

