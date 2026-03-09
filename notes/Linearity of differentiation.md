in [[Calculus|calculus]], the [[Derivative|derivative]] of any [[Linear combination|linear combination]] of [[Function|functions]] equals the same linear combination of the derivatives of the functions; 

this is also known as linearity of differentiation, the rule of linearity, or the [[Superposition principle|superposition rule]] for differentiation, the sum rule (the derivative of the sum of two functions is the sum of the derivatives) and the constant factor rule (the derivative of a constant multiple of a function is the same constant multiple of the derivative). 

let $f$ and $g$ be functions, with $\alpha$ and $\beta$ constants,

$$
\frac{d}{dx}(\alpha\cdot f(x)+\beta\cdot g(x))
$$

by the sum rule in differentiation, this is

$$
\frac{d}{dx}(\alpha\cdot f(x))+\frac{d}{dx}(\beta\cdot g(x))
$$

and by the constant factor rule in differentiation, this reduces to

$$
\alpha\cdot f'(x)+\beta\cdot g'(x)
$$

therefore, 

$$
\frac{d}{dx}(\alpha\cdot f(x)+\beta\cdot g(x))=\alpha\cdot f'(x)+\beta\cdot g'(x)
$$

omitting the brackets, this is often written as

$$
(\alpha\cdot f+\beta\cdot g)'=\alpha\cdot f'+\beta\cdot g'
$$

## Proof

let $a,b\in\mathbb{R}$. let $f,g$ be functions. let $j$ be a function, where $j$ is defined only where $f$ and $g$ are both defined (the [[Domain|domain]] of $j$ is the [[Intersection|intersection]] of the domains of $f$ and $g$). let $x$ be in the domain of $j$. let $j(x)=af(x)+bg(x)$.

we want to prove that $j'(x)=af'(x)+bg'(x)$.

by definition we can see that

$$
\begin{align}
j'(x)&=\lim_{h\rightarrow0}\frac{j(x+h)-j(x)}{h} \\
&=\lim_{h\rightarrow0}\frac{(af(x+h)+bg(x+h))-(af(x)+bg(x))}{h} \\
&=\lim_{h\rightarrow0}\frac{af(x+h)+bg(x+h)-af(x)-bg(x)}{h} \\
&=\lim_{h\rightarrow0}\frac{af(x+h)-af(x)+bg(x+h)-bg(x)}{h} \\
&=\lim_{h\rightarrow0}\frac{(af(x+h)-af(x))+(bg(x+h)-bg(x))}{h} \\
&=\lim_{h\rightarrow0}(\frac{af(x+h)-af(x)}{h}+\frac{bg(x+h)-bg(x)}{h}) \\
&=\lim_{h\rightarrow0}\left(\frac{a(f(x+h)-f(x))}{h}+\frac{b(g(x+h)-g(x))}{h}\right) \\
&=\lim_{h\rightarrow0}\left(a\frac{f(x+h)-f(x)}{h}+b\frac{g(x+h)-g(x)}{h}\right) \\
\end{align}
$$
