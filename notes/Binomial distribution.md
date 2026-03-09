in [[Probability theory|probability theory]] and [[Statistics|statistics]], the binomial distribution with [[Parameter (statistics)|parameters]] $n$ and $p$ is the [[Continuous or discrete variable|discrete]] [[Probability distribution|probability distribution]] of the number of successes in a [[Sequence|sequence]] of $n$ [[Independence|independent]] "experiments", each asking a "yes-no" question and each with its own [[Boolean|boolean]]-valued [[Outcome|outcome]]: *success* (with probability $p$) or *failure* (with probability $q=1-p$).

single success/failure experiment is also called a [[Bernoulli trial|Bernoulli trial]] and the sequence of outcomes is called a [[Bernoulli process]]

# [[Probability mass function (PMF)]]

in general, if the [[Random variables|random variable]] $X$ follows the binomial distribution with parameters $n\in\mathbb{N}$ and $p\in[0,1]$, we write $X$ ~ $\text{B}(n,p)$. the probability of getting exactly $k$ success in $n$ independent Bernoulli trials (with the same rate $p$) is given by the PMF:

$$
\begin{align}
f(k,n,p)&=\text{Pr}(k;n,p) \\
\\
&=\text{Pr}(X=k) \\
\\
&=\binom{n}{k}p^{k}(1-p)^{n-k} \\
\end{align}
$$

for $k=0,1,2,\dots,n$, where

$$
\binom{n}{k}=\frac{n!}{k!(n-k)!}
$$

is the [[Binomial coefficient|binomial coefficient]], hence the name of the distribution. 

the formula can be understood as:

$k$ success occur with probability $p^{k}$ and $n-k$ failures occur with probability $(1-p)^{n-k}$, however the $k$ successes can occur anywhere among the $n$ trials, and there are $\binom{n}{k}$ different ways of distributing $k$ successes in a sequence of $n$ trials.

## Example

suppose a [[Fair coin|biased coin]] comes up heads with probability $0.3$ when tossed. the probability of seeing exactly 4 heads in 6 tosses is:

$$
f(4,6,0.3)=\binom{6}{4}0.3^{4}(1-0.3)^{6-4}=0.059535
$$

# [[Cumulative distribution function (CDF)]]

the cumulative distribution function can be expressed as:

$$
F(k;n,p)=\text{Pr}(X\leq k)=\sum^{⌊k⌋​}_{i=0}\binom{n}{i}p^{i}(1-p)^{n-i}
$$

where $⌊k⌋​$ is the "[[Floor and ceiling functions|floor]]" under $k$; the greatest integer less than or equal to $k$.

# Properties

## [[Expected value]] and [[Variance|variance]]

if $X$ ~ $B(n,p)$, that is $X$ is a binomially distributed random variable, $n$ being the total number of experiments and $p$ the probability of each yielding a successful result, then the expected value of $X$ is:

$$
E(X)=np
$$

this follows from the linearity of the expected value along with the fact that $X$ is the sum of $n$ identical Bernoulli random variables, each with expected value $p$.

in other words, if $X_1,\dots,X_n$ are identical (and [[Independence|independent]]) Bernoulli random variables with parameter $p$, then $X=X_1+\dots+X_n$ and

$$
\begin{align}
E(X)&=E(X_1+\dots+X_n) \\ 
\\
&=E(X_1)+\dots+E(X_n) \\
\\
&=p+\dots+p \\
\\
&=np
\end{align}
$$

the variance is then:

$$
\text{Var}(X)=npq=np(1-p)
$$

this is because the variance of a sum of independent random variables is the sum of the variances.

## Higher [[Moment|moments]]

the first 6 [[Central moment|central moments]], defined as $\mu_{c}=E((X-E(X))^{c})$, are given by

$$
\begin{align}
\mu_1&=0, \\
\mu_2&=np(1-p), \\
\mu_3&=np(1-p)(1-2p), \\
\mu_4&=np(1-p)(1 + (3n-6)p(1-p)), \\
\mu_5&=np(1-p)(1-2p)(1 + (10n-12)p(1-p)), \\
\mu_6&=np(1-p)(1-30p)(1-p)(1-4p(1-p))+5np(1-p)(5-26p(1-p))+15n^{2}p^{2}(1-p)^{2}).
\end{align}
$$

the non-central moments satisfy

$$
\begin{align}
E(X)&=np \\
E(X^{2})&=np(1-p)+n^{2}p^{2}
\end{align}
$$

and in general,

$$
E(X^{c})=\sum _{k=0}^{c}\left\{{c\atop k}\right\}\,n^{\underline{k}}p^{k}
$$

where $\left\{{c\atop k}\right\}$ are the [[Stirling numbers|Stirling numbers of the second kind]], and $n^{\underline{k}}=n(n-1)\dots(n-k+1)$ is the $k$th [[Falling and rising factorials|failing power]] of $n$.




