integration is a key concept in [[Calculus|calculus]] that allows us to find the [[Integral|integral]] which defines quantities like [[Area|areas]] under a [[Curve|curve]], [[Volume|volume]], and other accumulations.

there are certain rules and steps for integrating functions:

# Rules for integration

## Power rule

for any real number $n\neq-1$.

$$
\int x^{n}\,dx=\frac{x^{n+1}}{n+1}+C
$$

## Sum rule

the integral of a sum of functions is the sum of their integrals

$$
\int(f(x)+g(x))\,dx=\int f(x)\,dx+\int g(x)\,dx
$$

## Difference rule

the integral of a difference of functions is the difference of their integrals

$$
\int(f(x)-g(x))\,dx=\int f(x)\,dx-\int g(x)\,dx
$$

## Constant multiple rule

a constant can be factored out of an integral

$$
\int cf(x)\,dx=c\int f(x)\,dx
$$

## [[Integration by parts]]

useful for products of functions

$$
\int u\,dv=uv-\int v\,du
$$

## Substitution rule

for making integration easier by changing variables,

$$
\int f(g(x))g'(x)\,dx=\int f(u)\,du
$$

where $u=g(x)$ and $du=g'(x)\,dx$.

# Constant of integration 

in the context of integration, $C$ represents the constant of integration. 

when you integrate a [[Function|function]] to find its antiderivative, the constant $C$ is added to account for the fact that there are infinitely many antiderivatives for any given function. 

this is because when you differentiate a constant, the result is $0$, which means adding or subtracting a constant from a function does not change its [[Derivative|derivative]].

for example, if the derivative of $F(x)$ is $f(x)$, then the derivative of $F(x) + C$ is also $f(x)$, for any real number value of $C$. 

when performing indefinite integration, we include $+\,C$ in the answer to indicate that there are multiple possible antiderivatives, differing only by a constant value.

in the case of definite integration, where you integrate over a specific interval from $a$ to $b$, the constant $C$ cancels out when calculating the difference between the upper and lower bounds of the integral, so it is not included in the final answer.

## Calculating the constant

the value of $C$ cannot be determined the from the process of indefinite integration alone. its value depends on additional information or conditions provided for the function. 

specifically, $C$ is determined by an initial condition or boundary condition that the function must satisfy. this is often presented as a point $(x_0, y_0)$ through which the function passes.

for example, if you have an integral resulting in 

$$
F(x)=\int f(x)\,dx=G(x)+C
$$

and you know that the function $F(x)$ passes through the point $(x_0, y_0)$, you can substitute $x_0$ into $G(x)$ and set it equal to $y_0$ to solve for $C$:

### Example

given $F(X)=\int f(x)\,dx=x^{2}+C$ and the condition that $F(1)=5$, we can find $C$ as follows:

first substitute the known point into the function:

$$
F(1)=1^{2}+C=5
$$

then solve for $C$:

$$
1+C=5\implies C=4
$$

so in this case $C=4$ and the [[Antiderivative|antiderivative]] $F(x)=x^{2}+4$ satisfies the given condition.
