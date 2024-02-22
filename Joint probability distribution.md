given two [[Random variables|random variables]] that are defined on the same [[Probability space|probability space]], the joint [[Probability distribution|probability distribution]] is the corresponding probability distribution on all possible pairs of outputs.

# Examples

## Coin flip

consider the flip of two fair coins; let $A$ and $B$ be [[Continuous or discrete variable#Discrete variable|discrete]] random variables associated with the [[Outcome|outcomes]] of the first and second coin flips, respectively.

each coin flip is a [[Bernoulli trial (Bernoulli random variables)]] and has a [[Bernoulli distribution]]. if a coin displays "heads" then the associated random variable takes the value $1$, and it takes the value $0$ otherwise.

the probability of each of these outcomes is $1/2$, so the [[Marginal distribution#PDF|marginal]] (unconditional) density functions are

$$
\begin{align}
P(A)=1/2\text{ for }A\in\{0,1\} \\
\\
P(B)=1/2\text{ for }B\in\{0,1\} \\
\end{align}
$$

the joint probability mass function of $A$ and $B$ defines probabilities for each pair of outcomes; all possible outcomes are:

$$
(A=0,B=0),\,(A=0,B=1),\,(A=1,B=0),\,(A=1,B=1)
$$

since each outcome is equally likely, the [[Joint probability mass function|joint probability mass function]] becomes

$$
P(A,B)=1/4\text{ for }A,B\in\{0,1\}
$$

and since the flips are [[Disjoint event|independent]], the joint probability mass function is the product of the marginals:

$$
P(A,B)=P(A)P(B)\text{ for }A,B\in\{0,1\}
$$