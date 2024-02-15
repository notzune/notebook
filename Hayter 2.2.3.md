this problem is an example of normalizing a [[Probability density function (PDF)|PDF]] when it is given as a [[Piecewise|piecewise function]] and the given range is not equal to 1[^1].

the problem says: a [[Random variables|random variable]] $X$ takes values between $-2$ and $3$ with a probability density function:

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

# Finding the missing variable $c$ and plotting the PDF

it first asks us to find the value of $c$, and then sketch the PDF:

to find the value of $c$ we must [[Integration|integrate]] $f(x)$ over its entire range to find $c$:

$$
\int^{0}_{-2}\left(\frac{15}{64}+ \frac{x}{64}\right)\,dx+\int^{3}_{0}\left(\frac{3}{8}+cx\right)\,dx=1
$$

here we set it equal to $1$ since that is the desired [[Range|range]] (because it has to represent the total probability of all outcomes, which is out of 1) ^55621e

the first integral:

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

which we can then plot:

| $x$ | $f(x)$ |
| ---- | ---- |
| -2 | 0.203125 |
| -1 | 0.21875 |
| 0 | 0.234375 |
| 1 | 0.36923077 |
| 2 | 0.36363636 |
| 3 | 0.35820896 |
![[Screenshot 2024-02-13 at 6.50.55 PM.png]]
# Finding the probability of $P(-1\leq X\leq1)$

to answer the second part of the problem, we are asked to find $P(-1\leq X\leq1)$ which we can find through integration of $f(x)$ from $-1$ to $1$. however since the function changes at $x=0$, we will need to split the integration at that point:

$$
P(-1\leq X\leq1)=\int^{0}_{-1}\left(\frac{15}{64}+\frac{x}{64}\right)\,dx+\int^{1}_{0}\left(\frac{3}{8}+0.125x\right)\,dx
$$

evaluating the first integral:

$$
\begin{align}
&\int^{0}_{-1}\left(\frac{15}{64}+\frac{x}{64}\right)\,dx=\left[\frac{15x}{64}+\frac{x^{2}}{128}\right]^{0}_{-1} \\
\\
&=\left[\frac{15(0)}{64}+\frac{(0)^{2}}{128}\right]-\left[\frac{15(-1)}{64}+\frac{(-1)^{2}}{128}\right] \\
\\
&=0-\left(-\frac{15}{64}+\frac{1}{128}\right) \\
&=\frac{15}{64}-\frac{1}{128} \\
&=\frac{29}{128} \\
\\
&=0.2265625
\end{align}
$$

evaluating the second integral:

$$
\begin{align}
&\int^{1}_{0}\left(\frac{3}{8}+0.125x\right)\,dx=\left[\frac{3x}{8}+\frac{0.125x^{2}}{2}\right]^{1}_{0} \\
\\
&=\left[\frac{3(0)}{8}+\frac{0.125(0)^{2}}{2}\right]-\left[\frac{3(1)}{8}+\frac{0.125(1)^{2}}{2}\right] \\
\\
&=0-\left(\frac{3}{8}+\frac{0.125}{2}\right) \\
&=0.375+0.0625 \\
\\
&=0.4375 \\
\end{align}
$$

and then adding them together:

$$
\begin{align}
P(-1\leq X\leq1)&=\int^{0}_{-1}\left(\frac{15}{64}+\frac{x}{64}\right)\,dx+\int^{1}_{0}\left(\frac{3}{8}+0.125x\right)\,dx \\
\\
&=0.2265625+0.4375 \\
\\
P(-1\leq X\leq1)&=0.6640625
\end{align}
$$

# Finding and sketching the CDF

for the last step it asks us to construct and sketch the [[Cumulative distribution function (CDF)|CDF]]. 

... and this is where i got stuck, ill try this another time[^2]

to find the CDF, we take the integral of the PDF:

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

for the first interval ($-2\leq x\leq0$), we integrate the function $\frac{15}{64}+\frac{x}{64}$ from $-2$ to $x$.

$$
F(x)=\int\left(\frac{15}{64}+\frac{x}{64}\right)\,dx=\frac{15x}{64}+\frac{x^{2}}{128}
$$

to find the [[Integration#Calculating the constant|constant of integration]] we can plug in $-2$ since we know that outside of this interval $[-2,3]$, the PDF is 0.

$$
\begin{align}
F(-2)&=\frac{15(-2)}{64}+\frac{(-2)^{2}}{128}+C \\
\\
0&=\frac{-30}{64}+\frac{4}{128}+C \\
\\
&=-0.46875+0.03125+C \\
&=-0.4375+C \\
\\
0.4375&=C
\end{align}
$$

making the CDF for $-2\leq x\leq0$:

$$
F(x)=0.0078125x^{2}+0.234375x+0.4375
$$

we do the same for the second part, the interval from $0$ to $3$:

$$
F(x)=\int\left(\frac{3}{8}+0.125x\right)\,dx=\frac{3x}{8}+\frac{x^{2}}{16}
$$

which gives us the general form of:

$$
F(x)=0.0625x^{2}+0.375x+C
$$

for the constant, $c$, we need to find the cumulative probability up to $x=0$ by plugging in $0$ to the first part of the function[^3]

$$
F(0)=0.0078125(0)^{2}+0.234375(0)+0.4375
$$

which gives us $0.4375$ which we can plug in for $c$:

$$
F(x)=0.0625x^{2}+0.375x+0.4375
$$

this gives us the complete CDF $F(x)$ over the entire range $-2\leq x\leq3$:

$$
F(x)=
\begin{cases}
0,&\text{for }x<-2 \\
\\
0.0078125x^{2}+0.234375x+0.4375,&\text{for }-2\leq x\leq0 \\
\\
0.0625x^{2}+0.375x+0.4375,&\text{for }0< x\leq3 \\
\\
1,&\text{for }x>3 \\
\end{cases}
$$

which we can then plot:

|$x$ |$F(x)$ |
|---|---|
|$−2$ |$0.0$ |
|$−1$ |$0.2109375$ |
|$0$ |$0.4375$ |
|1|$0.875$ |
|$2$ |$1.4375$ |
|$3$ |$2.125$
![[Screenshot 2024-02-15 at 6.18.27 PM.png]][^4]

[^1]: the total area under the probability density function $f(x)$ over the its entire range must equal 1, because it represents the total probability of all outcomes.
[^2]: timestamp so i can guilt myself later: 2024-02-13 @ 11:11 PM 🕚
[^3]: it is important to note that the "constant" for the second part is ***not*** the same as the constant for the first part since they describe two different things. CDFs need to be continuous so in-order to ensure that the entire piecewise function is continuous we account for the total probability of the first interval since the function describing the second interval is all of the probability values of the first and second interval combined (because it needs to be ***cumulative***).
[^4]: timestamp of when i came back to finish this: 2024-02-15 @ 6:28 PM 🕡