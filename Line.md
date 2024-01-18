in [[Geometry|geometry]], a straight line (line) is an infinitely long object with no width, depth, or [[Curvature|curvature]]. 

lines are [[Space|spaces]] of [[Dimension|dimension]] one, which may be [[Embedding|embedded]] in spaces of dimension two, three, or higher.

in three-dimensional space, a first degree equation in the variables $x$, $y$, and $z$ defines a plane, so two such equations provided the planes they give rise to are not parallel, define a line which is the [[Intersection|intersection]] of the planes.

more generally, in $n$-dimensional space $n-1$ first degree equations in the $n$ [[Coordinates|coordinate]] variables define a line under suitable conditions.

in more general [[Euclidean space]], $R^n$ (and in every other [[Affine space|affine space]]) , the line $L$ passing through two different points $a$ and $b$ has the [[Subset|subset]]:

$$
L=\{(1-t)a+tb|t\in\mathbb{R}\}
$$

the [[Orientation|direction]] of the line is from a reference point $a(t=0)$ to another point $b(t=1)$, or in other words, in the direction of the vector $b-a$. different choices of $a$ and $b$ can yield the same line.

three points are said to be [[Colinearity|collinear]] if they lie on the same line. three points usually determine a plane but in the case of three collinear points this does *not* happen. 

in [[Affine space|affine coordinates]], in $n$-dimensional space the points $X=(x_1,x_2,\dots,x_n),Y=(y_q,y_2,\dots,y_n)$ and $Z=(z_1,z_2,\dots,z_n)$ are collinear if the [[Matrices|matrix]]

$$
\begin{bmatrix}
    1 & x_1 & x_2 & ... & x_n \\
    1 & y_1 & y_2 & ... & y_n \\
    1 & z_1 & z_2 & ... & z_n \\
\end{bmatrix}
$$

has a [[Rank|rank]] less than 3. for three points in the plane ($n=2$), the above matrix is square and the points are collinear if and only if its [[Determinant|determinant]] is zero. 

the points $a$, $b$, and $c$ are collinear if and only if $d(x,a)=d(c,a)\text{ and }d(x,b)=d(c,b)\implies z=c$.

this doesn't hold true for all notions of distance (such as the [[Taxicab geometry|Manhattan distance]]).

a straight line has the formula 

$$
y=mx+b
$$

where $m$ is the [[Slope|slope]] of the line.