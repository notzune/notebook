# Concepts and Definitions

- [[Conditional probability distribution]]
- [[Continuous or discrete variable]]
- [[Cumulative distribution function (CDF)]]
- [[Disjoint event]]
- [[Independence]]
- [[Independent events]]
- [[Interquartile range (IQR)]]
- [[Joint probability distribution]]
- [[Algebra of random variables]]
- [[Marginal distribution]]
- [[Percentile]]
- [[Probability mass function (PMF)]]
- [[Quartile]]
- [[Random variables]]
- [[Symmetric probability distribution]]

# Formulas: 

## [[Expected value]]:

$$
E(X)=\sum_ip_ix_i
$$

## [[Weighted arithmetic mean]]

$$
\overline{x}=\frac{1}{n}(\sum^n_{i=1}x_i)=\frac{x_1+x_2+\dots+x_n}{n}
$$

## [[Chebyshev's inequality]]

$$
P(|X-\mu|\geq k\sigma)\leq\frac{1}{k^{2}}
$$
$$
P(\mu-k\sigma\leq X\leq\mu+k\sigma)=1-\frac{1}{k^{2}}
$$

## [[Variance]]

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