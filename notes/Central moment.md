in [[Probability theory|probability theory]] and [[Statistics|statistics]], a central moment is a [[Moment|moment]] of a [[Probability distribution|probability distribution]] of a [[Random variables|random variable]] about the variable's [[Mean|mean]].

in other words, it is the [[Expected value|expected value]] of a specified integer power of the deviation of the random variable from the mean.

the $n$-th moment about the mean (or $n$-th central moment) of a [[Real numbers|real]]-valued random variable $X$ is the quantity $\mu_n:=\text{E}[(X-\text{E}[X])^n]$, where E is the expectation operator. 

for a continuous [[Univariate function|univariate]] probability distribution with [[Probability density function (PDF)|probability density function]] $f(x)$, the $n$-th moment about the mean $\mu$ is

$$
\mu_n=\text{E}[(X-\text{E}[X])^n]=\int^{+\infty}_{-\infty}(x-\mu)^nf(x)\text{d}x
$$

## Properties

for all $n$, the $n$-th central moment is [[Homogeneous functions|homogeneous]] of degree $n$:

$$
\mu_n(cX)=c^n\mu_n(X)
$$

***only*** for $n$ such that $n$ equals 1, 2, or 3 do we have an additivity property for random variables $X$ and $Y$ that are [[Independence|independent]]: 