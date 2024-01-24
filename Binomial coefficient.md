in math, the binomial coefficients are the positive [[Integer|integers]] that occur as [[Coefficient|coefficients]] in the [[Binomial theorem|binomial theorem]].

commonly, a binomial coefficient is indexed by a pair of integers $n\geq  k\geq0$ and is written as $\binom{n}{k}$.

it is the coefficient of the $x^k$ term in the polynomial expansion of the binomial power $(1+x)^n$.

this coefficient can be computed by the multiplicative formula

$$
\binom{n}{k}=\frac{n\times(n-1)\times\dots\times(n-k+1)}{k\times(k-1)\times\dots\times1}
$$

or by using [[Factorial|factorial notation]], can be expressed as

$$
\binom{n}{k}=\frac{n!}{k!\space(n-k)!}
$$

for example, the fourth power of $1+x$ is

$$
\begin{align}

(1+x)^4&=\binom{4}{0}x^0+\binom{4}{1}x^1+\binom{4}{2}x^2+\binom{4}{3}x^3+\binom{4}{4}x^4 \\
\\
&=1+4x+6x^2+4x^3+x^4 \\
\\
\text{ where }
&=\binom{4}{0}=1 \\
&\dots \\
&=\binom{4}{2}=\frac{4\times3}{2\times1}=\frac{4!}{2!\space2!}=6 \\
&\text{etc}\dots
\end{align}
$$

arranging the numbers $\binom{n}{0},\binom{n}{1},\dots,\binom{n}{n}$ in successive rows for $n=0,1,2,\dots$ gives [[Pascal's triangle]] which satisfies the [[Recurrence relation|recurrence relation]]:

$$
\binom{n}{k}=\binom{n-1}{k-1}+\binom{n-1}{k}
$$

