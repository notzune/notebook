in [[Probability theory|probability theory]] and [[Statistics|statistics]], the hypergeometric distribution is a [[Discrete probability distribution|discrete probability distribution]] that describes the probability of $k$ success (random draws for which the object drawn has a specified feature/quality) in $n$ draws, [[Replacement|without replacement]] from a finite population of size $N$ that contains exactly $K$ objects with that feature, wherein each draw is either a success or a failure.

in contrast, the [[Binomial distribution|binomial distribution]] describes the probability of $k$ successes in $n$ draws *with* replacement.
 
# [[Probability mass function (PMF)]]

the result of each draw (the elements of the population being sampled) can be classified into one of two [[Disjoint event|mutually exclusive events]] (pass/fail, broken/not broken, employed/not employed, etc.)

the probability of a success changes on each draw, as each draw decreases the population.

a [[Random variables|random variable]] $X$ follows the hypergeometric distribution if its PMF is given by:

$$
p_X(k)=\text{Pr}(X=k)=\frac{\binom{K}{k}\binom{N-K}{n-k}}{\binom{N}{n}}
$$

where

- $N$ is the population size
- $K$ is the number of success states in the population
- $n$ is the number of draws
- $k$ is the number of observed successes
- $\binom{a}{b}$ is a [[Binomial coefficient|binomial coefficient]]

it can also be re-arranged as 

$$
\frac{\binom{K}{k}\binom{N-K}{n-k}}{\binom{N}{n}}=\frac{\binom{n}{k}\binom{N-n}{K-k}}{\binom{N}{K}}
$$

## Example

consider an urn with two colors of marbles, red and green. 

define for this example a green marble as a success and drawing a red as a failure. let $N$ describe the number of all marbles in the urn, and $K$ describe the number of green marbles, then $N-K$ is the number of red marbles.

assume for sake of example there are $5$ green and $45$ red marbles in the urn, after drawing $10$ without replacement, what is the probability that exactly $4/10$ are green?

$$
P(X=4)=f(4;10,5,10)=\frac{\binom{5}{4}\binom{45}{6}}{\binom{50}{10}}=\frac{5\cdot8145060}{10272278170}=0.003964583\dots
$$

