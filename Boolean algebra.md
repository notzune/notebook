in mathematics and [[Mathematical logic|mathematical logic]], boolean algebra is a branch of [[Algebra|algebra]] but differs in two ways. firstly, the values of the [[Variables|variables]] are the [[Truth value|truth values]] true and false, denoted 1 and 0 respectively. secondly, boolean algebra uses [[Logical operators|logical operators]] such as [[Logical conjunction|conjunction]] (***and***, denoted as $\wedge$), [[Logical disjunction|disjunction]] (***or***, denoted as $\vee$), and [[Logical negation|negation]] (***not***, denoted as $\neg$).

in boolean algebra, values are represented by [[Bit|bits]] (0 and 1) which do not behave like normal [[Integer|integers]] but instead only contains elements of the [[GF2|two-element field GF(2)]], that is, [[Modular Arithmetic|integer arithmetic modulo 2]], for which $1+1=0$.

addition and multiplication then play the boolean roles of [[XOR]] (exclusive-or) and [[AND]] (conjunction), respectively. 

| Logical  operation | Operator |  Notation   |                         Alternative notations                         |                            Definition                             |
| :----------------: | :------: | :---------: | :-------------------------------------------------------------------: | :---------------------------------------------------------------: |
|    Conjunction     | **AND**  | $x\wedge y$ |               $x\space\text{AND}\space y$, $\text{K}xy$               | $x\wedge y=1\text{ if }x=y=1,\space x\wedge y=0\text{ otherwise}$ |
|    Disjunction     |  **OR**  |  $x\vee y$  |                   $x\text{ OR }y,\space\text{A}xy$                    |   $x\vee y=0\text{ if }x=y=0,\space x\vee y=1\text{ otherwise}$   |
|      Negation      | **NOT**  |  $\neg x$   | $\text{NOT }x,\space\text{N}x,\space\overline{x},\space x',\space !x$ |       $\neg x=0\text{ if }x=1,\space\neg x=1\text{ if }x=0$       |

the values of $x\wedge y, x\vee y,$ and $\neg x$ can also be tabulated into a [[Truth table|truth table]]:

|  $x$  |  $y$  | $x\wedge y$ | $x\vee y$ |
| :---: | :---: | :---------: | :-------: |
| **0** | **0** |      0      |     0     |
| **1** | **0** |      0      |     1     |
| **0** | **1** |      0      |     1     |
| **1** | **1** |      1      |     1     |

| $x$ | $\neg x$ |
| :-: | :------: |
|  0  |    1     |
|  1  |    0     |

## Boolean logic operators

there exists three basic logical operations (also referred to as [[Logic gates|logic gates]]) called [[AND]], [[OR]], and [[NOT]]:

### **AND** 

is represent by a dot or by the absence of an operator symbol; for example $Z=X\cdot Y$ or $Z=XY$. this is read as "$Z$ is equal to $X$ AND $Y$" which is interpreted to mean that $Z=1$ [[if and only if]] $X=1$ AND $Y=1$, otherwise $Z=0$

### OR

represented by a plus symbol (+); for example $Z=X+Y$ which is read "$Z$ is equal to $X$ OR $Y$" which means that $Z=1$ if $X=1$ or if $Y=1$, or if both $X=1$ and $Y=1$. $Z=0$ if and only if both $X=0$ and $Y=0$.

### **NOT**

represented by a bar over the variable for example $\overline{Z}$ (pronounced ***Z-bar***) or $Z=\overline{X}$ which is read as "$Z$ is equal to NOT $X$", simply meaning that $Z$ is whatever $X$ is not therefore if $X=1$, $\overline{X}=0$, therefore $Z=0$ and vice versa. (this is the same concept as a [[Complement|complement]] from [[Set Theory|set theory]], in this case the [[Sets|set]] will always be the $GF(2)$ [[GF2|field]] which contains only the elements $0$ and $1$)