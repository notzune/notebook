in [[Probability theory|probability theory]], the [[Events|event]] $A\cup B$ is the [[Union|union]] of events $A$ and $B$ and consists of the outcomes that are contained within at least one of the events $A$ and $B$.

the [[Probability|probability]] of this event ($P(A\cup B)$), is the probability that at least one of the events $A$ and $B$ occurs.

since the probability of $A\cup B$ is obtained as the sum of the probability values of the outcomes within these three (mutually exclusive) events, the following result is obtained:

$$
P(A\cup B)=P(A\cap B')+P(A'\cap B)+P(A\cap B)
$$

this equality can be presented in other forms using the following relationships

$$
P(A\cap B')=P(A)-P(A\cap B)
$$

and

$$
P(A'\cap B)=P(B)-P(A\cap B)
$$

substituting in these expressions for $P(A\cap B')$ and $P(A'\cap B)$ gives the result:

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$

if the events $A$ and $B$ are mutually exclusive so that $P(A\cap B)=0$, then 

$$
P(A\cup B)=P(A)+P(B)
$$

in the case of $(A\cup B)'$, it can also be written as $A'\cup B'$

$$
(A\cup B)'=A'\cup B'
$$

the probability of the union of three events $A$, $B$, and $C$ is the sum of the probability values of the simple outcomes that are contained within at least one of the three events

it can also be calculated from the expression

$$
\begin{align}
P(A\cup B\cup C)&=[P(A)+P(B)+P(C)] \\
&-[P(A\cap B)+P(A\cap C)+P(B\cap C)] \\
&+P(A\cap B\cap C)
\end{align}
$$

(see also: [[Union of disjoint events|union of mutually exclusive events]])