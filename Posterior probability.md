a type of [[Conditional probability|conditional probability]] that results from [[Bayesian inference|updating]] the [[Prior probability distribution|prior probability]] with information summarized by the [[Likelihood function|likelihood]] when applying [[Baye's theorem|Baye's rule]].

the posterior probability contains everything there is to know about an uncertain proposition.

for example, how would we use the probabilities $P(A_i)$ and $P(B\mid A_i)$ to calculate the probabilities $P(A_i|B)$ which are the new, revised, probabilities of events $A_i$ conditional on event $B$.

# Example

imagine a school where 60% (0.6) of all students are boys (not girls) and the [[Complement (probability)|remaining]] 40% (0.4) are girls.

the school dress code states that girls can either wear pants or skirts, while boys must wear pants.

an observer sees a (random) student and for the sake of argument all they saw was that the student was wearing pants but the observer does not know if the student is a girl or boy.

the question is now what is the probability that the student is a girl? $P(G)$

the [[Events|event]] $G$ is that the student is a girl, and the event $T$ is that the student is wearing pants (trousers).

now to calculate the posterior probability $P(G\mid T)$, we first need to know

- $P(G)$, the probability that the student is a girl regardless of any other information. we know that this probability is 0.4 since 40% of students are girls.
- $P(B)$, the probability that the student is not a girl regardless of any other information which we know this to be the complement of event $G$, and it was also given to us as 0.6 (or 60%)
- $P(T\mid G)$, the probability that the student is wearing pants [[Conditional probability|if]] the student is a girl. since they can either wear pants or skirts, this is 0.5
- $P(T\mid B)$, the probability a student is wearing pants if the student is not a girl. this is given as 1 since all students who aren't girls wear pants.
- $P(T)$, the probability that a randomly selected student is wearing pants regardless of any other information.

to solve for $P(T)$, we can use the [[Law of total probability|law of total probability]]:

$$
P(T)=P(T\mid G)\space P(G)+P(T\mid B)\space P(B)
$$

which is,

$$
P(T)=0.5\times0.4+1\times0.6=0.8
$$

given all this information, the posterior probability of the observer having spotted a girl given that the observed student is wearing pants can be calculated by substituting these values in the formula:

$$
P(G\mid T)=\frac{P(T\mid G)\space P(G)}{P(T)}=\frac{0.5\times0.4}{0.8}=0.25
$$

intuitively you can just solve this using simple algebra, given that the school has $N$ number of students, non girls would be $=0.6N$, girls would be  $=0.4N$.

total number of pants wearers $=0.6N+50\%\text{ of } 0.4N$, and number of girls wearing pants would be just $50\%\text{ of } 0.4N$.

therefore, in the population of pants enthusiasts, girls are $=(50\%\text{ of }0.4N)/(0.6N+50\%\text{ of }0.4N)=25\%$, rewritten for clarity this is:

$$
\begin{align}
\text{\% girls wearing pants}&=\frac{\text{girls wearing pants}}{\text{total population of pant wearers}} \\
\\
&=\frac{0.5(0.4N)}{0.6N+(0.5(0.4N))} \\
\\
&=\frac{0.2N}{0.6N+0.2N} \\
\\
&=\frac{0.2}{0.8}=\frac{1}{4}=25\%
\end{align}
$$

you can solve any [[Baye's theorem]] problem like this.