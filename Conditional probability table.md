in [[Statistics|statistics]], the conditional probability table is defined for a [[Sets|set]] of [[Continuous or discrete variable#Discrete variable|discrete]] and mutually [[Independence|dependent]] [[Random variables|random variables]] to display the [[Conditional probability|conditional probabilities]] of a single variable with respect to the others. (in other words, the probability of each possible value of one variable if we know the values taken on by the other variables).

a conditional probability table can also be put into [[Matrices|matrix]] form.

let's consider a simple example with two [[Categorical variable|categorical variables]], one describing the weather [[Events|event]] $W=\{\text{rain}, \text{no rain}\}$, and another describing whether or not to carry an umbrella $U=\{\text{carry},\text{no carry}\}$.

in-order to simplify this, we can just make the outcome of rain be $W$ and the outcome of it not raining be the [[Complement (probability)|complement]], $W'$ and the same for carrying or not carrying an umbrella: $U$ and $U'$, respectively.

the decision to carry an umbrella ($U$), is [[Conditional probability|conditional]] on the weather ($W$):

| Weather | $P(U\mid W)$ | $P(U'\mid W)$ |
| ---- | ---- | ---- |
| Rain ($W$) | $0.9$ | $0.1$ |
| No rain ($W'$) | $0.2$ | $0.8$ |

from the table we can see that if it's raining, there's a $90\%$ chance a person will carry an umbrella and $10\%$ chance they will not and if it's not raining there's a $20\%$ chance they will carry an umbrella and $80\%$ chance they will not.

in matrix form, this would be shown as 

$$
W\times U=\begin{bmatrix}
    0.9 & 0.1 \\
    0.2 & 0.8 \\
\end{bmatrix}
$$

