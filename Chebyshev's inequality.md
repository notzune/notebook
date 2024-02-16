in [[Probability theory|probability theory]], Chebyshev's inequality provides a upper bound on the [[Probability|probability]] of [[Deviation|deviation]] of a [[Random variables|random variable]] (with finite [[Variance|variance]]) from its [[Weighted arithmetic mean|mean]].

in other words, the probability that a random variable deviates from its mean by more than $k\sigma$ is at most ${1}/{k^{2}}$, where $k$ is any positive [[Constant|constant]].

in mathematical terms,

$$
P(|X-\mu|\geq k\sigma)\leq\frac{1}{k^{2}}
$$

the inequality holds for any [[Probability distribution|probability distribution]]; it doesn't require the random variable to follow a [[Normal distribution|normal distribution]].

this inequality is useful for proving the [[Law of large numbers|law of large numbers]], and it's practical applications are similar to the [[68–95–99.7 rule]].

# Example

suppose that we have a random variable $X$ that represents the scores on a test. the mean score, $\mu$, is 75 and the variance, $\sigma^{2}$, is 16, which means the standard deviation $\sigma$ is 4 (since standard deviation ($\sigma$) is the square root of the variance)

we want to know what is the probability that a randomly selected test score deviates from the mean by more than 8 points

first we identify that 8 points away from the mean is $k\sigma$, where $k$ is our constant. since $\sigma=4$, then $8=2\sigma$, so $k=2$.

we then take the inequality:

$$
P(|X-\mu|\geq k\sigma)\leq\frac{1}{k^{2}}
$$

and plugi n $k=2$:

$$
P(|X-75|\geq 8)\leq\frac{1}{4}
$$

so that means the probability that a score is more than 8 points away from the mean is at most 25%.

this doesn't mean that exactly 25% of the scores will be outside of the range, it just means **at most** 25% will be.


