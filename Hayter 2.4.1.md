this problem is an example of calculating the [[Expected value|expectation]] and [[Variance|variance]] of a [[Random variables|random variable]].

suppose that the random variable $C$ takes the values $-2,1,4,$ and $6$ with [[Probability|probability values]] $\frac{1}{3},\frac{1}{6},\frac{1}{3},$ and $\frac{1}{6}$, respectively. 

# Finding the expectation

we are already given the [[Probability mass function (PMF)|PMF]] of the random variable $X$:

$$
\begin{align}
&p_X(-2)&=P(X=-2)&=\frac{1}{3} \\
\\
&p_X(1)&=P(X=1)&=\frac{1}{6} \\
\\
&p_X(4)&=P(X=4)&=\frac{1}{3} \\
\\
&p_X(6)&=P(X=6)&=\frac{1}{6} \\
\end{align}
$$

which we can plug into the formula to find the expectation $E(X)$:

$$
E(X)=-2\cdot\frac{1}{3}+1\cdot\frac{1}{6}+4\cdot\frac{1}{3}+6\cdot\frac{1}{6}\approx1.8\overline{3}
$$

# Finding the variance

the problem then asks us to find the variance of $X$ using the formula

$$
\text{Var}(X)=E((X-E(X))^{2})
$$

since we know $E(X)$, we can plug in the different values of $X$:

$$
\begin{align} \text{Var}(X)&=E((X-E(X))^{2}) \\ 
\\ 
&=\sum(P(X)\cdot(X-E(X))^{2}) \\ 
\\ 
&P(-2)\cdot(-2-1.83)^{2}&=\frac{1}{3}\cdot(-2-1.83333)^{2}&\approx4.898 \\ 
&P(1)\cdot(1-1.83)^{2}&=\frac{1}{6}\cdot(1-1.83333)^{2}&\approx0.116 \\ &P(4)\cdot(4-1.83)^{2}&=\frac{1}{3}\cdot(4-1.83333)^{2}&\approx1.565 \\ &P(6)\cdot(6-1.83)^{2}&=\frac{1}{6}\cdot(6-1.83333)^{2}&\approx2.894 \\ 
\\ 
&&\text{Var}(X)&\approx9.473 
\end{align}
$$

# Finding the variance with alternative formula

the problem then gives us an alternative formula and asks us to use it to compute the variance:

$$
\text{Var}(X)=E(X^{x})-(E(X))^{2}
$$

this formula breaks down into two parts:

1. $E(X^{2})$ - is the expected value of the square of the random variable $X$, to calculate it you square each possible value of $X$ then multiply each by it's corresponding probability and then sum those products.
2. $(E(X))^{2}$ - the square of the expected value of $X$ which we already calculated in the [[#Finding the expectation|first part]].

$$
E(X^{2})=(-2)^{2}\cdot\frac{1}{3}+(1)^{2}\cdot\frac{1}{6}+(4)^{2}\cdot\frac{1}{3}+(6)^{2}\cdot\frac{1}{6}\approx12.8\overline{3}
$$

plugging this back into the formula given to us we get:

$$
\begin{align}
\text{Var}(X)&=E(X^{x})-(E(X))^{2} \\
\\
&\approx12.8\overline{3}-(1.8\overline{3})^{2} \\
&\approx12.8333-3.3611 \\
\\
\text{Var}(X)&\approx9.4722
\end{align}
$$

as we can see this is close to the variance we got in the [[#Finding the variance|second part]].