an integral represents the accumulation of quantities, such as [[Area|areas]] under [[Curve|curves]], total distance traveled, or the [[Mass|mass]] of an object with varying [[Density|density]]. it's a fundamental concept in [[Calculus|calculus]], used to find many things, including [[Area|areas]], volumes, central points, among others.

there are mainly two types of integrals: indefinite and definite integrals.

# Indefinite integral

is the [[Antiderivative|antiderivative]] of a [[Function|function]], represented as:

$$
\int f(x)\,dx
$$

it gives a family of functions $F(x)+C$ where $C$ is the constant of integration. this form of integration does not specify limits and is used to find the general form of the original function given its rate of change.

# Definite integral

calculates the accumulation of quantities on a specific interval $[a,b]$, represented as:

$$
\int^{b}_{a}f(x)\,dx
$$

this form provides a specific numerical value and is used to calculate areas, volumes, and total changes.

# Example

consider the function $f(x)=x^{2}$. to find the area under the curve from $x=1$ to $x=3$, we would use the definite integral.

to find the indefinite integral of 

$$
f(x):\int x^{2}\,dx=\frac{x^{3}}{3}+C
$$
    
apply the limits for the definite integral (3 and 1):

$$
\begin{align}
\int^{3}_{1}x^{2}\,dx&=\left[\frac{x^{3}}{3}\right]^{3}_{1} \\
\\
&=\frac{3^{3}}{3}-\frac{1^{3}}{3} \\
\\
&=\frac{27}{3}-\frac{1}{3} \\
\\
&=9-\frac{1}{3}=8\frac{2}{3}
\end{align}
$$

this result, $8\frac{2}{3}$, represents the total area under the curve of $f(x)=x^{2}$ from $x=1$ to $x=3$.

if the function was something like $f(x)=4x-x^{2}$ from $x=0$ to $x=4$, we would calculate the area under the curve for the interval $[0,4]$ by first finding the indefinite integral of $f(x)$: 

$$
\int(4x-x^{2})\,dx=2x^{2}-\frac{x^3}{3}+C
$$

apply the limits for the definite integral ($0$ and $4$):

$$
\begin{align*}
\int_{0}^{4}(4x-x^2)\,dx&=\left[2x^{2}-\frac{x^3}{3}\right]_{0}^{4} \\
\\
&= \left(2(4)^{2}-\frac{(4)^3}{3}\right)-\left(2(0)^{2}-\frac{(0)^3}{3}\right) \\
\\
&=\left(2\cdot16-\frac{64}{3}\right)-(0) \\
\\
&=32-\frac{64}{3} \\
\\
&=\frac{96-64}{3} \\
\\
&=\frac{32}{3}
\end{align*}
$$

this result, $\frac{32}{3}$, represents the total area under the curve of $f(x) = 4x - x^{3}$ from $x=0$ to $x=4$.