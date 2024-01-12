a group in math is a [[Sets|set]] with an [[Operation|operation]] that satisfies the following constraints: the operation is [[Associative property|associative]] and has an [[Identity element|identity element]], and every element of the set has an [[Inverse element|inverse element]].

one of the more familiar groups is the set of [[Integer|integers]] with addition:

$$
\mathbb{Z}=\{...,-4,-3,-2,-1,0,1,2,3,4,...\}
$$

for any two integers $a$ and $b$, the sum $a+b$ is also an integer. this [[Closure|closure]] property says that addition is a [[Binary Operation|binary operation]] on $\mathbb{Z}$. the following properties help define the group axiom:

- for all integers $a,b,\text{ and }c$, one has $(a+b)+c=a+(b+c)$ which is a demonstration of the [[Associative property|associative property]], more specifically the [[Associativities of Addition and Multiplication|associativities of addition]].
- if $a$ is any integer, then $0+a=a$ and $a+0=a$. [[Zero|zero]] is called the [[Identity element|identity element]] of addition because adding it to any integer returns the same integer.
- for every integer $a$, there is an integer $b$ such that $a+b=0\text{ and }b+a=0$. the integer $b$ is called the [[Inverse element|inverse element]] of $a$ and is denoted $-a$.

# Definition

a group is a non-empty set $G$ together with a binary operation on $G$, here denoted "$\cdot$", that combines any two elements $a$ and $b$ of $G$ to form an element of $G$, denoted $a\cdot b$, such that the following three requirements, known as [[Group axiom|group axioms]], are satisfied:

1. [[Associative property|associativity]]: for all $a,b,c$ in $G$, one has $(a\cdot b)\cdot c=a\cdot(b\cdot c)$.
2. [[Identity element|identity element]]: there exists an element $e$ in $G$ such that for every $a$ in $G$, one has $e\cdot a=a\text{ and }a\cdot e=a$.
3. [[Inverse element|inverse element]]: for each element $a$ in $G$, there exists an element $b$ in $G$ such that $a\cdot b=e\text{ and }b\cdot a=e$, where $e$ is the identity element.

basic facts about all groups that can be obtained directly from these group axioms.

for example, repeated applications (through [[Mathematical induction|induction]] of the associativity axiom show the unambiguity of:

$$
a\cdot b\cdot c=(a\cdot b)\cdot c=a\cdot(b\cdot c)
$$

generalized to more than three factors because this implies that the parentheses can be inserted anywhere within such a series of terms, therefore they are usually omitted.

### Uniqueness of identity element

the axioms imply that the identity element is unique; that is, there exists only one identity element: any two identity elements $e$ and $f$ of a group are equal, because the axioms imply:

$$
e=e\cdot f=f
$$

### Uniqueness of inverses

the axioms also imply that the inverse of each element is unique.

let a group element $a$ have both $b$ and $c$ as inverses (where $b$ and $c$ are distinct), then:

$$
\begin{align}
b &= b\cdot e & \text{ ($e$ is the identity element)} \\
&= b\cdot(a\cdot c) & \text{ ($c$ is an inverse)} \\
&= (b\cdot a)\cdot c & \text{ (associativity)} \\
&= e\cdot c & \text{ ($b$ is an inverse)} \\
&= c & \text{ ($e$ is the identity element)} 
\end{align}
$$

therefore, we speak about *the* inverse of an element.

### Division

given elements $a$ and $b$ of a group $G$, there is a unique solution in $x$ in $G$ to the equation $a\cdot x=b$, namely $a^{-1}\cdot b$.

it follows that for each $a$ in $G$, the function $G\rightarrow G$ that maps each $x$ to $a\cdot x$ is a [[Bijection|bijection]]; called
*left multiplication* by $a$ or *left translation* by $a$.

similarly, given $a$ and $b$, the unique solution to $x\cdot a=b$ is $b\cdot a^{-1}$. for each $a$, the function $G\rightarrow G$ that maps each $x$ to $x\cdot a$ is a bijection called *right multiplication* by $a$ or *right translation* by $a$.

## Equivalent definition with relaxed axioms

the group axioms for identity and inverses may be "weakened" or relaxed to show only the existence of a left identity and left inverses. 

however, from just the left side we can prove that the existence of a left identity or left inverse implies the existence of the right identity or right inverse.

assuming associativity and the existence of a left identity $e$ (that is, $e\cdot f=f$) and a left inverse $f^{-1}$ for each element $f$ (that is, $f^{-1}\cdot f=e$), one can show that every left inverse is also a right inverse of the same element:

$$
\begin{align}
f\cdot f^{-1}&=e\cdot(f\cdot f^{-1})&\text{ (left identity)} \\
&=((f^{-1})^{-1}\cdot f^{-1})\cdot(f\cdot f^{-1})&\text{ (left inverse)} \\
&=(f^{-1})^{-1}\cdot((f^{-1}\cdot f)\cdot f^{-1})&\text{ (associativity)} \\
&=(f^{-1})^{-1}\cdot(e\cdot f^{-1})&\text{ (left inverse)} \\
&=(f^{-1})^{-1}\cdot f^{-1}&\text{ (left identity)} \\
&=e&\text{ (left inverse)} \\
\end{align}
$$

similarly, the left identity is also a right identity:

$$
\begin{align}
f\cdot e&=f\cdot(f^{-1}\cdot f)&\text{ (left inverse)} \\
&=(f\cdot f^{-1})\cdot f&\text{ (associativity)} \\
&=e\cdot f&\text{ (right inverse)} \\
&=f&\text{ (left identity)} \\
\end{align}
$$

these proofs require all three axioms (associativity, existence of left identity and existence of left inverse) to hold true. for a structure with a looser definition (such as a [[Semigroup|semigroup]]) you might find that a left identity is not necessarily a right identity,