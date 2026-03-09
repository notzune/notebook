an important property of base-10 [[Logarithmic functions|logarithms]] which makes them useful in calculations is that the logarithm of numbers greater than 1 that differ by a power of 10 all have the same fractional part, called the mantissa. 

the mantissa represents the [[Significant figures|significant digits]] of a [[Floating-point arithmetic|floating-point number]], without considering its scale or magnitude. 

it's similar to the coefficient in scientific notation that carries the essential digits of a number. in scientific notation, a number like $5.12\times10^{3}$ has a coefficient (or "mantissa" in this analogy) of 5.12, which indicates the precision of the number, while $10^{3}$ (the [[Exponent|exponent]] part) determines its scale.

# In Context of [[Floating-point arithmetic]]

in floating-point representation, a number is typically stored in three parts: the sign, the exponent, and the mantissa. the length of the mantissa determines how precise the number can be. more [[Bit|bits]] allocated to the mantissa allow for a more precise representation of the significant digits of the number.

