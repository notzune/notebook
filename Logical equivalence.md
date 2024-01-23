in [[Logic|logic]] and math, statements $p$ and $q$ are said to be logically equivalent if they have the same [[Truth value|truth value]] in every [[Mathematical structure|model]]. the logical equivalence of $p$ and $q$ is sometimes expressed as:

$$
p\equiv q
$$

## General logical equivalences

| *Equivalence* | _Name_ |
| ---- | ---- |
| $p\wedge\top\equiv p$<br>$p\vee\bot\equiv p$ | [[Identity element\|Identity laws]] |
| $p\vee\top\equiv\top$<br>$p\wedge\bot\equiv\bot$ | [[Domination laws]] |
| $p\wedge p\equiv p$<br>$p\wedge p\equiv p$ | [[Idempotent]] or tautology laws |
| $\neg(\neg p)\equiv p$ | [[Double negation law]] |
| $p\vee q\equiv q\vee p$<br>$p\wedge q\equiv q\wedge p$ | [[Commutative property\|Commutative laws]] |
| $(p\vee q)\vee r\equiv p\vee(q\vee r)$<br>$(p\wedge q)\wedge r\equiv p\wedge(q\wedge r)$ | [[Associative property\|Associative laws]] |
| $p\vee(q\wedge r)\equiv(p\vee q)\wedge (p\vee r)$<br>$p\wedge(q\vee r)\equiv(p\wedge q)\vee (p\wedge r)$ | [[Distributive property\|Distributive laws]] |
| $\neg(p\wedge q)\equiv\neg p\vee\neg q$<br>$\neg(p\vee q)\equiv\neg p\wedge\neg q$ | [[De Morgan's Laws]] |
| $p\vee(p\wedge q)\equiv p$<br>$p\wedge(p\vee q)\equiv p$ | [[Absorption law\|Absorption laws]] |
| $p\vee\neg p\equiv\top$<br>$p\wedge\neg p\equiv\bot$ | [[Negation laws]] |
### In [[Conditional statement|conditional statements]]

1. $p\implies q\equiv\neg p\vee q$
2. $p\implies q\equiv\neg q\implies\neg p$
3. $p\vee q\equiv\neg p\implies q$
4. $p\wedge q\equiv\ p\implies q$
5. $p\wedge q\equiv\neg(p\implies\neg q)$
6. $(p\implies q)\wedge(p\implies r)\equiv p\implies(q\wedge r)$
7. $(p\implies q)\vee(p\implies r)\equiv p\implies(q\vee r)$
8. $(p\implies r)\wedge(q\implies r)\equiv(p\vee q)\implies r$
9. $(p\implies r)\vee(q\implies r)\equiv(p\wedge q)\implies r$

### In equivalences involving biconditionals

1. $p\iff q\equiv(p\implies q)\wedge(q\implies p)$
2. $p\iff q\equiv\neg p\iff\neg q$
3. $p\iff q\equiv(p\wedge q)\vee(\neg p\wedge\neg q)$
4. $\neg(p\iff q)\equiv p\iff\neg q$


   