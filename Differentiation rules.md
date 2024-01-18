## Rules for basic functions

the following are the rules for the derivatives of the most common basic functions. here, $a$ is a real number and $e$ is [[e (constant)|the mathematical constant approximately 2.71828]].

- ### Derivates of powers:
	$$
	\begin{align}
	&\frac{d}{dx}x^a=ax^{a-1} \\
	\end{align}
	$$

- ### Functions of [[Exponential function|exponential]], [[Natural log|natural logarithm]], and [[Logarithmic functions|logarithm]] with general base:
	$$
	\begin{align}
	&\frac{d}{dx}e^x=e^x \\
	\\
	&\frac{d}{dx}a^x=a^x\ln(a),\text{ for $a>0$} \\
	\\
	&\frac{d}{dx}\ln(x)=\frac{1}{x},\text{ for $x>0$} \\
	\\
	&\frac{d}{dx}\log_a{(x)}=\frac{1}{x\ln(a)},\text{ for $x,a>0$} 
	\end{align}
	$$

- ### [[Trigonometric functions]]
	$$
	\begin{align}
	&\frac{d}{dx}\sin(x)=\cos(x) \\
	\\
	&\frac{d}{dx}\cos(x)=-\sin(x) \\
	\\
	&\frac{d}{dx}\sec^2(x)=\frac{1}{\cos^2(x)}=1+\tan^2(x) \\
	\end{align}
	$$

- ### [[Inverse trigonometric functions]]
	$$
	\begin{align}
	&\frac{d}{dx}\arcsin(x)=\frac{1}{\sqrt{1-x^2}},\text{ for }-1<x<1 \\
	\\
	&\frac{d}{dx}\arccos(x)=-\frac{1}{\sqrt{1-x^2}},\text{ for }-1<x<1 \\
	\\
	&\frac{d}{dx}\arctan(x)=\frac{1}{1+x^2}
	\end{align}
	$$

- ### Rules for [[Function composition|combined functions]]
	(given that the $f$ and $g$ are functions)
	
	- *Constant rule*: 
		
		if $f$ is constant, then for all $x$,
		$$
		f'(x)=0
		$$
	
	- *[[Linearity of differentiation|Sum rule]]*:
		$$
		(\alpha f+\beta g)'=\alpha f' +\beta g'
		$$
		for all functions $f$ and $g$ and all real numbers $\alpha$ and $\beta$.
	
	- *[[Product rule]]*:
		$$
		(fg)'=f'g+fg'
		$$
		for all functions $f$ and $g$. as a special case, this rule includes the fact
		$$
		(\alpha f)'=\alpha f'
		$$
		whenever $\alpha$ is a constant because $\alpha'f=0\cdot f=0$ by the constant rule
	
	- *[[Quotient rule]]*:
		$$
		\left(\frac{f}{g}\right)'=\frac{f'g-fg'}{g^2}
		$$
		for all functions $f$ and $g$ at all inputs where $g\neq0$.
	
	- [[Chain rule]] for [[Function composition|composite functions]]: 
		
		if $f(x)=h(g(x))$, then
		$$
		f'(x)=h'(g(x))\cdot g'(x)
		$$
		