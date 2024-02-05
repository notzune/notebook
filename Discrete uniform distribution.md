in [[Probability theory|probability theory]] and [[Statistics|stats]], the discrete uniform distribution is a [[Symmetric probability distribution|symmetric]] [[Probability distribution|probability distribution]] where a finite number of values are equally likely to be observed; every one of $n$ values has equal probability $1/n$. 

the discrete uniform distribution itself is by definition non-parametric. it's easier to just represent its values generally by all integers in an interval $[a,b]$ so that $a$ and $b$ become the main parameters of the distribution, usually the interval would just be $[1,n]$ with the single parameter $n$ being of any importance. 

the [[Cumulative distribution function (CDF)|CDF]] of this distribution then can be expressed for any $k\in[a,b]$ as

$$
F(k;a,b)=\frac{|k|-a+1}{b-a+1}
$$