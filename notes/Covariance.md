in [[Probability theory|probability theory]] and [[Statistics|statistics]], the covariance is a measure of the joint variability of two [[Random variables|random variables]]. 

for two [[Joint probability distribution|jointly distributed]] [[Real numbers|real]]-valued random variables $X$ and $Y$ with finite [[Moment|second moments]], the covariance is defined as the [[Expected value|expected value]] (or [[Weighted arithmetic mean|mean]]) of the product of their [[Standard deviation|deviations]] from their individual expected values:

$$
\text{Cov}(X,Y)=E((X-E(X))(Y-E(Y)))
$$

where $E(X)$ is the expected value of $X$, also known as the mean of $X$. 

the covariance is sometimes denoted as $\sigma_{XY}$ or $\sigma(X,Y)$.

by using the linearity property of expectations, this definition can be simplified to the expected value of their product minus the product of their expected values:

$$
\begin{align}
\text{Cov}(X,Y)&=E((X-E(X))(Y-E(Y))) \\
\\
&=E(XY-X\,E(Y))-E(X\mid Y+E(X)E(Y)) \\
\\
&=E(XY)-E(X)E(Y)-E(X)E(Y)+E(X)E(Y) \\
\\
&=E(XY)-E(X)E(Y) \\
\end{align}
$$