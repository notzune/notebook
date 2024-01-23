in [[Probability theory|probability theory]] a conditional probability of [[Events|event]] $A$ conditional on event $B$ is

$$
P(A|B)=\frac{P(A\cup B)}{P(B)}\text{ for }P(B)>0
$$

it measures the [[Probability|probability]] that event $A$ occurs when it is known that event $B$ occurs.

one example of conditional probability is a situation in which two events $A$ and $B$ are [[Disjoint event|mutually exclusive]]. 

in this case, events $A$ and $B$ have no outcomes in common, so the occurrence of event $B$ prevents the possibility of event $A$ occurring. 

because of this, we can assert that the probability of event $A$ conditional on event $B$ must be zero:

$$
P(A|B)=0\text{ (if $A,B$ are disjoint)}
$$

since $A\cap B=\emptyset$ for mutually exclusive events, this assertion is in agreement with the formula

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}=\frac{0}{P(B)}=0
$$

another example of conditional probability is a situation where an event $B$ is [[Subset|contained]] within an event $A$, that is $B\subset A$.

if event $B$ occurs, we know (by definition) that event $A$ must also occur (since $B$ is a [[Subset|subset]] of $A$), so we can assert that the probability of $A$ conditional on event $B$ must be one.

since in this case $A\cap B=B$, we can prove this by using the formula

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}=\frac{P(B)}{P(B)}=1
$$

