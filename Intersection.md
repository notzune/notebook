in math, the intersection of two or more objects is another object consisting of everything that is contained in all of the objects simultaneously.

## In [[Geometry|geometry]]

in geometry, an intersection is a point, line, or curve common to two or more objects (such as lines, curves, planes, and surfaces)

### On a plane

for the determination of the intersection point of two non-parallel lines

$$
a_1x+b_1y=c_1,a_2x+b_2y=c_2
$$

one gets (by using [[Cramer's rule]] or by substituting out a variable) the coordinates of the intersection point $(x_s,y_s)$:

$$
x_s=\frac{c_1b_2-c_2b_1}{a_1b_2-a_2b_1},y_s=\frac{a_1c_2-a_2c_1}{a_1b_2-a_2b_1}
$$

if $a_1-b_2-a_2b_1=0$ the lines are parallel and these formulas cannot be used because they involve dividing by 0.

for two non-parallel [[Line segment|line segments]] $(x_1,y_1),(x_2,y_2)$ and $(x_3,y_3),(x_4,y_4)$ there doesn't necessarily be an intersection point because the intersection point $(x_0,y_0)$ doesn't need to be contained in the line segments.

$$
\begin{align}
&(x(s),y(s))=(x_1+s(x_2-x_1),y_1+s(y_2-y_1)) \\
&(x(s),y(t))=(x_1+t(x_4-x_3),y_1+t(y_4-y_3)) \\
\end{align}
$$

the line segments intersect only ion a common point of the corresponding lines if the corresponding parameters $s_0,t_0$ fulfill the condition $0\leq s_0,t_0\leq1$. the parameters are the solution of the linear system

$$
\begin{align}
s(x_2-x_1)-t(x_4-x_3)=x_3-x_1 \\
s(y_2-y_1)-t(y_4-y_3)=y_3-y_1 \\
\end{align}
$$


## In [[Set theory|set theory]]

in set theory an intersection of two [[Sets|sets]] $A$ and $B$, denoted by $A\cap B$, is the set containing all elements of $A$ that also belong to $B$ or equivalently, all elements of $B$ that also belong to $A$

### Examples

$$
\begin{align}
\{1,2,3\}\cap\{2,3,4\}=\{2,3\} \\
\\
\{1,2,3\}\cap\{4,5,6\}=\emptyset \\
\\
\mathbb{Z}\cap\mathbb{N}=\mathbb{N} \\
\\
\{x\in\mathbb{R}:x^{2}=1\}\cap\mathbb{N}=\{1\}
\end{align}
$$

