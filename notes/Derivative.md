in [[Calculus|calculus]], a derivative is a tool that quantifies the sensitivity of change of a [[Function|function]]'s output with respect to tis input.

the derivative of a function ($f(x)$) of a single variable at chose input, when it exists ($x=a$), is the [[Slope|slope]] of the [[Tangent|tangent]] line to the graph of the function at that point. 

the tangent line is the best [[Linear approximation|linear approximation of the function near that input value.]] for this reason, the derivative is often called the instantaneous rate of change which is the ratio of the instantaneous change in the dependent variable to the independent variable.

the process of finding a derivative is called [[Differentiation|differentiation]], and there are multiple [[Notation for differentiation|different notations]] for it. (see also: [[Differentiation rules|rules of differentiation]])

## Definition

### As a limit

a [[Function of a real variable|function of a real variable]] $f(x)$ is [[Differentiable functions|differentiable]] at a point $a$ of its [[Domain|domain]] if its domain contains an [[Interval|open interval]] containing $a$, and the following [[Limit|limit]] exists:

$$
L=\lim_{h\rightarrow 0}\frac{f(a+h)-f(a)}{h}
$$

this means that for every positive [[Real numbers|real number]] $\varepsilon$ (even very small), there exists a positive real number $\delta$ such that, for every $h$ such that $|h|<\sigma\text{ and }h\neq0\text{ then }f(a+h)$ is defined, and

$$
\left\vert L-\frac{f(a+h)-f(a)}{h}\right\vert<\varepsilon
$$

where the vertical bars denote [[Absolute value|absolute value]]. this is an example of [[Limit of a function|(ε, δ)-definition of a limit]].

if the function $f$ is differentiable at $a$, that is if the limit $L$ exists, then this limit is called the *derivative* of $f$ at $a$.

if $f$ is a function that has a derivative at every point in its domain, then a function can be define by mapping every point $x$ to the value of the derivative of $f$ at $x$. this function is written $f'$ and is called the *derivative function* or the *derivative of* $f$. 

the function whose value at $a$ equals $f'(a)$ whenever $f'(a)$ is defined and elsewhere is undefined is also called the derivative of $f$. it is still a function, but its domain may be smaller than the domain of $f$.

for example, let $f$ be the squaring function: $f(x)=x^2$, then the quotient in the definition of the derivative is

$$
\frac{f(a_h)-f(a)}{h}=\frac{(a+h)^2-a^2}{h}=\frac{a^2+2ah+h^2-a^2}{h}=2a+h
$$

the division is valid as long as $h\neq0$. the closer $h$ is to 0, the closer this expressions becomes to the value $2a$. 

the limit exists and for every input $a$ the limit is $2a$. so the derivative of the squaring function is the double function: $f'(x)=2x$. 