in mathematics, a piecewise function is a [[Function|function]] defined by multiple sub-functions, where each sub-function applies to a different [[Interval|interval]] of the [[Domain|domain]].

# Examples

## Absolute value

consider the piecewise definition of the [[Absolute value|absolute value]] function:

$$
|x|=
\begin{cases} 
-x & \text{if } x < 0 \\
x & \text{if } x \geq 0 \\
\end{cases}
$$
## [[Piecewise linear function]]

another example would be the plot of this piecewise linear function:
![[Screenshot 2024-02-13 at 5.00.18 PM.png]]
$$
f(x)=
\begin{cases} 
-3-x&\text{if }x\leq-3 \\ 
x+3&\text{if }-3<x\leq0 \\ 
3-2x&\text{if }0<x\leq3 \\ 
0.5x-4.5&\text{if }x>3 \\
\end{cases}
$$

## [[Integration|Integration]] of piecewise functions

[[Hayter 2.2.3|here]] is another example of a piecewise function and it's plot:
![[Screenshot 2024-02-13 at 6.50.55 PM.png]]
from the original [[Probability and Statistics (index)|probability]] question, we have the [[Probability density function (PDF)|PDF]] as:

$$
f(x)=
\begin{cases}
\frac{15}{64}+\frac{x}{64},&\text{for }-2\leq x\leq0 \\
\\
\frac{3}{8}+cx,&\text{for }0\leq x\leq3 \\
\\
0&\text{everywhere else}
\end{cases}
$$

and are asked to find the value of $c$. since this is a probability question [[Hayter 2.2.3#^55621e|we know that the total range has to be 1]], and we can therefore integrate the separate functions over that range:


$$
\int^{0}_{-2}\left(\frac{15}{64}+ \frac{x}{64}\right)\,dx+\int^{3}_{0}\left(\frac{3}{8}+cx\right)\,dx=1
$$

the first integral then becomes:

$$
\int^{0}_{-2}\left(\frac{15}{64}+\frac{x}{64}\right)\,dx=\left[\frac{15x}{64}+\frac{x^{2}}{128}\right]^{0}_{-2}
$$

evaluating this from $-2$ to $0$, we get:

$$
\begin{align}
&\left[\frac{15(0)}{64}+\frac{(0)^{2}}{128}\right]-\left[\frac{15(-2)}{64}+\frac{(-2)^{2}}{128}\right] \\
\\
&=0-\left(-\frac{30}{64}+\frac{4}{128}\right) \\
&=\frac{30}{64}-\frac{4}{128} \\
\\
&=\frac{7}{16} \\
\end{align}
$$

now for the second integral:

$$
\int^{3}_{0}\left(\frac{3}{8}+cx\right)\,dx=\left[\frac{3x}{8}+\frac{cx^{2}}{2}\right]^{3}_{0}
$$

evaluating this from $0$ to $3$, we get:

$$
\begin{align}
&\left[\frac{3(3)}{8}+\frac{c(3)^{2}}{2}\right]-\left[\frac{3(0)}{8}+\frac{c(0)^{2}}{2}\right] \\
\\
&=\frac{9}{8}+\frac{9c}{2} \\
\end{align}
$$

given that the sum of these integrals equals 1, we can now solve for $c$:

$$
\begin{align}
\frac{7}{16}+\frac{9}{8}+\frac{9c}{2}&=1 \\
\\
\frac{7}{16}+\frac{18}{16}+\frac{9c}{2}&=1 \\
\\
\frac{25}{16}+\frac{9c}{2}&=1 \\
\\
\frac{9c}{2}&=-\frac{9}{16} \\
\\
9c&=-\frac{9}{8} \\
\\
c&=-\frac{1}{8} \\
\\
c&=-0.125
\end{align}
$$

plugging this back into the piecewise function, we get:

$$
f(x)=
\begin{cases}
\frac{15}{64}+\frac{x}{64},&\text{for }-2\leq x\leq0 \\
\\
\frac{3}{8}+0.125x,&\text{for }0\leq x\leq3 \\
\\
0&\text{everywhere else}
\end{cases}
$$