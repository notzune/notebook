a machine produces iron bars whose lengths have a [[Weighted arithmetic mean|mean]] ($\mu$) of $110.8$ cm and a [[Standard deviation|standard deviation]] of $0.5$ cm. we want to find the lower bound on the [[Probability|probability]] that an iron bar chosen at random has a length between $109.55$ cm and $112.05$ cm.

we can use [[Chebyshev's inequality]] to calculate the lower bound[^1]:

$$
P(|X-\mu|\geq k\sigma)\leq\frac{1}{k^{2}}
$$

to find how many standard deviations away the desired interval is, we can subtract the mean in-order to find $k$ (the number of standard deviations away from the mean):

$$
\begin{align}
110.8-109.55=1.25/0.5=2.5 \\
112.05-110.8=1.25/0.5=2.5 \\
\end{align}
$$

once we calculate $k$, we can plug everything into the formula:

$$
\begin{align}
P(|X-110.8|\geq2.5)&\leq\frac{1}{2.5^{2}} \\
\\
&\leq\frac{1}{6.25}=0.16
\end{align}
$$

so the lower bound of the probability $P(X)$ of a random iron bar having a length between $109.55$ cm and $112.05$ cm is $0.16$ or $16\%$, to find the upper bound we subtract this from $1$:

$$
1-0.16=0.84
$$

now that we have the upper bound, we can write the probability that $X$ will fall between that interval as such:

$$
P(109.55\leq X\leq112.05)\geq0.84\text{ or }84\%
$$

[^1]: i'm not sure if this was a typo, because Chebyshev's can only provide an upper bound so I don't completely understand what the question is asking