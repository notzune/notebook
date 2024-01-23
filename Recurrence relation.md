a recurrence relation is an [[Equation|equation]] according to which the $n$th term of a [[Sequence|sequence]] of numbers is equal to some combination of the previous terms.

only $k$ previous terms of the sequence appear in the equation, for a [[Parameter|parameter]] $k$ that is independent of $n$; this number $k$ is called the order of the relation.

if the values of the first $k$ numbers in the sequence have been given, the rest of the sequence can be calculated by repeatedly applying the equation.

in linear recurrences, the $n$th term is equated to a [[Linear function|linear function]] of the $k$ previous terms. 

a famous example is the recurrence for the [[Fibonacci sequence|fibonacci numbers]]:

$$
F_n=F_{n-1}+F_{n-2}
$$

where the order $k$ is two and the linear function adds the two previous terms. this example is a [[Linear recurrence with constant coefficients|linear recurrence with constant coefficients]], because the coefficients of the linear function (1 and 1) are constants that do not depend on $n$.

for these kind of recurrences, one can express the general term of the sequence as a [[Closed-form expression|closed-form expression]] of $n$.

[[P-recursive equation|linear recurrences with polynomial coefficients]] depending on $n$ are also important because many common elementary and [[Special functions|special functions]] have a [[Taylor series]] whose coefficients satisfy such a recurrence relation. (see: [[Holonomic functions|holonomic functions]])

solving a recurrence relation means obtaining a [[Closed-form expression|closed-form solution]]: a non-recursive function of $n$.

## Definition

a recurrence relation is an equation that expresses each element of a sequence as a function of the preceding ones. in the case where only the immediately preceding element is involved, a recurrence relation has the form:

$$
u_n=\varphi(n,u_{n-1})\space\space\text{ for }n>0,\\
$$

where, 

$$
\varphi:\mathbb{N}\times X\rightarrow X\\
$$

is a function, where $X$ is a [[Sets|set]] to which the elements of a sequence must belong. for any $u_0\in X$, this defines a unique sequence with $u_0$ as its first element, called the initial value.

it is easy to modify the definition for getting sequences starting from the term of index 1 or higher.

this defines recurrence relation of first order. a recurrence relation of order $k$ has the form

$$
u_n=\varphi(n,u_{n-1},u_{n-2},...,u_{n-k})\space\text{ for }n\geq k
$$

where,

$$
\varphi:N\times X^k\rightarrow X
$$

is a function that involves $k$ consecutive elements of the sequence. in this case, $k$ initial valeus are needed for defining a sequence.

## Examples

### Factorial

the [[Factorial|factorial]] is defined by the recurrence relation

$$
n!=n(n-1)!\space\text{ for }n>0
$$

and the initial condition

$$
0!=1
$$

this is an example of a linear recurrence with polynomial coefficients of order 1, with the simple polynomial

$$
f(n)=n
$$

as its only [[Coefficient|coefficient]].

### Logistic map

a [[Logisitc map|logistic map]] is another example of a recurrence relation

$$
x_{n+1}=rx_n(1-x_n)
$$

with a given [[Constant|constant]] $r$; given the initial term $x_0$, each subsequent term is determined by this relation.