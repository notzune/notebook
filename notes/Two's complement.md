most common [[Signed number representations|method of representing signed]] (positive, negative, and zero) [[Integer|integers]] on [[Computer|computers]], and more generally, [[Fixed-point arithmetic|fixed point binary]] values. two's complement uses the [[Bit numbering|binary digit with the greatest place value]] as the sign to indicate whether the binary number is positive or negative. when the most significant bit is $1$, the number is [[Signed|signed]] as negative; and when the most significant bit is $0$, the number is signed as positive.

it is computed by:

1. starting with the binary representation of the number, with the leading bit being a sign bit
2. inverting (flipping) all bits–changing every 0 to 1, and vice versa
3. adding 1 to the entire inverted number, ignoring any [[Integer overflow|overflow]].  (accounting for overflow will produce the wrong value)

# Example

calculate the decimal number $-6$ from the binary number $6$

1. $+6$ in decimal is $0110$ in binary; the leftmost significant bit (the first $0$) is the sign
2. flip all bits in $0110$, giving $1001$.
3. add the place value to the flipped number $1001$, giving $1010$.

to verify that $1010$ indeed has a value of $-6$, add the place values together but subtract the sign value from the first calculation because the most significant value is the sign value, it must be subtracted to produce the correct result:

$$
\begin{align}
1010&=-(1\times2^{3})+(0\times2^{2})+(1\times2^{1})+(0\times2^{0}) \\
\\
&=1\times-8+0+1\times2+0 \\
\\
&=-6
\end{align}
$$
