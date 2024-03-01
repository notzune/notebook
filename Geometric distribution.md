in [[Probability theory|probability theory]] and [[Statistics|statistics]], the geometric distribution is either one of two [[Discrete probability distribution|discrete probability distributions]]:

- the probability distribution of the number $X$ of [[Bernoulli trial|Bernoulli trials]] needed to get one success, supported on the set $\{1,2,3,\dots\}$
- the probability distribution of the number $Y=X-1$ of failures before the first success, supported on the set $\{0,1,2,\dots\}$

the geometric distribution gives the probability that the first occurrence of success requires $k$ independent trials, each with success probability $p$. if the probability of success on each trail is $p$, then the probability that the $k$-th trial is the first success is

$$
\text{Pr}(X=k)=(1-p)^{k-1}p
$$

for $k=1,2,3,4,\dots$

the above form is used for modeling the number of trials **up to and including the first success**.

the following form is used for modeling the number of failures until the first success:

$$
\text{Pr}(Y=k)=\text{Pr}(X=k+1)=(1-p)^{k}p
$$

for $k=0,1,2,3,\dots$

in either case, the sequence of probabilities is a [[Geometric sequence|geometric sequence]].