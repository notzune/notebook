in math, the moments of a [[Function|function]] are certain quantitative measures related to the shape of the function's graph.

in [[Physics|physics]], if the function represents mass density, then the zeroth moment is the total mass, the first moment (normalized by total mass) is the [[Center of mass|center of mass]], and the second moment is the [[Moment of inertia|moment of inertia]].

in [[Statistics|statistics]], if the function is a [[Probability distribution|probability distribution]], then the first moment is the [[Expected value|expected value]], the second central moment is the variance, the third standardized moment is the skewness, and the fourth standardized moment is the kurtosis.

for a distribution of mass or probability on a bounded interval, the collection of all the moments (of all orders, from $0$ to $\infty$) determines the distribution ([[Hausdorff moment problem]]). the same is not true on unbounded intervals ([[Hamburger moment problem]]).

## Definition 

the $n$-th raw moment (moment about zero) of a distribution is defined by

$$
\mu'_n = \langle x^n \rangle,\text{ where }
\begin{align}
\langle f(x)\rangle= 
\begin{cases}
\sum f(x)P(x),&\text{discrete distribution} \\
\\
\int f(x)P(x)dx,&\text{continuous distribution} \\
\end{cases}
\end{align}
$$

the $n$-th moment of a [[Real numbers|real]]-valued [[Continuous function|continuous function]] $f(x)$ of a real variable about a value $c$ is the [[Integral|integral]]

$$
\mu_n=\int^\infty_{-\infty}(x-c)^nf(x)\text{ d}x
$$

if $f$ is a [[Probability density function (PDF)|probability density function]], then the value of the integral above is called the $n$-th moment of the [[Probability distribution|probability distribution]].

more generally, if $F$ is a [[Cumulative distribution function (CDF)|cumulative probability distribution function]] of any probability distribution, which may not have a density function, then the $n$-th moment of the probability distribution is given by the Riemann-Stietjes integral

$$
\mu'_n=\text{E}[X^n]=\int^\infty_{-\infty}x^n\text{d}F(x)
$$

where $x$ is a [[Random variables|random variable]] that has a cumulative distribution $F$, and E is the [[Expected value|expected value]] or mean. when

$$
\text{E}[|X^n|]=\int^\infty_{-\infty}|x^n|\text{d}F(x)=\infty
$$

the moment is said not to exist. if the $n$-th moment about any point exists, so does the $(n-1)$-th moment (and therefore, all lower-order moments) about every point.

the zeroth moment of any probability density function is 1, since the area under any probability density function must be equal to one.

