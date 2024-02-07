Blimp is a billionaire. in the last 50 years he has paid taxes only once. chances of being audited in any given year are 1 out of 10 for ordinary residents and 1 out of 100 for billionaires. once you get audited, your chances of going to prison are 1 out of 100 if you have paid taxes that year, and 1 out of 10 if you have not.

the probability $P$ of him paying his taxes $T$ in 2024 based on his record so far is given to us as $P(T)=1/50$, the [[Complement (probability)|complement]] of this event would therefore be $P(\overline{T})=49/50$; the rest is given from the problem:

$$
\begin{align}
&P(T)=\text{chance that Blimp pays taxes}=1/50 \\
&P(\overline{T})=\text{chance that Blimp doesn't pay}=49/50 \\
\\
&P(A)=\text{chance to get audited}
\begin{cases}
P(A_O)=&1/10&\text{ for ordinary people} \\
P(A_B)=&1/100&\text{ for billionaires} \\
\end{cases} 
\\
\\
&P(J)=\text{chance of going to jail}
\begin{cases}
P(J\mid\overline{T})=&1/10&\text{ if you didn't pay taxes that year} \\
P(J\mid T)=&1/100&\text{ if you paid taxes that year} \\
\end{cases} 
\end{align}
$$

the total probability of Blimp going to jail in a year can be calculated by considering both scenarios: paying taxes and not paying taxes, and then getting audited and sent to jail in each case. this is essentially the [[Law of total probability|law of total probability]] applied to this scenario.

the probability of Blimp going to jail in a year when he has paid his taxes can be found by calculating the [[Probabilities of event intersections|probability of the event intersection]] of the events: 

- $T$ - him paying his taxes
- $A_B$ - the probability that he gets audited (as a billionaire)
- $J\mid T$ - (*read: J conditional on T*) the probability of him going to jail if he pays his taxes

this can be computed as:

$$
P(J\mid T)=P(T)\times P(A_B)\times P(J\mid T)
$$

substituting with the given probabilities,

$$
P(J\mid T)=\left(\frac{1}{50}\right)\times\left(\frac{1}{100}\right)\times\left(\frac{1}{100}\right)=\frac{1}{500,000}
$$

similarly, the probability of Blimp going to jail in a year when he has *not* paid his taxes:

1. $\overline{T}$ - him *not* paying his taxes
2. $A_B$ - the probability that he gets audited (as a billionaire)
3. $J\mid\overline{T}$ - the probability that he goes to jail for not paying his taxes

$$
P(J|\overline{T})=P(\overline{T})\times P(A_B)\times P(J\mid\overline{T})
$$

which when computed, 

$$
P(J\mid\overline{T})=\left(\frac{49}{50}\right)\times\left(\frac{1}{100}\right)\times\left(\frac{1}{10}\right)=\frac{49}{50,000}
$$

for the second part of the question, it says if you get elected president $E$, your chance of going to jail becomes $P(J\mid E)=0$. if Blimp has a $1/10$ chance of being elected $P(E)$, we can find the new probability of him going to jail.

first we find the complement of the event of him being elected $E$, which is

$$
P(\overline{E})=1-P(E)=\frac{9}{10}
$$

we already calculated two events where Blimp would go to jail:

- $P(J\mid T)$ - jail if he pays his taxes
- $P(J\mid\overline{T})$ - jail if he doesn't pay taxes

both of these probabilities are now [[Conditional probability|conditional]] on the probability of him getting elected, $P(E)$, since being elected changes the probability of going to jail, $P(J$), to $0$ no matter what.

so then we need to multiply each of these probabilities by the probability of not being elected, $P(\overline{E})$, to adjust for this new condition.

the new total probability of Blimp going to jail, considering the new possibility of him being elected, is

$$
P(J\mid T\cap\overline{E})+P(J\mid\overline{T}\cap\overline{E})
$$

which can be rewritten as

$$
P(\overline{E})\times P(J\mid T)+P(\overline{E})\times P(J\mid\overline{T})
$$

substituting the variables with their respective probabilities:

$$
\left(\frac{9}{10}\right)\times\left(\frac{1}{500,000}\right)+\left(\frac{9}{10}\right)\times\left(\frac{49}{50,000}\right)
$$

which then can be simplified to:

$$
P(J\mid E)=\left(\frac{9}{10}\right)\times\left(\frac{1}{500,000}+\frac{49}{50,000}\right)\approx0.0008838
$$

the third part of the question changes the chance for election to $P(E)=9/10$ (instead of the prior $P(E)=1/10$), which makes the complement, $P(\overline{E})=9/10$ 

so now the probability of him being sent to jail can be calculated as:

$$
P(J\mid E)=\left(\frac{1}{10}\right)\times\left(\frac{1}{500,000}+\frac{49}{50,000}\right)\approx0.0000982
$$

we can check to make sure the answer makes sense by comparing the two probabilities,

$$
0.0000982<0.0008838
$$

which makes sense since there is a higher probability of him being elected now, which means a lower probability of him being sent to jail.