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

# Examples

## Discrete Random Variable (Using [[Probability mass function (PMF)|PMF]] to find CDF)

suppose you have a discrete random variable $X$ that represents the number of heads when flipping a fair coin three times. the possible values of $X$ are ${0, 1, 2, 3}$.

the probability mass function, $P(X=x)$, might look like this:

- $P(X=0) = 0.125$ (getting all tails)
- $P(X=1) = 0.375$ (getting one head and two tails)
- $P(X=2) = 0.375$ (getting two heads and one tail)
- $P(X=3) = 0.125$ (getting all heads)

to find the cumulative distribution function, $F(x)$, you sum the probabilities for all outcomes up to and including $x$:

$$
F(x)=\sum_{y:y\leq x}P(X=y)
$$

so, $F(x)$ will be:

$$
\begin{align}
&F(0)&=P(X=0)&&=0.125 \\
&F(1)&=P(X=0)+P(X=1)&=0.125+0.375&=0.500 \\
&F(2)&=P(X=0)+P(X=1)+P(X=2)&=0.500+0.375&=0.875 \\
&F(3)&=P(X=0)+P(X=1)+P(X=2)+P(X=3)&=0.875+0.125&=1.000 \\
\end{align}
$$

## Continuous Random Variable (Using PDF and CDF)

consider a continuous random variable $X$ that has a uniform distribution between 0 and 1. the probability density function, $f_X(x)$, is:

$$
f_X(x) = \begin{cases} 
1 & \text{for } 0 \leq x \leq 1 \\
0 & \text{otherwise}
\end{cases}
$$

the cumulative distribution function, $F_X(x)$, is the integral of the probability density function from $-\infty$ to $x$:

$$
F_X(x)=\int^{x}_{-\infty}f_X(t)dt
$$

so, for $0 \leq x \leq 1$, $F_X(x)$ will be:

$$
F_X(x) = \int_{0}^{x} 1 dt = x
$$

and $F_X(x)$ will look like:

- $F_X(x) = 0$ for $x < 0$
- $F_X(x) = x$ for $0 \leq x \leq 1$
- $F_X(x) = 1$ for $x > 1$