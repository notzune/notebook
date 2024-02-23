in [[Probability theory|probability theory]] and [[Statistics|statistics]], the binomial distribution with [[Parameter (statistics)|parameters]] $n$ and $p$ is the [[Continuous or discrete variable|discrete]] [[Probability distribution|probability distribution]] of the number of successes in a [[Sequence|sequence]] of $n$ [[Independence|independent]] "experiments", each asking a "yes-no" question and each with its own [[Boolean|boolean]]-valued [[Outcome|outcome]]: *success* (with probability $p$) or *failure* (with probability $q=1-p$).

single success/failure experiment is also called a [[Bernoulli trial|Bernoulli trial]] and the sequence of outcomes is called a [[Bernoulli process]]

# Probability mass function (PMF)

in general, if the [[Random variables|random variable]] $X$ follows the binomial distribution with parameters $n\in\mathbb{N}$ and $p\in[0,1]$, we write $X$ ~ $\text{B}(n,p)$. the probability of getting exactly $k$ success in $n$ independent Bernoulli trials (with the same rate $p$) is given by the [[Probability mass function (PMF)|PMF]]:

$$
f(k,n,p)=\text{Pr}(k;n,p)=\text{Pr}(X=k)=\binom{n}{k}p^{k}(1-p)^{n-k}
$$

for $k=0,1,2,\dots,n$, where

$$
\binom{n}{k}=\frac{n!}{k!(n-k)!}
$$

is the [[Binomial coefficient|binomial coefficient]], hence the name of the distribution. 

the formula can be understood as:

$k$ success occur with probability $p^{k}$ and $n-k$ failures occur with probability $(1-p)^{n-k}$, however the $k$ successes can occur anywhere among the $n$ trials, and there are $\binom{n}{k}$ different ways of distributing $k$ successes in a sequence of $n$ trials.

