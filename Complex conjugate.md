in math, the complex conjugate of a [[Complex numbers|complex number]] is the number with an equal [[Real numbers|real]] part and an [[Imaginary numbers|imaginary]] part equal in [[Magnitude|magnitude]] but opposite in [[Signed|sign]]. 

that is, if $a$ and $b$ are real numbers then the complex conjugate of $a+bi$ is $a-bi$. the complex conjugate of $z$ is often denoted as $\overline{z}$ or $z^*$.

in [[Polar coordinate system|polar form]], if $r$ and $\varphi$ are real numbers then the conjugate of $re^{i\varphi}$ is $re^{-i\varphi}$. this can be shown using [[Euler's formula]].

the product of a complex number and its conjugate is a real number: $a^2+b^2$ (or $r^2$ in [[Polar coordinate system|polar coordinates]]).

the complex conjugate of a complex number $z$ is written as $\overline{z}$ or $z^*$. the first notation (using a [[Vinculum|vinculum]]) avoids confusion with the notation for the [[Conjugate transpose|conjugate transpose]] of a [[Matrices|matrix]], which can be thought of as a generalization of the complex conjugate.

if a complex number is represented as a $2\times 2$ matrix, the notations are identical, and the complex conjugate corresponds to the [[Transpose|matrix transpose]], which is a flip along the diagonal.

## Properties

the following apply for all complex numbers $z$ and $w$, unless stated otherwise, and can be proved by writing $z$ and $w$ in the form $a+bi$.

for any two complex numbers, conjugation is [[Distributive property|distributive]] over addition, subtraction, multiplication and devision.

$$
\begin{align}
\overline{z+w}&=\overline{z}+\overline{w}, \\
\overline{z-w}&=\overline{z}-\overline{w}, \\
\overline{zw}&=\overline{z}\space\overline{w}, \\
\overline{(\frac{z}{w})}&=\frac{\overline{z}}{\overline{w}},\space\text{ if }w\neq 0\\
\end{align}
$$

a complex number is equal to its complex conjugate if its imaginary part is zero, that is, if the number is real. in other words, real numbers are the only [[Fixed point|fixed points]] of conjugation.

conjugation does not change the [[Modulus|modulus]] of a complex number: $|\overline{z}|=|z|$.

conjugation is an [[Involution|involution]], meaning the conjugate of the conjugate of a complex number $z$ is $z$. in symbols, $\overline{\overline{z}}=z$.

the product of a complex number with its conjugate is equal to the square of the number's modulus: $z\overline{z}=|z|^2$.

this property allows easy computation of the [[Multiplicative inverse|multiplicative inverse]] of a complex number given in rectangular coordinates:

$$
z^{-1}=\frac{\overline{z}}{|z|^2},\space\text{ for all }z\neq 0.
$$

conjugation is [[Commutative property|commutative]] under composition with [[Exponentiation|exponentiation]] to integer powers, with the [[Exponential function|exponential function]], and with the [[Natural logarithm|natural logarithm]] for nonzero arguments:

$$
\begin{align}
&\overline{z^n}=(\overline{z})^n,\space\text{ for all }n\in\mathbb{Z} \\
\\
&\exp(\overline{z})=\overline{\exp(z)} \\
\\
&\ln(\overline{z})=\overline{\ln(z)},\space\text{ if $z$ is not zero or a negative real number}
\end{align}
$$

if $p$ is a [[Polynomial|polynomial]] with [[Real numbers|real]] coefficients and $p(z)=0$, then $p(\overline{z})=0$ as well. thus, non-real roots of real polynomials occur in complex conjugate pairs (see [[Complex conjugate root theorem|complex conjugate root theorem]]).

in general, if $\varphi$ is a [[Holomorphic functions|holomorphic function]] whose restriction to the real numbers is real-valued, and $\varphi(z)$ and $\varphi(\overline{z})$ are defined, then

$$
\varphi(\overline{z})=\overline{\varphi(z)}
$$

the map of $\sigma(z)=\overline{z}$ from $\mathbb{C}$ to $\mathbb{C}$ is a [[Homeomorphism|homeomorphism]] (where topology on $\mathbb{C}$ is taken to be the standard topology) and [[Antilinear map|antilinear]], if one considers $\mathbb{C}$ as a complex [[Vector space|vector space]] over itself.

even though it may appear to be a [[Pathological|well-behaved]] function, it is not holomorphic; it reverses orientation wheres holomorphic functions locally preserve orientation. it is [[Bijection|bijective]] and compatible with the arithmetical operations, and hence is a [[Field|field]] [[Automorphism|automorphism]]. as it keeps the real numbers fixed, it is an element of the [[Galois group]] of the [[Field extension|field extension]] $\mathbb{C}/\mathbb{R}$. this Galois group has only two elements: $\sigma$ and the identity on $\mathbb{C}$. thus, the only two field automorphisms of $\mathbb{C}$ that leave the real numbers fixed are the identity map and complex conjugation.

