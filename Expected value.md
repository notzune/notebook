in [[Probability theory|probability theory]], the expected value (also known as the expectation, expectancy, expectation operator, mean, expectation value, or first [[Moment|moment]]) is a generalization of the [[Weighted arithmetic mean|weighted average]].

the expected value of a random variable with a finite number of outcomes is a weighted average of all possible outcomes. in the case of continuum of possible outcomes, the expectation is defined by [[Integral|integration]]. 

the expected value of a random variable $X$ is often denoted by E($X$), E$[X]$, or E$X$; with E often stylized as $E$ or $\mathbb{E}$. 

the expected value or expectation of a [[Continuous or discrete variable|discrete]] [[Random variables|random variable]] with a [[Probability mass function (PMF)|probability mass function]] $P(X=x_i)=p_i$ is 

$$
E(X)=\sum_ip_ix_i
$$

$E(X)$ provides the [[Weighted arithmetic mean|mean]] of the random variable.

# Examples

let $X$ represent the outcome of a roll of a fair six-sided [[Dice (die)|die]]. more specifically, $X$ is the number of [[Pip (counting)|pips]] showing on the top face of the die after the toss.

the possible values for $X$ are $1,2,3,4,5$ and $6$, all of which are equally likely with a probability of $1/6$,

the expectation ($E(X)$) of $X$ is then

$$
E(X)=1\cdot\frac{1}{6}+2\cdot\frac{1}{6}+3\cdot\frac{1}{6}+4\cdot\frac{1}{6}+5\cdot\frac{1}{6}+6\cdot\frac{1}{6}=3.5
$$

if one rolls the die $n$ times and computes the average ([[Arithmetic mean|arithmetic mean]]) of the results, then as $n$ grows, the average will almost surely [[Limit of a sequence|converge]] to the expected value, a fact known as the [[Law of large numbers|law of large numbers]].

another example is a game of roulette, which is a game that consists of a small ball and a wheel with 38 numbered pockets around the edge. as the wheel is spun, the ball bounces around randomly until it settles into a pocket. 

suppose the random variable $X$ represents the outcome of a \$1 bet on a single number. the probability of the bet winning is $1/38$, and the payoff is \$35, otherwise the player loses the bet (\$-1).

the expected profit from such a bet will be:

$$
E(\text{gain from \$1 bet})=-\$1\cdot\frac{37}{38}+$35\cdot\frac{1}{38}=-\$\frac{1}{19}
$$

so the expected value to be won from a \$1 bet is -\$1/19, so in 190 bets the net loss would be around \$10.
