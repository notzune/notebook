the joint [[Probability mass function (PMF)|probability mass function]] of two [[Continuous or discrete variable#Discrete variable|discrete]] [[Random variables|random variables]] $X,Y$ is

$$
p_{X,Y}(x,y)=P(X=x\text{ and }Y=y)
$$

or, in terms of [[Conditional probability|conditional]] distributions

$$
p_{X,Y}(x,y)=P(Y=y\mid X=x)\times P(X-x)=P(X=x\mid Y=y)\times P(Y=y)
$$

where $P(Y=y\mid X=x)$ is the [[Probability|probability]] of $Y=y$ given that $X=x$.

the generalization of this is the joint probability distribution of $n$ discrete random variables $X_1,X_2,\dots,X_n$ which is:

$$
P_{X_1,\dots,X_n}(x_1,\dots,x_n)=P(X_1=x_1\text{ and }\dots\text{ and }X_n=x_n)
$$

or equivalently written as:

$$
\begin{align}
P_{X_1,\dots,X_n}(x_1,\dots,x_n)&=P(X_1=x_1)\times P(X_2=x_2\mid X_1=x_1) \\
&\times P(X_3=x_3\mid X_1=x_1,X_2=x_2) \\
\\
&\dots \\
\\
&\times P(X_n=x_n\mid X_1=x_1,X_2=x_2,\dots,X_{n-1}=x_{n-1}) \\
\end{align}
$$