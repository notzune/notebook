## Mass given density

mass is found by multiplying the volume by the density where density is uniform.

$$\text{m}=\text{V}\cdot\rho$$

when density $\rho$ is not uniform, we take the [[Integral|integral]] of the [[Density|density]] function to find the [[Mass|mass]].

### example

$$\rho=\rho(x)=2x\sqrt{5-2x^2};\space 0<x<1$$

$$
m=\int^{1}_{0}2x\sqrt{5-2x^2}\space dx
$$
$$
\begin{align}
u=5-2x^2 \\
\\
du=-4x\space dx \\
\\
\frac{-du}{z}=2\space dx\\
\\
=-\frac{1}{2}\frac{u^{\frac{3}{2}}}{\frac{3}{2}}
\end{align}
$$
## Springs ([[Hooke's Law]])

$$F_s=Kd=Kx$$

where $Kd$ is the [[Displacement|displacement]] from equilibrium, it is positive when spring is stretched.

work done by a force (a to b):

$$
W=\int^{a}_{b}F(x)dx
$$

an example is how much force is needed to move an object from $x=0$ to $x=3$ in the presence of $F(x)=5x^2$

$$
W=\int^{3}_{0}5x^2\space dx=\frac{5x^3}{3}=45
$$

now find W needed to compress spring 1 meter, if $F=40\text{N}$ holds the spring 2 meters from equilibrium.

$$
F_s=Kd\implies-40=K(-2);K=20
$$

$$
\begin{align}
W=\int^{1}_{0}20x\space dx \\
=10x^2 \\
=10\text{J}
\end{align}
$$

