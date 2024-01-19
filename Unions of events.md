in [[Probability theory|probability theory]], the [[Events|event]] $A\cup B$ is the [[Union|union]] of events $A$ and $B$ and consists of the outcomes that are contained within at least one of the events $A$ and $B$.

the [[Probability value|probability]] of this event ($P(A\cup B)$), is the probability that at least one of the events $A$ and $B$ occurs.

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