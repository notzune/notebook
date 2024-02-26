in [[Probability theory|probability]] and [[statistics]], a probability mass function is a [[function]] that gives the probability that a [[Continuous or discrete variable|discrete]] [[Random variables|random variable]] is exactly equal to some value. 

sometimes it is also known as the discrete probability density function.

the probability mass function is used in defining a [[Discrete probability distribution|discrete probability distribution]] and such functions exist for either [[scalar]] or multivariate random variables whose [[domain]] is discrete.

# Explanation

formally, it is the function $p:\mathbb{R}\rightarrow[0,1]$ defined by

$$
p_X(x)=P(X=x)
$$

for $-\infty<x<\infty$, where $P$ is a [[Probability measure|probability measure]].   

this equation means that the probability of of the random variable $X$ being *exactly* equal to some value $x$ is given by $p_X(x)$. this function works for all real numbers but is meaningful for the particular values that $X$ can take ([[Sample space|sample space]]).

the rules for a PMF, $p_X$, associated with a discrete random variable $X$ are:

1. the probability for each specific outcome $x_i$, denoted as $p_i$, must be between $0$ and $1$. $0\leq p_i\leq1$
2. the sum of the probabilities for all possible [[Outcome|outcomes]] must equal 1. $\sum_i p_i=1$.

# Examples

consider a [[Fair|fair]] six-sided [[Dice (die)|die]]. the random variable $X$ can be the result of a die roll, so $X$ can take on any value from 1 to 6; each outcome is equally likely so each has a probability of $1/6$.

the PMF of the die roll, $p_X(x)$ can be described as:

$$
\begin{align}
&p_X(1)&=P(X=1)&=\frac{1}{6} \\
\\
&p_X(2)&=P(X=2)&=\frac{1}{6} \\
\\
&p_X(3)&=P(X=3)&=\frac{1}{6} \\
\\
&p_X(4)&=P(X=4)&=\frac{1}{6} \\
\\
&p_X(5)&=P(X=5)&=\frac{1}{6} \\
\\
&p_X(6)&=P(X=6)&=\frac{1}{6} \\
\\
\end{align}
$$

these probabilities adhere to the rules of a PMF: each $p_i$ is between $0$ and $1$ and the sum of all $p_i$'s equals to 1.

another example, we now have ***TWO*** (2) dice and we want to know the sum of the two numbers (i.e., you roll a 6 and a 2 so the sum of the two die would be 8) and we want to calculate the probabilities for the possible outcomes.

we will assign the random variable $Y$ to represent the two dice so that $Y$ can take on the values from 2 (1+1) to 12 (6+6).

the [[Sample space|sample space]] of $Y$ (the [[Sets|set]] of all possible outcomes for the two dice) consists of $36$ [[Element|elements]] (since there are 6 possible outcomes for the first die multiplied by 6 possible outcomes from the second one). visually this would look something like this:

$$
S_Y=\{(1,1),(1,2),(1,3),\dots,(6,6)\}
$$

the outcomes of the rolls are all equally likely ($1/6$) as we saw in the prior example but the sums are not, for example there are a lot more ways to roll a 7 than there are a 2.

to find the PMF, $p_Y(y)$, we need to count how many outcomes correspond to each possible sum, then divide by the total number of outcomes (36).

the sums and their corresponding probabilities: 

- sum = 2: can only occur if both dice show a 1. 
	- $P(Y=2)=\frac{1}{36}$
- sum = 3: can only occur if the dice show either $(1,2)\text{ or }(2,1)$. 
	- $P(Y=3)=\frac{2}{36}$
- sum = 4: occurs if the dice show $(1,3),(2,2)\text{ or }(3,1)$. 
	- $P(Y=4)=\frac{3}{36}$
- sum = 5: occurs if the dice show $(1,4),(2,3),(3,2)\text{ or }(4,1)$. 
	- $P(Y=5)=\frac{4}{36}$
- sum = 6: occurs if the dice show $(1,5),(2,4),(3,3),(4,2)\text{ or }(5,1)$. 
	- $P(Y=6)=\frac{5}{36}$
- sum = 7: occurs if the dice show $(1,6),(2,5),(3,4),(4,3),(5,2)\text{ or }(6,1)$. 
	- $P(Y=7)=\frac{6}{36}$
- sum = 8: mirrors sum = 6. 
	- $P(Y=8)=\frac{5}{36}$
- sum = 9: mirrors sum = 5. 
	- $P(Y=9)=\frac{4}{36}$
- sum = 10: mirrors sum = 4. 
	- $P(Y=10)=\frac{3}{36}$
- sum = 11: mirrors sum = 3. 
	- $P(Y=11)=\frac{2}{36}$
- sum = 12: mirrors sum = 1. 
	- $P(Y=12)=\frac{1}{36}$
now let's put these probabilities in the formula:

$$
p_Y(y) = 
\begin{cases} 
\frac{1}{36} & \text{for } y=2 \\

\frac{2}{36} & \text{for } y=3 \\
\frac{3}{36} & \text{for } y=4 \\
\frac{4}{36} & \text{for } y=5 \\
\frac{5}{36} & \text{for } y=6 \\
\frac{6}{36} & \text{for } y=7 \\
\frac{5}{36} & \text{for } y=8 \\
\frac{4}{36} & \text{for } y=9 \\
\frac{3}{36} & \text{for } y=10 \\
\frac{2}{36} & \text{for } y=11 \\
\frac{1}{36} & \text{for } y=12 \\
0 & \text{otherwise}
\end{cases}
$$

this PMF, $p_Y(y)$, tells us the probability of each possible sum $y$ when two six-sided dice are rolled. notice that the probabilities sum to 1, as required by the rules of a PMF. 

the [[Shape of the distribution|shape]] of the distribution is triangular and symmetric because there are more ways to roll numbers in the middle of the range (like 6, 7, or 8) than numbers at the ends (like 2 or 12).