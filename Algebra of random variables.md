a [[Linear|linear]] [[Function|function]] of a [[Random variables|random variable]] $X$ is another random variable

$$
Y=aX+b
$$

for some numbers $a,b\in\mathbb{R}$, it is a general result that 

$$
E(Y)=aE(X)+b
$$

so that the [[Expected value|expectation]] of the random variable $Y$ is just the same linear function of the expectation of the random variable $X$, however for the [[Variance|variance]],

$$
\text{Var}(Y)=a^{2}\text{Var}(X)
$$

and the [[Standard deviation|standard deviation]] of $Y$, $\sigma_{Y}$, is given by

$$
\sigma_{Y}=|a|\sigma_{X}
$$

where $\sigma_X$ is the standard deviation of $X$. note that the "shift" amount ($b$) does not influence the variance of $Y$ and that the "scale" amount ($a$) is *squared* in the relationship between the two variances.

# Elementary algebra of random variables

considering two random variables $X$ and $Y$, the following [[Operation|operations]] are possible:

- addition: $Z=X+Y=Y+X$
- subtraction: $Z=X-Y=-Y+X$
- multiplication: $Z=XY=YX$
- division: $Z=X/Y=X\cdot(1/Y)=(1/Y)\cdot X$
- exponentiation: $Z=X^{Y}=e^{Y\ln(X)}$

in all cases, the variable $Z$ resulting from each operation is also a random variable. all [[Commutative property|commutative]] and [[Associative property|associative]] properties of conventional algebraic operations are also valid for random variables.

if any of the random variables is replaced by a deterministic variable or by a constant, all the previous properties still remain valid.

# Expectation algebra for random variables

the following [[Expected value|expected value]] $E$ of the random variables $Z$ resulting from an algebraic operation between to random variables can be calculated using the following set of rules:

- addition: $E(Z)=E(X+Y)=E(X)+E(Y)=E(Y)+E(X)$
- subtraction: $E(Z)=E(X-Y)=E(X)-E(Y)=-E(Y)+E(X)$
- multiplication: $E(Z)=E(XY)=E(YX)$,
	- if $X$ and $Y$ are [[Independence|independent]] from each other, then: $E(XY)=E(X)\cdot E(Y)=E(Y)\cdot E(X)$
- division: $E(Z)=E(X/Y)=E(X\cdot(1/Y))=E((1/Y)/cdot X))$,
	- if $X$ and $Y$ are independent from each other, then: $E(X/Y)=E(X)\cdot E(1/Y)=E(1/Y)\cdot E(X)$
- exponentiation: $E(Z)=E(X^{Y})=E(e^{Y\ln(X)})$

if any of the variables is replaced by a deterministic variable or by a constant ($k$), the previous properties remain valid when considering that $P(X=k)=1$ and, therefore, $E(X)=k$.

if $Z$ is defined as a general non-linear algebraic function $f$ of a random variable $X$, then:

$$
E(Z)=E(f(X))\neq f(E(X))
$$

# Variance algebra for random variables

- addition: $\text{Var}(Z)=\text{Var}(X+Y)=\text{Var}(X)+2\text{Cov}(X,Y)+\text{Var}(Y)$
	- if $X$ and $Y$ are independent, then: $\text{Var}(X+Y)=\text{Var}(X)+\text{Var}(Y)$
- subtraction: $\text{Var}(Z)=\text{Var}(X-Y)=\text{Var}(X)-2\text{Cov}(X,Y)+\text{Var}(Y)$
	- if $X$ and $Y$ are independent, then: $\text{Var}(X-Y)=\text{Var}(X)+\text{Var}(Y)$[^1]
- multiplication: $\text{Var}(Z)=\text{Var}(XY)=\text{Var}(YX)$
	- if $X$ and $Y$ are independent from each other then: $\text{Var}(XY)=E(X^{2})\cdot E(Y^{2})-(E(X)\cdot E(Y))^{2}=\text{Var}(X)\cdot \text{Var}(Y)+\text{Var}(X)\cdot(E(Y))^{2}+\text{Var}(Y)\cdot(E(X))^{2}$
- division: 

[^1]: for independent random variables, the variance is the same for additions and subtractions: $\text{Var}(X+Y)=\text{Var}(X-Y)=\text{Var}(Y-X)=\text{Var}(-X-Y)$