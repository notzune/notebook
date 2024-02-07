in [[Probability theory|probability theory]], a provability density function (PDF), density function, or density of an absolutely continuous random variable, is a function whose value at any given sample (or point) in the [[Sample space|sample space]] can be interpreted as providing a [[Relative likelihood|relative likelihood]] that the value of the random variable would be equal to the sample.

although the absolute likelihood for a continuous random variable to take on any particular value is 0 (since there is an infinite set of possible values to begin with), the value of the PDF at two different samples can be used to infer, in any particular draw, how much more likely it is that the random variable would be closer to one sample compared to the other.

in other words, the PDF is used to specify the probability of the random variable falling within a particular range of values, as opposed to taking on any one value. 

this probability is given by the [[Integration|integral]] of this variable's PDF over that range—that is, it is given by the area under the density function but above the horizontal axis and between the lowest and greatest values of the range.

$$
P(a\leq X\leq b)=\int^{b}_{a}f(x)\,dx
$$

the probability density function is nonnegative everywhere, and the area under the entire curve is equal to 1.

$$
\int_\text{state space}f(x)\,dx=1
$$

the probability that a [[Continuous or discrete variable|continuous]] [[Random variables|random variable]] $X$ takes any specific value $a$ is always $0$.

# Example
![[Screenshot 2024-02-07 at 11.39.55 AM.png]]
suppose that a metal cylinder is manufactured to have a $50$ mm diameter with a tolerance of $\pm0.5$ mm, the PDF would be written as: 

$$
f(x)=1.5-6(x-50.0)^{2}
$$

for $49.5\leq x\leq50.5$ and $f(x)=0$ elsewhere (as shown by the figure). this is a valid probability density function because it is positive within the state space $[49.5,50.5]$ and because

$$
\begin{align}
\int^{50.5}_{49.5}(1.5-6(x-50.0)^{x})\,dx&=[1.5x-2(x-50.0)^{3}]^{50.5}_{49.5} \\
&=[1.5\times50.5-2(50.5-50.0)^{3}]-[1.5\times49.5-2(49.5-50.0)^{3}] \\
&=75.5-74.5 \\
\\
&=1.0 \\
\end{align}
$$

then if we want to find the probability that the metal cylinder has a diameter between $49.8$ and $50.1$ mm, we can calculate it like so:

$$
\begin{align}
\int^{50.5}_{49.5}(1.5-6(x-50.0)^{x})\,dx&=[1.5x-2(x-50.0)^{3}]^{50.1}_{49.8} \\
&=[1.5\times50.1-2(50.1-50.0)^{3}]-[1.5\times49.8-2(49.8-50.0)^{3}] \\
&=75.148-74.716 \\
\\
&=0.432 \\
\end{align}
$$
