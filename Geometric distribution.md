in [[Probability theory|probability theory]] and [[Statistics|statistics]], the geometric distribution is either one of two [[Discrete probability distribution|discrete probability distributions]]:

- the probability distribution of the number $X$ of [[Bernoulli trial|Bernoulli trials]] needed to get one success, supported on the set $\{1,2,3,\dots\}$
- the probability distribution of the number $Y=X-1$ of failures before the first success, supported on the set $\{0,1,2,\dots\}$

the geometric distribution gives the probability that the first occurrence of success requires $k$ independent trials, each with success probability $p$. if the probability of success on each trail is $p$, then the probability that the $k$-th trial is the first success is

$$
\begin{align}
\text{Pr}(X=k)&=(1-p)^{k-1}p \\
\\
\text{Pr}(X=k)&=q^{k-1}p \\
\end{align}
$$

for $k=1,2,3,4,\dots$

the above form is used for modeling the number of trials **up to and including the first success**.

the following form is used for modeling the number of failures until the first success:

$$
\begin{align}
&\text{Pr}(Y=k)=\text{Pr}(X=k+1)&=(1-p)^{k}p \\
\\
&\text{Pr}(Y=k)&=q^{k}p \\
\end{align}
$$

for $k=0,1,2,3,\dots$

in either case, the sequence of probabilities is a [[Geometric sequence|geometric sequence]].

# Example

a doctor is seeking an antidepressant for a newly diagnosed patient (who also happens to be a stats student). 

suppose that, of the available anti-depressant drugs, the probability that any particular drug will be effective for a particular patient is $p=0.6$. 

what is the probability that the first drug found to be effective for this patient is the first drug tested, the second drug tested, and so on?

the probability that the first drug works means that there are zero failures before the first success, $Y=0$.

$$
\text{Pr}(Y=0)=q^{0}p=0.4^{0}\times0.6=1\times0.6=0.6
$$

the probability that the first drug fails but the second drug works means there is one failure before the first success, $Y=1$.

$$
\text{Pr}(Y=1)=q^{1}p=0.4^{1}\times0.6=0.4\times0.6=0.24
$$

the probability that the first two drugs fail but the third drug works means there is two failures before the first success, $Y=2$.

$$
\text{Pr}(Y=2)=q^{2}p=0.4^{2}\times0.6=0.096
$$

and so on.

# [[Expected value]] and [[Variance]]

the expected value of a geometrically distributed [[Random variables|random variable]] is given as

$$
E(X)=\frac{1}{p}
$$

while the variance is given as

$$
\text{Var}(X)=\frac{1-p}{p^{2}}
$$
