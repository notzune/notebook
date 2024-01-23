in applied mathematics, a bit-reversal permutation is a [[Permutation|permutation]] of a [[Sequence|sequence]] of $n$ items, where $n=2^k$ is a [[Power of two|power of two]].

it is defined by indexing the [[Element|elements]] of the sequence by the numbers from $0$ to $n-1$, representing each of these numbers by its [[Binary number|binary representation]] (padded to have length exactly $k$), and mapping each item to the item whose representation has the same [[Bit|bits]] in the reversed order.

repeating the same permutation twice returns to the original ordering on the items, so the bit reversal permutation is an [[Involution|involution]].

this permutation can be applied to any sequence in [[Time complexity|linear time]] while performing only simple index calculations.

## Example

consider the sequence of eight letters *"abcdefgh"*. their indexes are the binary numbers 000, 001, 010, 011, 100, 101, 110, and 111, which when reversed become 000, 100, 010, 110, 001, 101, 011, and 111. 

thus, the letter a in position 000 is mapped to the same position (000), the letter b in position 001 is mapped to the fifth position (the one numbered 100), etc., giving the new sequence *"aecgbfdh"*. 

repeating the same permutation on this new sequence returns to the starting sequence.

writing the index numbers in decimal (but, as above, starting with position 0 rather than the more conventional start of 1 for a permutation), the bit-reversal permutations on $n=2^k$ items, for $k=0,1,2,3,\dots,$ are:

| k | $n=2^k$ | permutation |
| ---- | ---- | ---- |
| 0 | 1 | 0 |
| 1 | 2 | 0 1 |
| 2 | 4 | 0 2 1 3 |
| 3 | 8 | 0 4 2 6 1 5 3 7 |
| 4 | 16 | 0 8 4 12 2 10 6 14 1 9 5 13 3 11 7 15 |