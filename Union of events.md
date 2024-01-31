in [[Probability theory|probability theory]], the [[Events|event]] $A\cup B$ is the [[Union|union]] of events $A$ and $B$ and consists of the outcomes that are contained within at least one of the events $A$ and $B$.

the [[Probability|probability]] of this event ($P(A\cup B)$), is the probability that at least one of the events $A$ and $B$ occurs.

since the probability of $A\cup B$ is obtained as the sum of the probability values of the outcomes within these two ([[Disjoint event|mutually exclusive]]) events, the following result is obtained:

$$
P(A\cup B)=P(A\cap B')+P(A'\cap B)+P(A\cap B)
$$

this equality can be presented in other forms using the following relationships between union and [[Intersection of events|intersection]]. (see also: [[De Morgan's Laws]] and [[Identities for set operations|set identities]])

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

if the events $A$ and $B$ are [[Disjoint event|mutually exclusive]] so that $P(A\cap B)=0$, then 

$$
P(A\cup B)=P(A)+P(B)
$$

(see also: [[Union of disjoint events|union of mutually exclusive events]])

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

logically, it follows that the union of an event and it's complement will always equal 1 (or more formally, the sample space $S$)

$$
P(A\cup A')=1
$$

# Example

to find the probability of picking a black ace from a  [[Deck of cards|standard deck of playing cards]],

we can first find the probability of event $A$:

$$
\text{picking a black card}\rightarrow P(A)=1/2
$$

because there are two black suits (13 cards each), out of the deck (52)$=36/52=1/2$. 

then we can find the probability of event $B$,

$$
\text{picking an ace}\rightarrow P(A)=1/13
$$

because there are 4 aces in a deck ($4/52=1/13$)

so to find the probability of picking a black ace we take the [[Intersection of events|intersection]] of these events:

$$
P(A\cap B)=1/26
$$

since there are only 2 black aces in the card

$$
\begin{align}
P(A\cup B)&=P(A)+P(B)-P(A\cap B) \\
\\
&=1/2+1/13-1/26 \\
\\
&=15/26-1/26 \\
\\
P(A\cup B)&=14/26=7/13
\end{align}
$$

so there's a $7/13$ or $\approx0.54\%$ chance of picking a black ace from a standard deck of cards.