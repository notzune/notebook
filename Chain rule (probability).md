(not to be confused with the [[Chain rule|chain rule]] of [[Calculus|calculus]])

in [[Probability theory|probability theory]], the chain rule (also called the general product rule) describes how to calculate the [[Probability|probability]] of the [[Intersection of events|intersection]] of, not necessarily [[Independence|independent]], [[Events|events]] or the [[Joint probability distribution|joint distribution]] of [[Random variables|random variables]] respectively, using [[Conditional probability|conditional probabilities]].

# Two events

for two events $A$ and $B$, the chain rule states that

$$
P(A\cap B)=P(B\mid A)P(A)
$$

# Finitely many events

for events $A_1,\dots,A_n$ whose intersection has a probability $\neq$ zero, the chain rule states:

$$
\begin{align}
P(A_{1}\cap A_{2}\cap\ldots\cap A_{n})&=P(A_{n}\mid A_{1}\cap \ldots \cap A_{n-1})P (A_{1}\cap \ldots \cap A_{n-1}) \\
\\
&=P (A_{n}\mid A_{1}\cap \ldots \cap A_{n-1})P (A_{n-1}\mid A_{1}\cap \ldots \cap A_{n-2})P(A_{1}\cap\ldots\cap A_{n-2}) \\
\\
&=P (A_{n}\mid A_{1}\cap \ldots \cap A_{n-1})P (A_{n-1}\mid A_{1}\cap \ldots \cap A_{n-2})\cdot \ldots \cdot P (A_{3}\mid A_{1}\cap A_{2})P (A_{2}\mid A_{1})P (A_{1}) \\
\\
&=P (A_{1})P (A_{2}\mid A_{1})P (A_{3}\mid A_{1}\cap A_{2})\cdot \ldots \cdot P (A_{n}\mid A_{1}\cap \dots \cap A_{n-1}) \\
\\
&=\prod _{k=1}^{n}P (A_{k}\mid A_{1}\cap \dots \cap A_{k-1}) \\
\\
&=\prod _{k=1}^{n}P\left(A_{k}\,{\Bigg |}\,\bigcap _{j=1}^{k-1}A_{j}\right)\end{align}
$$
