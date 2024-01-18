in math, a differential equation is an equation that relates on o more unknown [[Function|functions]] and their [[Derivative|derivatives]].

in applications, the functions generally represent physical quantities, the derivates represent their [[Rate of change|rates of change]], and the differential equation defines a relationship between the two.

the study of differential equations consists mainly of the study of their solutions (the [[Sets|set]] of [[Function|functions]] that satisfy each equation), and of the properties of their solutions. 

only the simplest differentials are soluble by explicit formulas; however, many properties of the solutions of a given differential may be determined without computing them exactly.

differential equations, as defined by Newton, take forms similar to these three equations:

$$
\begin{align}
&\frac{dy}{dx}=f(x) \\
\\
&\frac{dy}{dx}=f(x,y) \\
\\
&x_1\frac{\partial y}{\partial x_1}+x_2\frac{\partial y}{\partial x_2}=y \\
\end{align}
$$

in all these cases, $y$ is an unknown function of $x$ (or of $x_1$ and $x_2$), and $f$ is a given function.

note that the $dx$ and $dy$ come from [[Leibniz's notation]] (see also [[Notation for differentiation|notation for differentiation]])

Jacob Bernoulli proposed the [[Bernoulli differential equation]] which is an [[Ordinary differential equation (ODE)|ordinary differential equation]] of the form

$$
y\prime+P(x)y=Q(x)y^n
$$

## Types

differential equations can be divided into several types which can help inform as to what approach one should take for a solution.

### [[Ordinary differential equation (ODE)|Ordinary Differential Equations (ODEs)]]

an ODE is an equation containing an unknown function of one real or complex variable $x$, its derivatives, and some given functions of $x$. the unknown function is generally represented by a variable (often denoted $y$). which *depends* on $x$.

thus $x$ is often called the *independent* variable of the equation as $y$ would be the *dependent*. this is in contrast with [[Partial differential equation (PDE)|partial differential equations]] which may have *more than* one independent variable.

#### Separable Equations

$$
\frac{dy}{dx}=g(x)h(y)
$$

and are best approached by separating the variables (also known as the [[Separation of variables|Fourier method]]) and [[Integral|integrating]] both sides. 

#### Exact Equations

$$
M(x,y)+N(x,y)\frac{dy}{dx}=0,\space\text{ where }\frac{\partial M}{\partial y}=\frac{\partial N}{\partial x}
$$

and are approached by finding the potential function.