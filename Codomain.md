a codomain or set of destination of a [[Function|function]] is a set into which all of the output of the function is constrained to fall. 

it is the set $Y$ in the notation $f : X\rightarrow Y$. the term [[Range|range]] is sometimes ambiguously used to refer to either the codomain or the [[Image|image]] of a function.

a codomain is part of a function $f$ if $f$ is defined as a triple $(X,Y,G)$ where $X$ is called the [[Domain|domain]] of $f$, $Y$ its codomain, and $G$ its graph.

the set of all elements of the form $f(x)$ where $x$ ranges over the elements of the domain $X$, is called the [[Image||image]] of $f$.

the [[Image|image]] of a function is a [[Subset|subset]] of its codomain so it might not coincide with it. namely, a function that is not [[Surjective functions|surjective]] has elements $y$ in its codomain for which the equation $f(x)=y$ does not have a solution.

## Examples

for a function:

$$
f:\mathbb{R}\rightarrow\mathbb{R}
$$

defined by

$$
f:x\mapsto x^{2},\text{ or equivalently }f(x)=x^{2}
$$

the codomain of $f$ is $\mathbb{R}$, but %f% does not map to any negative number. thus the image of $f$ is the set $\mathbb{R}_{0}^{+}$; i.e. the interval $[0,\infty)$.

an alternative function $g$ is defined thus:

$$
\begin{align}
g:\mathbb{R}\rightarrow\mathbb{R}_{0}^{+} \\
\\
g:x\mapsto x^{2} \\
\end{align}
$$
while $f$ and $g$ map a given $x$ to the same number, they are not the same function because they have different codomains. a third function $h$ can be defined to demonstrate why:

$$
h:x\mapsto \sqrt{x}
$$

the domain of $h$ cannot be $\mathbb{R}$ but can be defined to be $\mathbb{R}_{0}^{+}$.

$$
h:\mathbb{R}_{0}^{+}\rightarrow\mathbb{R}
$$

the [[Function composition|compositions]] are denoted 

$$
\begin{align}
h\circ f, \\
\\
h\circ g. \\
\end{align}
$$

$h\circ f$ is not useful, it is true, unless defined otherwise that the image of $f$ is not known; its only known that it is a subset of $\mathbb{R}$. its possible that $h$, when composed with $f$, might receive an [[Argument of a function|argument]] for which no output is defined - negative numbers are not elements of the domain of $h$, which is the [[Square root|square root function]].
