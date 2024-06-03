in [[Probability theory|probability theory]], a continuity correction is an adjustment that is made when a [[Continuous or discrete variable|discrete]] [[Probability distribution|distribution]] is approximated by a continuous distribution. 

## [[Binomial distribution]]

if a [[Random variables|random variable]] $X$ has a binomial distribution with [[Parameter (statistics)|parameters]] $n$ and $p$, (i.e. $X$ is distributed as the number of "successes" in $n$ independent [[Bernoulli trial]]s) with probability $p$ of success on each trial, then 

$$
P(X\leq x)=P(X<x+1)
$$

for any $x\in\{0,1,2,\dots n\}$. if $np$ and $np(1-p)$ are large (sometimes taken as both $\geq5$) then the probability above is fairly well approximated by

$$
P(Y\leq x+1/2)
$$

where $Y$ is a [[Normal distribution|normally distributed]] random variable with the same [[Expected value|expected value]] and the same [[Variance|variance]] as $X$, i.e. $E(Y)=np$ and $\text{var}(Y)=np(1-p)$. this addition of $1/2$ to $x$ is a continuity correction.

