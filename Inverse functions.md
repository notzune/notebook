the inverse function of a [[Function|function]] $f$ (also referred to as the inverse of $f$) is a function that undoes the [[Operation|operation]] of $f$. the inverse of $f$ exists if and only if $f$ is [[Bijection|bijective]] and is denoted by $f^{-1}$.

for a function $f:X\rightarrow Y$, its inverse $f^{-1}:Y\rightarrow X$ asserts an explicit description: it maps each element $y\in Y$ to the unique element $x\in X$ such that $f(x)=y$.

for example, lets take the function:

$$
f(x)=5x-7
$$

you can think of $f$ as the function which multiplies its input by 5 then subtracts 7 from the resulting number.

to undo this, one adds 7 to the input then divides the result by 5; therefore the inverse of $f$ in this example is the function $f^{-1}:\mathbb{R}\rightarrow\mathbb{R}$ defined by

$$
f^{-1}(y)=\frac{y+7}{5}
$$

## Definitions

let $f$ be a function whose [[Domain|domain]] is the [[Sets|set]] $X$, and whose [[Codomain|codomain]] is the set $Y$. then $f$ is invertible if there exists a function $g$ from $Y$ to $X$ such that: 

$$
g(f(x))=x\space\forall x\in X\space\wedge f(g(y))=y\space\forall y\in Y
$$

if $f$ is invertible then there is exactly one function $g$ satisfying this property. the function $g$ is called the inverse of $f$ and is denoted as $f^{-1}$.

the function $f$ is invertible if and only if it is bijective, this is because the condition:

$$
g(f(x))=x\space\forall x\in X
$$

implies that 