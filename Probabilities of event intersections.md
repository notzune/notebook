based on the definition of a [[Conditional probability|conditional probability]] ($P(A|B)$), the probability of an [[Events|event]] [[Intersection of events|intersection]] can be expressed as

$$
P(A\cap B)=P(B)\space P(A|B)
$$

in other words, the [[Probability|probability]] of events $A$ and $B$ both occurring can be obtained by multiplying the probability of event $B$ by the probability of event $A$ conditional on $B$. 

this behavior is due to the [[General Multiplication Law of Probability|general multiplication law of probability]].

by definition, you can also calculate the probability of event $B$ conditional on $A$ in the same way.

$$
P(A\cup B)=P(A)\space P(B|A)
$$

therefore it does not matter which of the two events $A$ or $B$ is being conditioned upon. more generally,

$$
P(C|A\cap B)=\frac{P(A\cap B\cap C)}{P(A\cap B)}
$$

so the probability of the [[Intersection of events|intersection]] of three events can be calculated as 

$$
P(A\cap B\cap C)=P(A\cap B)\space P(C|A\cap B)=P(A)\space P(B|A)\space P(C|A\cap B)
$$

thus the probability of all three events occurring can be obtained by multiplying together the probability of one event, the probability of a second conditioned on the first event, and probability of the third event conditioned on the intersection of the first and second events.

we can get the following multiplication law for the intersection of a series of events

$$
P(A_1\cap\dots\cap A_n)=P(A_1)\times P(A_2|A_1)\times P(A_3|A_1\cap A_2)\times\dots\times P(A_n|A_1\cap\dots\cap A_{n-1})
$$

