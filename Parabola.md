a parabola is a [[Plane curve|plane curve]] which is [[Reflection symmetry|mirror-symmetrical]] and is approximately U-shaped; it is a [[Conic sections|conic section]].

a parabola has a [[Point|point]] (the [[Focus|focus]]) and a [[Line|line]] (the [[Directrix|directrix]]). the focus does not lie on the directrix. 

the parabola is the [[Locus of points|locus of points]] in that plane that are [[Equidistant|equidistant]] from the directrix and the focus.

a parabola is given by the function

$$
y=ax^{2}+bx+c,\space\text{where }a\neq0
$$

# Roots

the [[Zero|roots or zeroes]] of a parabola are the values of $x$ for which $y=0$. using the [[Quadratic formula|quadratic formula]], the roots can be found by:

$$
x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}
$$

if the parabola is defined by two roots, $x_1$ and $x_2$, the quadratic can be expressed as

$$
y=a(x-x_1)(x-x_2)
$$

# [[Vertex (geometry)|Vertex]]

the vertex of a parabola is the highest or lowest point, depending on whether the parabola opens upwards ($a>0$) or downwards ($a<0$), the vertex can be found using the formula

$$
x_v=\frac{-b}{2a}
$$

and by substituting $x_v$ back into the original equation, we can find the $y$-coordinate of the vertex ($y_v$),

$$
y_v=a(x_v)^{2}+bx_v+c
$$

## Vertex form

the vertex form of a parabola, which is given by

$$
y=a(x-h)^{2}+k
$$

where $(h,k)$ is the vertex of the parabola.

# Axis of symmetry

the axis of symmetry is a vertical line that passes through the vertex of the parabola, and it can be defined by the same equation used to find the $x_v$ of the vertex

$$
x_{\text{symmetry}}=\frac{-b}{2a}
$$

# Focus and directrix

## Focus

the focus of a parabola is a point $(f_x,f_y)$ from which distances are measured to form the parabola. 

the directrix is a line opposite the opening of the parabola. the distance from any point on the parabola to the focus is equal to the [[Perpendicularity|perpendicular]] distance from that point to the directrix.

the focus for a parabola in vertex form is given by

$$
(f_x,f_y)=\left(h,k+\frac{1}{4a}\right)
$$

## Directrix

the directrix for a parabola in vertex form is the line given by 

$$
y=k-\frac{1}{4a}
$$

# Examples

## Finding a parabola from an ordered pair

say a certain manufacturing plant makes metal cylinders with a diameter of $50.0\,\text{mm}$ with a tolerance[^1] of $0.5\,\text{mm}$, we want to then graph the parabola that represents the possible values of the diameter.[^2]

so now from this we know: 

the diameter is meant to be $50.0\,\text{mm}$ which is the "perfect" diameter (where we can assume most of the values will fall around) and we can correctly assume this to be the vertex of the function.

the parabola should have a maximum or minimum at the [[#Vertex (geometry) Vertex|vertex]], representing the ideal measurement without any tolerance.

the parabola will intersect the $x$-axis (diameter) at the points where the tolerance is at its limits, which we know are $49.5\,\text{mm}$ and $50.5\,\text{mm}$.

given this we can set up the parabola in [[#Vertex form|vertex form]]. we can assume the vertex $(h,k)$ is at the perfect measurement ($50.0\,\text{mm}$, the *goal*) and the maximum value ($k$) which can be any positive value since it just represent the maximum amount of tolerance; set this to $k=1$.5[^3]. 

the vertex form of the parabola is then:

$$
\begin{align}
y&=a(x-h)^{2}+k \\
\\
y&=a(x-50.0)^{2}+1.5 \\
\end{align}
$$

to find $a$, we can use the fact that we know the roots of the parabola (where it intersects the $x$-axis) since we know the limits of the function (the range of possible values, $49.5$ and $50.5$), and that we know since it intersects the $x$-axis then $y=0$.

$if we plug in $x=49.5$ into the equation and solve for $a$ using $y=0$ at this point:

$$
0=a(49.5-50.0)^{2}+1.5
$$

solving for $a$, we get:

$$
\begin{align}
-1.5&=a(-0.5)^{2} \\
\\
-1.5&=0.25a \\
\\
a&=-6 \\
\end{align}
$$

so the equation modeling the possible diameters for metal cylinders at this particular factory is

$$
f(x)=1.5-6(x-50.0)^{2}
$$

[^1]: the [[Tolerance|tolerance of something]] just means plus/minus ($\pm\,n$) whatever value the tolerance is said to be ($n$), in this case: $50.0\pm0.5=(49.5,50.5)$.
[^2]:  in-order to get the [[Probability distribution|probability distribution]] so that we can calculate the [[Probability|probability]] that a cylinder will have a specific diameter within the allowed range. (see also: [[Probability density function (PDF)#Example|this example]])
[^3]: this number is arbitrary, it can mean literally anything since there is no other context given for this example, i actually don't even know why it would be 1.5, that's just the number that the textbook used for this problem when I was working through it