in [[Probability theory|probability theory]] and [[Statistics|statistics]], variance is the [[Expected value|expected value]] of the [[Squared deviations from the mean (SDM)|squared deviations from the mean]] of a [[Random variables|random variable]]. 

the [[Standard deviation|standard deviation]] is obtained as the square root of the variance. 

variance is a measure of [[Dispersion|dispersion]], meaning it is a measure of how far a set of numbers is spread out from their average value. it is the second [[Central moment|central moment]] of a distribution, and the [[Covariance|covariance]] of the random variable with itself.

it is often denoted by $\sigma^2$, $s^2$, $\text{Var}(X), V(X)$, or $\mathbb{V}(X)$.

## Definition

the variance of a random variable $X$ is the [[Expected value|expected value]] of the squared deviation from the mean of $X$, $\mu=\text{E}[X]$:

$$
\text{Var}(X)=\text{E}[(X-\mu)^2]
$$

or in other words, is the deviation from the [[Expected value|expectance]]:

$$
\text{Var}(X)=\text{E}[(X-\text{E}(X))^2]
$$

and it can be expanded like so:

$$
\begin{align}
\text{Var}(X)&=\text{E}[(X-\text{E}(X))^{2}] \\
\\
&=\text{E}[X^{2}-2X\,\text{E}(X)+\text{E}(X)^{2}] \\
\\
&=\text{E}[X^{2}]-2\text{E}(X)\text{E}(X)+\text{E}(X)^{2} \\
\\
&=\text{E}[X^{2}]-\text{E}(X)^{2} \\
\end{align}
$$

or alternatively, can be thought of as:

$$
\begin{align}
\text{Var}(X)&=E((X-E(X))^{2}) \\
\\
&=\sum(P(X)\cdot(X-E(X))^{2}) \\
\end{align}
$$

the variance can also be thought of as the covariance of a random variable with itself:

$$
\text{Var}(X)=\text{Cov}(X,X)
$$

and you can also express it in terms of [[Expected value|expectation]]:

$$
E(X^{2})-E(X)^{2}=\text{Var}(X)=\text{Cov}(X,X)
$$

# Discrete random variables

if the generator of a random variable $X$ is [[Continuous or discrete variable#Discrete variable|discrete]] with [[Probability mass function (PMF)|PMF]] $x_1\mapsto p_1,x_2\mapsto p_2,\dots,x_n\mapsto p_n$, then 

$$
\text{Var}(X)=\sum^{n}_{i-1}p_i\cdot(x_i-\mu)^{2}
$$

where $\mu$ is the expected value; that is,

$$
\mu=\sum^{n}_{i-1}p_i\cdot x_i
$$

when such a discrete [[Weighted arithmetic mean|weighted variance]] is specified by weights whose sum is not 1, then one divides by the sum of the weights
 