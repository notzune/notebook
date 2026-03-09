in mathematics and [[Combinatorics|combinatorics]], a combination is a selection of items from a [[Sets|set]] that has distinct [[Element|members]], such that the order of selection does not matter (unlike [[Permutation|permutations]] where the order plays a role).

see also: [[Binomial coefficient|binomial coefficient]]

a combination of $k$ objects from $n$ objects ($n\geq k$) is an unordered collection of $k$ objects selected [[Replacement|without replacement]] (without repetition) from the group of $n$ objects.

the number of possible combinations of $k$ objects from $n$ objects is

$$
C^n_k=\binom{n}{k}=\frac{n!}{(n-k)!\space k!}
$$

if the set has $n$ elements, the number of $k$-combinations (denoted by $C(n,k)$ or $C^n_k$) is equal to the [[Binomial coefficient|binomial coefficient]].

combinations with replacement (in which repetition is allowed) would be referred to as $k$-combination with repetition, or $k$-[[Multiset|multiset]].

## Shortcuts

$$
\begin{align}
C^n_1&=\binom{n}{1}=\frac{n!}{(n-1)!\space1!}=n \\
\\
C^n_2&=\binom{n}{2}=\frac{n!}{(n-2)!\space2!}=\frac{n(n-1)}{2} \\
\\
C^n_{n-1}&=\binom{n}{n-1}=\frac{n!}{1!\space(n-1)!}=n \\
\\
C^n_n&=\binom{n}{n}=\frac{n!}{0!\space n!}=1
\end{align}
$$

## Example problems

### Example 1
suppose that in a taste test, each participant samples eight products and is asked to select the three best products, but not in any particular order. the possible answers to the test then

$$
\binom{8}{3}=\frac{8!}{5!\space3!}=\frac{8\times7\times6}{3\times2\times1}=56
$$

### Example 2
suppose that 9 out of 500 chips in a particular box are defective, and that 3 chips are sampled at random from the box without replacement. the total number of possible samples is

$$
\binom{500}{3}=\frac{500!}{497!\space3!}=\frac{500\times499\times498}{3\times2\times1}=20,708,500
$$

the [[Probability|probability]] of choosing 3 defective chips can be calculated by dividing the number of samples that contain 3 defective chips by the total number of samples. since there are 9 defective chips, the number of samples that contain 3 defective chips is

$$
\binom{9}{3}=\frac{9!}{6!\space3!}=\frac{9\times8\times7}{3\times2\times1}=84
$$

so the probability of choosing 3 defective chips is

$$
\frac{\binom{9}{3}}{\binom{500}{3}}=\frac{(\frac{9!}{6!\space3!})}{(\frac{500!}{497!\space3!})}=\frac{9\times8\times7}{500\times499\times498}\approx4.0\times10^{-6}
$$

the number of samples that contain exactly 1 defective chip is

$$
9\times\binom{491}{2}
$$

because we have 9 ways to choose 1 defective chip (since there are 9 defective chips), and we have $\binom{491}{2}$ ways to chose 2 non-defective chips from the 491 non-defective chips from the total 500 chips.

the probability of only choosing one defective chip is then

$$
\frac{9\times\binom{491}{2}}{\binom{500}{3}}=\frac{(9\times\frac{491!}{489!\space2!})}{(\frac{500!}{497!\space3!})}=\frac{9\times491\times490\times3}{500\times499\times498}=0.0522
$$

these calculations are an example of the [[Hypergeometric distribution|hypergeometric distribution]].