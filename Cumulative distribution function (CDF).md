in [[Probability theory|probability theory]] and [[Statistics|statistics]], the cumulative distribution function (CDF) of a real-valued [[Random variables|random variable]] $X$, or just distribution function of $X$, evaluated at $x$, is the [[Probability|probability]] that $X$ will take a value less than or equal to $x$.

the cumulative distribution function is an alternate way of specifying the probabilistic properties of a [[Random variables|random variable]] $X$ with the function

$$
F(x)=P(X\leq x)
$$
where the right-hand side represents the probability that the random variable $X$ takes on a value less than or equal to $x$.

the probability that $X$ lies in the semi-closed [[Interval|interval]] $(a,b]$, where $a<b$, is therefore

$$
P(a<X\leq b)=F_X(b)-F_X(a)
$$

the cumulative distribution function can be used to calculate the [[Probability mass function (PMF)|probability mass function]] and vice versa.

for example, suppose the mass function is known, the cumulative distribution function can then be calculated from the expression

$$
F(x)=\sum_{y:y\leq x}P(X=y)
$$

in other words, the value of $F(x)$ is constructed by simply adding together the probabilities $P(X=y)$ for values $y$ that are no larger than $x$.

the probability density function of a continuous random variable can be determined from the cumulative distribution function by differentiating using the [[Fundamental theorem of calculus|fundamental theorem of calculus]] as long as the [[Derivative|derivative]] exists.; i.e. given $F(x)$,

$$
f(x)=\frac{dF(x)}{dx}
$$

the CDF of a continuous random variable $X$ can be expressed as the [[Integration|integral]] of its [[Probability density function (PDF)|probability density function]] $f_X$ as follows:

$$
F_X(x)=\int^{x}_{-\infty}fx(t)dt
$$