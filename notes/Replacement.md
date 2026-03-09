in [[Probability theory|probability theory]], replacement effects the [[Probability|probabilities]] of [[Outcome|outcomes]] from a [[Sample space|sample space]].

with replacement means there is repetition as an outcome has a chance of happening more than once and all outcomes have a constant equal probability of happening. 

the draws in probability with replacement are [[Independent events|independent events]] since one event's outcome does not affect the probability of the other event(s).

say you have a box with 2 blue balls and 3 orange balls

here are the probabilities of picking each color ball with replacement.

$$
\text{Probabilities}
\begin{cases}
\text{blue}=\frac{2}{5}=40\% \\
\text{orange}=\frac{3}{5}=60\% \\
\end{cases}
$$

![[Screenshot 2024-01-23 at 8.55.54 PM.png]]

without replacement means there is no repetition as the outcome is then removed from the sample space once it is "drawn" and it increases the probability of the other outcomes since there is a smaller sample size.

back to the earlier example with 2 blue balls and 3 oranges ones, if its now done without replacement then the sample size will get smaller each draw and the probabilities will change each time

![[Screenshot 2024-01-23 at 8.56.03 PM 1.png]]

so in this example, assuming we still start out with the 2 blues and 3 oranges and we draw an orange ball on the first trial, we are left with 2 blues and 2 oranges which changes the probabilities of the outcomes as seen below for each hypothetical trial:

$$
\begin{align}
&\text{Draw \#1}
\begin{cases}
\text{blue}=\frac{2}{5}=40\% \\
\text{orange}=\frac{3}{5}=60\% \\
\end{cases} \\
\\
&\text{Draw \#2}
\begin{cases}
\text{blue}=\frac{2}{4}=50\% \\
\text{orange}=\frac{2}{4}=50\% \\
\end{cases} \\
\\
&\text{Draw \#3}
\begin{cases}
\text{blue}=\frac{1}{3}=33.33\% \\
\text{orange}=\frac{2}{3}=66.67\% \\
\end{cases} \\
\\
&\text{Draw \#3}
\begin{cases}
\text{blue}=\frac{0}{2}=0\% \\
\text{orange}=\frac{2}{2}=100\% \\
\end{cases} \\
\end{align}
$$
