in [[Probability theory|probability theory]] and [[Statistics|statistics]], the negative binomial distribution is a [[Discrete probability distribution|discrete probability distribution]] that models the number of failures in  a sequence of [[Independence|independent]] and identically distributed [[Bernoulli trial|Bernoulli trials]] before a specified (non-random) number of successes ($r$) occurs. 

for example, we can define rolling a 6 on a dice as a success, and rolling any other number as a failure, and ask how many failure rolls will occur before we see the third success ($r=3$).

in such a case, the probability distribution of the number of failures that appear will be a negative binomial distribution.

# [[Probability mass function (PMF)]]

the PMF of the negative binomial distribution is

$$
f(k;r,p)\equiv\text{Pr}(X=k)=\binom{k+r-1}{k}(1-p)^{k}p^{r}
$$

where $r$ is the number of success, $k$ is the number of failures, and $p$ is the probability of success on each trial.

the quantity in parentheses is the [[Binomial coefficient|binomial coefficient]], and is equal to

$$
\binom{k+r-1}{k}=\frac{(k+r-1)!}{(r-1)!(k)!}=\frac{(k=r-1)(k+r-2)\dots(r)}{k!}
$$

there are $k$ failures chosen from $k+r-1$ trails rather than $k+r$ because the last of the $k+r$ trials is by definition a success.

