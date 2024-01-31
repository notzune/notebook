![[Screenshot 2024-01-30 at 11.48.42 PM 1.png]]
this problem is an example of [[Law of total probability|the law of total probability]]. the probability of being pulled over $P(\text{pulled over})$, can occur in two [[Disjoint event|mutually exclusive events]]: either the person was speeding or they were not (they obviously can't be in both states, at least not for sake of argument).

to find the total probability of being pulled over we need to consider both of these events.

the [[Conditional probability|conditional probability]] of being pulled over when speeding, $P(\text{pulled over}\mid\text{speeding})$ can't by added to the probability of someone being pulled over when not speeding, $P(\text{pulled over}|\text{not speeding})$ because these two probabilities alone do not take into account how likely each event is.

therefore we need to weigh each conditional probability by the probability of its corresponding event (speeding or not speeding).
$P(\text{pulled over}) = P(\text{pulled over} | \text{speeding}) \cdot P(\text{speeding}) + P(\text{pulled over} | \text{not speeding}) \cdot P(\text{not speeding})$
$$
\begin{align}
P(\text{speeding})=\frac{1}{2} \\
\\
P(\text{pulled over}\mid\text{speeding})=\frac{1}{5} \\
\\
P(\text{not speeding})=\frac{1}{2} \\
\\
P(\text{pulled over}\mid\text{not speeding})=\frac{1}{10} \\
\end{align}
$$

$$
P(\text{pulled over}) = \left( \frac{1}{5} \right) \left( \frac{1}{2} \right) + \left( \frac{1}{10} \right) \left( \frac{1}{2} \right)
$$
$$
\begin{align}
P(\text{pulled over})&=\frac{1}{10}+\frac{1}{20} \\
&=\frac{2}{20}+\frac{1}{20} \\
&=\frac{3}{20} \\
\end{align}
$$

so, the total probability of being pulled over is $\frac{3}{20}$ or $15\%\space(0.15)$.