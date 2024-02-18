the weak law of large numbers is a central theorem in the study of [[Probability theory|probability theory]]. it states that the [[Arithmetic mean|average]] of the results obtained from a large number of [[Independence|independent]] and identical random samples [[Convergence and divergence|converges]] to a true value if it exists.

let $X_1,\dots,X_n$ be a [[Sequence|sequence]] of independent and identically [[Probability distribution|distributed]] random variables, each having a [[Weighted arithmetic mean|mean]] $\langle X_i\rangle=\mu$  and [[Standard deviation|standard deviation]] $\sigma$,

$$
X=\frac{X_1+\dots+X_n}{n}
$$

then as $n\rightarrow\infty$, the sample mean $\langle x\rangle$ equals the population mean $\mu$ of each variable

$$
\begin{align}
\langle X\rangle&=\left\langle\frac{X_1+\dots+X_n}{n}\right\rangle \\
\\
&=\frac{1}{n}(\langle X_1\rangle+\dots+\langle X_n\rangle) \\
\\
&=\frac{n\,\mu}{n} \\
\\
&=\mu
\end{align}
$$

the [[Variance|variance]] also follows,

$$
\begin{align}
\text{Var}(X)&=\text{Var}\left(\frac{X_1+\dots+X_n}{n}\right) \\
\\
&=\text{Var}\left(\frac{X_1}{n}\right)+\dots+\text{Var}\left(\frac{X_n}{n}\right) \\
\\
&=\frac{\sigma^{2}}{n^{2}}+\dots+\frac{\sigma^{2}}{n^{2}} \\
\\
&=\frac{\sigma^{2}}{n} \\
\end{align}
$$

therefore, by [[Chebyshev's inequality]], for all $\epsilon>0$,

$$

$$