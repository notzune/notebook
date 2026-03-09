in [[Propositional calculus|propositional logic]], modus tollens is a [[Deductive reasoning|deductive]] [[Logical form|argument form]] and a [[Rule of inferences|rule of inference]].

modus tollens is a mixed [[Hypothetical syllogism|hypothetical syllogism]] that takes the form of: "if $P$, then $Q$. not $Q$. therefore, not $P$".

it is the application of the general truth that if a statement is true, then so is its [[Contraposition|contrapostive]].

the form shows that [[Inferences|inference]] from $P$ implies $Q$ to the negation of $Q$ implies the negation of $P$ is a [[Validity|valid]] [[Argument|argument]].

modus tollens is closely related to [[Modus ponens|modus ponens]].

$$
\begin{align}
&\text{If $P$, then $Q$.} \\
&\text{Not $Q$.} \\
&\text{Therefore, not $P$.}
\end{align}
$$

the first [[Premise|premise]] is a [[Conditional statement|conditional]] (if-then) claim, such as $P\implies Q$. the second premise is an assertion that $Q$, the [[Consequent|consequent]] of the conditional claim, is not hte case.

from these two premises it can be logically concluded that $P$, the [[Antecedent|antecedent]] pf the conditional claim, is also not true.

for example:

$$
\begin{align}
&\text{If the dog detect s an intruder, the dog will bark.} \\
&\text{The dog did not bark.} \\
&\text{Therefore, no intruder was detected by the dog.} \\
\end{align}
$$

## Relation to *modus ponens*

every use of modus tollens can be converted to use a modus ponens and one use of [[Transposition|transposition]] to the premise which is a material [[Implication|implication]]. 

$$
\begin{align}
&\text{If $P$, then $Q$.}&\text{(premise - material implication)} \\
&\text{If not $Q$, then not $P$.}&\text{(derived by transposition)} \\
&\text{Not $Q$.}&\text{(premise)} \\
&\text{Therefore, not $P$.}&\text{(derived by modus ponens)} \\
\end{align}
$$

likewise, every use of modus ponens can be converted to a use of modus tollens and transposition. 

$$
\begin{align}
&P\rightarrow Q,\neg Q \\
&\text{\_\_\_\_\_\_\_\_\_\_} \\
&\therefore\neg P
\end{align}
$$