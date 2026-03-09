here is a list of notable [[Logarithmic functions|logarithmic]] [[Identity (mathematics)|identities]], remember that a logarithm can be defined by:

$$
\log_{b}(y)=x\iff b^{x}=y
$$

so from that we get these simple identities:

$$
\begin{align}
\log_{b}(1)&=0\text{ because }b^{0}=1 \\
\log_{b}(b)&=1\text{ because }b^{1}=b \\
\\
b^{\log_{b}(x)}&=x \\
\log_{b}(b^{x})&=x \\
\end{align}
$$

## Simplifying operations 

$$
\begin{align}
&\log_{b}(xy)=\log_{b}(x)+\log_{b}(y)&\text{because }&b^{c}b^{d}=b^{c+d} \\
\\
&\log_{b}(\frac{x}{y})=\log_{b}(x)-\log_{b}(y)&\text{because }&\frac{b^{c}}{b^{d}}=b^{c-d} \\
\\
&\log_{b}(x^d)=d\log_{b}(x)&\text{because }&(b^{c})^{d}=b^{cd} \\
\\
&\log_b(\sqrt[y]{x})=\frac{\log_{b}(x)}{y}&\text{because }&\sqrt[y]{x}=x^{\frac{1}{y}} \\
\\
&x^{\log_{b}(y)}=y^{\log_{b}(x)}&\text{because }&x^{\log_{b}(y)}=b^{\log_{b}(x)\log_{b}(y)}\\
&&&=(b^{\log_{b}(y)})^{\log_{b}(x)} \\
&&&=y^{\log_{b}(x)} \\
\\
&c\log_{b}(x)+d\log_{b}(y)=\log_{b}(x^{c}y^{d})&\text{because }&\log_{b}(x^{c}y^{d})=\log_{b}(x^{c})+\log_{b}(y^{d})
\end{align}
$$

where $b$, $x$, and $y$ are positive real numbers and $b\neq1$, and $c$ and $d$ are real numbers.