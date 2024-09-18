the natural logarithm of a number is its [[Logarithmic functions|logarithm]] to the [[Base|base]] of the mathematical [[e (constant)|constant]] $e$.

the natural logarithm of $x$ is written as $\ln x$ or equivalently as $\log_{e}(x)$.

it is defined as the [[Integral|integral]], or area under a curve, of a [[Hyperbolic functions|hyperbola]]:

$$
\ln{x}=\int^{x}_{0}=\frac{1}{t}dt
$$
## Properties of natural logarithms

### Product rule:

$$
\ln{xy}=\ln{x}+\ln{y}
$$

proof:

$$
\ln{xy}=\int^{xy}_{1}\frac{1}{t}dt
$$

### Power rule:

$$
\ln{x^r}=r\ln{x}
$$

proof:

$$
\ln{x^r}=\int^{x^r}_{1}\frac{1}{t}dt
$$

### Quotient rule:

$$
\ln{(\frac{x}{y})}=\ln{x}-\ln{y}
$$

or,

$$
\ln{(x\cdot y^{-1})}=\ln{x}+\ln{y^{-1}}
$$

### Chain rule


## Example of trick

$$
\begin{align}
\int{x^{2}\cdot5^{x^{3}+2}}\space dx \\
=\frac{1}{3}\int{5^{u}}\space du \\
u=x^{3}+2 \\
du=3x^{2}dx \\
\frac{du}{3}=x^{2}dx \\
=\frac{5^{x^{3}+2}}{3\ln{5}}+c \\
\end{align}
$$

## Inverse function theorem