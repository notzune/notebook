in [[Probability theory|probability theory]], the law (or formula) of total probability is a rule relating [[Marginal distribution|marginal probabilities]] to [[Conditional probability|conditional probabilities]].

## Definition

let $A_1,\dots,A_n$ be a partition of a [[Sample space|sample space]] $S$ so that the events $A_i$ are [[Disjoint event|mutually exclusive]] with

$$
S=A_1\cup\dots\cup A_n
$$

suppose that the probabilities of these $n$ events ($P(A_1),\dots,P(A_n)$) are known, and consider an event $B$  as shown in the figure below, and suppose that the conditional probabilities $P(B|A_1),\dots,P(B|A_n)$ are also known.

![[Screenshot 2024-01-20 at 3.46.19 PM.png]]

the question then becomes how to use the probabilities $P(A_i)$ and $P(B|A_i)$ to calculate the probability of $B$. 

we can calculate $P(B)$ by noting that

$$
B=(A_1\cap B)\cup\dots\cup(A_n\cap B)
$$

where the events $A_i\cap B$ are disjoint, so that

$$
\begin{align}
P(B)&=P(A_1\cap B)+\dots+P(A_n\cap B) \\
\\
&=P(A_1)P(B|A_1)+\dots+P(A_n)P(B|A_n)
\end{align}
$$

this result is known as the law of total probability and states that if one and only one of a series of events $A_i$ can occur, then the probability of another event $B$ can be obtained as the weighted average of the conditional probabilities $P(B|A_i)$, with weights equal to the probabilities $P(A_i)$.

more generally, if $A_1,\dots,A_n$ is a [[Partition (probability theory)|partition]] of a [[Sample space|sample space]], then the probability of an event $B$ can be obtained from the probabilities $P(A_i)$ and $P(B|A_i)$ using the formula:

$$
P(B)=P(A_1)P(B|A_1)+\dots+P(A_n)P(B|A_n)
$$

or it can also be written as

$$
P(B)=\sum_nP(B\cap A_n)
$$

or as

$$
P(B)=\sum_nP(B|A_n)P(A_n)
$$

## In [[Conditional probability|conditional probabilities]]

taking the $A_n$ as above, and assuming that $C$ is an event [[Independent events|independent]] of any of the $A_n$

$$
\begin{align}
P(B|C)&=\frac{P(B,C)}{P(C)}=\frac{\sum_nP(B,A_n,C)}{P(C)}\\
\\
&=\frac{\sum_nP(B|A_n,C)P(A_n|C)P(C)}{P(C)} \\
\\
&=\sum_nP(B|A_n,C)P(A_n,|C)
\end{align}
$$