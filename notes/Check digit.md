a check digit is a form of redundancy check used for error detection on identification numbers such as bank account numbers. it is similar to a [[Binary|binary]] [[Parity bit|parity bit]] which is used to check for errors in computer-generated data.

one of the more complex [[Algorithm|algorithms]] for check digits is known as the Luhn algorithm or Luhn formula. this is also known as the "[[Modulus|mod]] 10" algorithm. it works as follows:

1. remove the last digit of the number. this is the check digit.
2. reverse the digits of the number.
3. multiply the digits in odd positions (1, 3, 5, etc.) by 2 and subtract 9 to any result higher than 9
4. add all the numbers together
5. the sum plus the check digit should be a multiple of 10. if it is, the number is valid

# Example

take an example credit card number: 4004-6067-3429-0019 and determine if it has the correct check digit.

1. remove the last digit (the check digit):

$$
4004-6067-3429-001
$$

2. reverse the sequence:

$$ 
100-3429-7606-4004
$$

3. multiply every other position by $2$ (starting from the first number after reversing): 

$$
\begin{align*}
&1\times2, 0, 0\times2, 3, 4\times2, 2, 9\times2, 7, 6\times2, 0, 0\times2, 4, 0\times2, 0, 0\times2, 4 \\
=\ &2, 0, 0, 3, 8, 2, 18, 7, 12, 0, 0, 4, 0, 0, 0, 4
\end{align*}
$$

4. Subtract $9$ from numbers greater than $9$: 

$$
\begin{align*}
2, 0, 0, 3, 8, 2, 9, 7, 3, 0, 0, 4, 0, 0, 0, 4
\end{align*}
$$

5. sum all the numbers together and add the check digit (the check digit is $9$): 

$$
\sum = 2 + 0 + 0 + 3 + 8 + 2 + 9 + 7 + 3 + 0 + 0 + 4 + 0 + 0 + 0 + 4 + 9 = 51
$$

in this example the total is $51$ which is **not** a multiple of $10$ and therefore is an incorrect check digit.

# [[Pseudocode]] for the Luhn Algorithm

```plaintext
function isValidLuhn(number):
    remove the hyphens from number
    set sum to 0
    set checkDigit to the last digit of number
    remove the last digit from number
    reverse the digits in number
    
    for each digit in number at index i starting from 0:
        if i is even:
            double the digit
            if the doubled value is greater than 9:
                subtract 9 from the doubled value
        add the result (or the original digit if not doubled) to sum
        
    sum += checkDigit
    
    if sum modulo 10 is 0:
        return true
    else:
        return false
```


