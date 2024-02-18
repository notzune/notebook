in [[Statistics|statistics]], the conditional probability table is defined for a [[Sets|set]] of [[Continuous or discrete variable#Discrete variable|discrete]] and mutually [[Independence|dependent]] [[Random variables|random variables]] to display the [[Conditional probability|conditional probabilities]] of a single variable with respect to the others (in other words, the probability of each possible value of one variable if we know the values taken on by the other variables). 

a conditional probability table can also be put into [[Matrices|matrix]] form.

# Examples

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

for a more complex example involving something like designing NPC/AI behavior we can assume a scenario where we are meant to design the NPCs to make certain decisions (such as patrolling, interacting with other players, or seeking shelter) based on multiple gameplay elements/factors (such as the time of day, weather, player presence)

let's assign some random variables to the events

- $T$ - time of day $\{\text{day, night}\}$
- $W$ - weather $\{\text{clear, storm}\}$
- $P$ - player $\{\text{near, far}\}$
- $B$ - NPC behavior $\{\text{patrol, interact, shelter}\}$

in this scenario, $B$ would be dependent on $T, W,$ and $P$.

|time |weather |player |$P(B_\text{patrol})$ |$P(B_\text{interact})$ |$P(B_\text{shelter})$ |
|---|---|---|---|---|---|
|day |clear |near |$0.3$ |$0.6$ |$0.1$ |
|day |clear |far |$0.7$ |$0.2$ |$0.1$ |
|day |storm |near |$0.2$ |$0.5$ |$0.3$ |
|day |storm |far |$0.6$ |$0.1$ |$0.3$ |
|night |clear |near |$0.5$ |$0.4$ |$0.1$ |
|night |clear |far |$0.8$ |$0.1$ |$0.1$ |
|night |storm |near |$0.1$ |$0.2$ |$0.7$ |
|night |storm |far |$0.4$ |$0.1$ |$0.5$ |

then we can express the specific categorical variable with a matrix:

$$
P(B_\text{patrol})=
\begin{bmatrix}
    0.3 & 0.5 & 0.2 & 0.1 \\
    0.7 & 0.8 & 0.6 & 0.4 \\
\end{bmatrix}
$$

from a [[Computer programming|programming]] perspective in something like [[Java]], we can implement something like

```java
public NPCBehavior decideBehavior(Time time, Weather weather, PlayerPresence playerPresence) {
    // Assume cpt is a pre-defined data structure containing the CPT
    double[] probabilities = cpt.get(time).get(weather).get(playerPresence);
    return weightedRandomChoice(probabilities, NPCBehavior.values());
}
```


