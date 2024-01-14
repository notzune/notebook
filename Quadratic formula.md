in [[Elementary algenra|elementary algebra]], the quadratic formula is a formula that provides the two solutions, or roots, to a [[Quadratic equation|quadratic equation]]. there are other ways of solving a quadratic instead of usnig the quadratic formula, such as [[Completing the square|completing the square]].

given a general quadratic equation of the form

$$
ax^2+bx+c=0
$$

with $x$ representing an unknown, with $a$, $b$, and $c$ representing constants, and with $a\neq0$, the quadratic formula is:

$$
x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}
$$
where the plus-minus symbol ($\pm$) indicates that the quadratic has two solutions. written separately it becomes:

$$
\begin{align}
&x_1=\frac{-b+\sqrt{b^2-4ac}}{2a} \\
\\ \text{and} \\
\\
&x_2=\frac{-b-\sqrt{b^2-4ac}}{2a} \\
\end{align}
$$

each of these two solutions is also called a [[Zero|root (or zero)]] of the quadratic. geometrically, these roots represent the $x$-values at which *any* [[Parabola|parabola]], explicitly given as $y=ax^2+bx+c$, crosses the $x$-axis.

as well as being a formula that yields the zeros of any parabola, the quadratic formula can also be used to identify the axis of symmetry of the parabola, and the number of [[Real numbers|real]] zeros the quadratic equation contains.

the expression $\Delta=b^2-4ac$ is known as the [[Discriminant|discriminant]]. if $a$, $b$, and $x$ are real numbers and $a\neq 0$ then

$$
\begin{align}
&1.\text{ when }b^2-4ac>0,\text{ there are two distinct real roots to the equation }ax^2+bx+c=0. \\
&2.\text{ when }b^2-4ac=0,\text{ there is one repeated real solution.} \\
&3.\text{ when }b^2-4ac<0,\text{ there are two distinct complex solutions.}
\end{align}
$$

when $b^2-4ac<0$, there are two distinct [[Complex numbers|complex]] solutions, which are also [[Complex conjugate|complex conjugates]] of each other.

## Equivalent formulations

the quadratic formula may also be written as

$$
\begin{align}
&x=-\frac{b}{2a}\pm\sqrt{(\frac{b}{2a})^2-\frac{c}{a}} \\
\\ \text{ or }
\\
&x=\frac{1}{a}(-\frac{b}{2}\pm\sqrt{(\frac{b}{2})^2-ac}).\\
\end{align}
$$

because these formulas allow re-use of intermediately calculated values, these may be easier to use when computing with a calculator or by hand. when the discriminant $b^2-4ac$ is negative, complex roots are involved and the quadratic formula can be written as:

$$
x=-\frac{b}{2a}\pm i\sqrt{\lvert(\frac{b}{2a})^2-\frac{c}{a}\rvert}=\frac{1}{a}(-\frac{b}{2}\pm i\sqrt{|(\frac{b}{2})^2-ac|})
$$

### Muller's method

a lesser known quadratic formula (also named "citardauq") which is used in [[Muller's method]] and which can be found from [[Vieta's formulas]], provides (assuming $a\neq 0,\space c\neq 0$) the same roots via the equation:

$$
x=\frac{-2c}{b\pm\sqrt{b^2-4ac}}=\frac{2c}{-b\mp\sqrt{b^2-4ac}}
$$

for positive $b$, the subtraction causes cancellation in the standard formula (respectively negative $b$ and addition), resulting in poor accuracy so switching to Muller's formula with the opposite is a good workaround.

## Derivations

### [[Completing the square|By completing the square]]

divide the quadratic equation

$$
ax^2+bx+c=0
$$

by $a$, which is allowed because $a$ is non-zero:

$$
x^2+\frac{b}{a}x=-\frac{c}{a}
$$

subtract $\frac{c}{a}$ from both sides of the equation,

$$
x^2+\frac{b}{a}x=-\frac{c}{a}
$$

the quadratic equation is now in a form to which the method of [[Completing the square|completing the square]] is applicable. by adding a constant to both sides of the equation such that the left hand side becomes a complete square, the quadratic becomes:

$$
x^2+\frac{b}{a}x+(\frac{b}{2a})^2=-\frac{c}{a}+(\frac{b}{2a})^2
$$

which produces:

$$
(x+\frac{b}{2a})^2=-\frac{c}{a}+\frac{b^2}{4a^2}
$$

after rearranging the terms on the right side to have a common denominator, we get:

$$
(x+\frac{b}{2a})^2=\frac{b^2-4ac}{4a^2}
$$

the square has thus been completed. if the discriminant $b^2-4ac$ is positive, we can take the [[Square root|square root]] of both sides, getting the following equation:

$$
x+\frac{b}{2a}=\pm\frac{\sqrt{b^2-4ac}}{2a}
$$

(actually the equation remains true even if the discriminant is not positive, by interpreting the root of the discriminant as any of its two opposite complex roots)

in which case, isolating $x$ would give the formula:

$$
x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}
$$

#### Shorter method

1. multiply each side by $4a$,
2. rearrange.
3. add $b^2$ to both sides to complete the square.
4. the left side is the outcome of the polynomial $(2ax+b)^2$.
5. take the square root of both sides.
6. isolate $x$

thus the quadratic is derived as follows:

$$
\begin{align*} 
&ax^2 &+ &\space bx &+ &\space c &= &\space0 \\ 
&4a^2x^2 &+ &\space 4abx &+ &\space4ac &= &\space0 \\ 
&4a^2x^2 &+ &\space 4abx &&&= &-4ac \\ 
&4a^2x^2 &+ &\space 4abx &+ &\space b^2 &=&\space b^2 - 4ac \\ 
&&&(2ax + b)^2 &&&= &\space b^2 - 4ac \\ 
\\
&\text{(valid if $b^2 - 4ac$ is positive)} &&2ax+b &&&= &\pm\sqrt{b^2 - 4ac} \\
\\
&&&2ax &&&= &-b \pm \sqrt{b^2 - 4ac} \\ 
\\
&&&&x &&= &\frac{-b\pm\sqrt{b^2 - 4ac}}{2a}
\end{align*}
$$



