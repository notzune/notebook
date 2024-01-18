this notation is not to be confused with the notation:

$$
\begin{align*}
b \mod n
\end{align*}
$$
(note that it is written without parentheses) 


which refers to the [[Modulo]] operation which is a calculation and not a relation between numbers.

modular arithmetic is often referred to as "wrap around" arithmetic. the most common example is how the numbers on clock behave; the numbers "wrap around" or "rest" after reaching a certain value called the [[Modulus]] (in this case 12).

given an integer $n > 1$, called a [[Modulus]], two integers $a$ and $b$ are said to be congruent modulo $n$, if $n$ is a divisor of their difference; that is, if there is an integer $k$ such that:

$$
a − b = kn
$$
congruent modulo $n$ is a [[Congruence Relation|congruence relation]], meaning that it is an [[Equivalence relation|equivalence relation]] that is compatible with the operations of addition, subtraction, and multiplication.

it is denoted as:
$$
a \equiv b\pmod{n}
$$
which reads "a is congruent to b modulo n." this means that when $a$ and $b$ are divided by $n$, they have the same remainder.
$$

$$
one use of modular arithmetic is in the 12-hour clock, in which the day is divided into two 12-hour periods. 

if the time is 7:00 now, then 8 hours later it will be 3:00. simple addition would result in 7 + 8 = 15, but 15:00 reads as 3:00 on the clock face because clocks "wrap around" every 12 hours and the hour number starts over at zero when it reaches 12. 

we  can then say that 15 is congruent to 3 modulo 12, written: 
$$15 \equiv 3\pmod{12}$$
so that:
$$
7 + 9 \equiv 3\pmod{12}
$$
similarly, 8:00 represents a period of 8 hours, and twice this would give 16:00, which reads as 4:00 on the clock face, written as:
$$
2\times8 \equiv 4\pmod{12}
$$
