in [[Probability theory|probability theory]], two [[Events|events]] $A$ and $B$ are said to be independent events if 

$$
P(B|A)=P(B)
$$

so that the [[Probability|probability]] of event $B$ remains the same whether or not the event $A$ is [[Conditional probability|conditioned]] upon. in other words, knowledge of the occurrence (or lack of occurrence) of event $A$ does not affect the probability of event $B$.

in this case

$$
P(A\cap B)=P(A)\space P(B|A)=P(A)\space P(B)
$$

and

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}=\frac{P(A)P(B)}{P(B)}=P(A)
$$

so the probability of event $A$ remains the same whether or not $B$ is conditioned upon, and the probability of both occurring ($P(A\cap B)$) is obtained simply by multiplying together the individual probabilities of the two events $P(A)$ and $P(B)$. 

the probability of the [[Intersection of events|intersection]] of a series of independent events $A_1,\dots,A_n$ is given by

$$
P(A_1\cap\dots\cap A_n)=P(A_1)P(A_2)\dots P(A_n)
$$

see also: [[Disjoint event|disjoint event]]