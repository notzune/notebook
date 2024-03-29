in mathematics, especially in [[Algebra|algebra]], factorization consists of writing a number or another mathematical object as a product of several factors, usually smaller or simpler objects.

for example, $3\times5$ is an [[Integer factorization|integer factorization]] of $15$, and $(x-2)(x+2)$ is a [[Polynomial factorization|polynomial factorization]] of $x^2-4$.

# General methods

the following methods apply to any expression that is a sum or that may be transformed into a sum.

## Common factor

the [[Distributive property|distributive law]] allows factoring out a common factor

$$
6x^3y^2+8x^4y^3-10x^5y^3=2x^3y^2(3+4xy-5x^2y)
$$

## Grouping

to factor the following by grouping

$$
4x^2+20x+3xy+15y
$$

we can see that the first two terms have a common factor ($x$), and the last two terms have a common factor ($y$),

$$
(4x^2+20x)+(3xy+15y)=4x(x+5)+3y(x+5)
$$

from this we can see the [[Factorization#Common factor|common factor]] $x+5$ and we can factor it out as

$$
4x^2+20x+3xy+15y=(4x+3y)(x+5)
$$

in general this works for sums of 4 terms that have been obtained as the product of two [[Binomial (polynomial)|binomials]].

## Adding and subtracting terms

a typical use of this is the [[Completing the square|completing the square]] method for getting the [[Quadratic formula|quadratic formula]].

an example would be the factorization of $x^4+1$, which introduces the [[Imaginary numbers|non-real square root of -1]], denoted as $i$, then one has a [[Difference of two squares|difference of squares]].

$$
x^4+1=(x^2+i)(x^2-i)
$$

by adding and subtracting $2x^2$, and grouping three terms,

$$
\begin{align}
x^4+1&=(x^4-2x^2+1)-2x^2 \\
&=(x^2+1)^2-(x\sqrt{2})^2 \\
&=(x^2+x\sqrt{2}+1)(x^2-x\sqrt{2}+1) \\
\end{align}
$$

subtracting and adding $2x^2$ also yields

$$
\begin{align}
x^4+1&=(x^4-2x^2+1)+2x^2 \\
&=(x^2-1)^2+(x\sqrt{2})^2 \\
&=(x^2+x\sqrt{-2}-1)(x^2-x\sqrt{-2}-1) \\
\end{align}
$$

the factorizations work not only over the complex numbers, but also over any [[Field|field]], where either -1, 2 or -2 is a square.

in a [[Finite field|finite field]], the product of two non-squares is a square; this implies that the polynomial $x^4+1$, which is [[Irreducible polynomial|irreducible]] over the integers, is reducible [[Modulo|modulo]] every prime number. for example,

$$
\begin{align}
x^4+1&\equiv(x+1)^4\pmod{2} \\
x^4+1&\equiv(x^2+x-1)(x^2-x-1)\pmod{3} \\
\end{align}
$$
since $1^2\equiv-2\pmod{3}$;

$$
x^4+1\equiv(x^2+2)(x^2-2)\pmod{5}
$$
since $2^2\equiv-1\pmod{5}$;

$$
x^4+1\equiv(x^2+3x+1)(x^2-3x+1)\pmod{7}
$$
since $3^2\equiv2\pmod{7}$.

# Recognizable patterns

here are identities that are pretty commonly used patterns. in these examples, the variables $E$ and $F$ may represent any subexpression of the expression that has to be factorized.

## [[Difference of two squares]] 

$$
E^2-F^2=(E+F)(E-F)
$$
for example

$$
\begin{align}
a^2+2ab+b^2&-x^2+2xy-y^2 \\
&=(a^2+2ab+b^2)-(x^2-2xy+y^2) \\
&=(a+b)^2-(x-y)^2 \\
&=(a+b+x-y)(a+b-x+y) \\
\end{align}
$$

## Sum/difference of two cubes

$$
\begin{align}
E^3+F^3=(E+F)(E^2-EF+F^2) \\
\\
E^3-F^3=(E-F)(E^2+EF+F^2) \\
\end{align}
$$

## Difference of two fourth powers

$$
\begin{align}
E^4-F^4&=(E^2+F^2)(E^2-F^2) \\
&=(E^2+F^2)(E+F)(E-F)
\end{align}
$$

## Sum/difference of two $n$th powers
### Difference, even exponent

$$
E^{2n}-F^{2n}=(E^n+F^n)(E^n-F^n)
$$

### Difference, even or odd exponent

$$
E^n-F^n=(E-F)(E^{n-1}+E^{n-2}F+E^{n-3}F^2+\dots+EF^{n-2}+F^{n-1})
$$

### Sum, odd exponent

$$
E^n+F^n=(E+F)(E^{n-1}=E^{n-2}F+E^{n-3}F^2-\dots-EF^{n-2}+F{n-1})
$$

### Sum, even exponent

if the exponent is a power of two then the expression cannot be factorized without introducing [[Complex numbers|complex number]]. if $n$ has an odd divisor (if $n=pq$ with $p$ being odd), then use the formula [[Factorization#Sum, odd exponent|above]].

### Trinomials and cubic formulas

$$
\begin{align}
&x^2+y^2+z^2+2(xy+yz+xz)=(x+y+z)^2 \\
\\
&x^3+y^3+z^3-3xyz=(x+y+z)(x^2+y^2+z^2-xy-xz-yz) \\
\\
&x^3+y^3+z^3+3x^2(y+z)+3y^2(x+z)+3x^2(x+y)+6xyz=(x+y+z)^3 \\
\\
&x^4+x^2y^2+y^4=(x^2+xy+y^2)(x^2-xy+y^2) \\
\end{align}
$$

### [[Binomial theorem|Binomial expansions]]

$$
\begin{align}
&a^2+2ab+b^2=(a+b)^2 \\
\\
&a^2-2ab+b^2=(a-b)^2 \\
\\
&a^3+3a^2b+3ab^2+b^3=(a+b)^3 \\
\\
&a^3-3a^2b+3ab^2-b^3=(a-b)^3 \\
\end{align}
$$

### [[Root of unity|Roots of unity]]

the $n$th roots of unity are the complex numbers which are a root of the polynomial $x^n-1$.

$$
e^{2ik\pi/n}=\cos\frac{2\pi k}{n}+i\sin\frac{2\pi k}{n}
$$

for $k=0,\dots,n-1$.

so for any two expressions $E$ and $F$, one has

$$
\begin{align}
&E^n-F^n=(E-F)\prod^{n-1}_{k=1}(E-Fe^{2ik\pi/n}) \\
\\
&E^n+F^n=\prod^{n-1}_{k=0}(E-Fe^{(2k+1)i\pi/n})&\text{ if $n$ is even} \\
\\
&E^n+F^n=(E+F)\prod^{n-1}_{k=1}(E+Fe^{2ik\pi/n})&\text{ if $n$ is odd}
\end{align}
$$

if $E$ and $F$ are real expressions, and one wants real factors, you have to replace every pair of [[Complex conjugate|complex conjugate]] by its product

as the complex conjugate of $e^{i\alpha}$ is $e^{-i\alpha}$, and

$$
\begin{align}
(a-be^{i\alpha})(a-be^{-i\alpha})&=a^2-ab(e^{i\alpha}+e^{-i\alpha})+b^2e^{i\alpha}e^{-i\alpha} \\
&=a^2-2ab\cos\alpha+b^2 \\
\end{align}
$$

