# Binomial Coefficients
- If we have set A which is {1, 2, 3, 4, 5}, there are 32 subsets. We know this because all 5 numbers can either be included or excluded from a subset, so there are 2 possibilities for every number. So $\mathcal{P} (\mathbb{A}) = 2^5$
- Finding how many sets have 3 items is more complicated. You can do $5 * 4 * 3$, representing 5 options for the first item, 4 for the second, etc., however this equal 60, which is > 32. This is because the 60 includes repeating sets. We know there are 6 possibilities for the order of 3 item subsets because $3 * 2 * 1$. Using this, we can divide 60 by 6 to find that there are 10 3 item subsets of A.
- When seeing how many subsets of A exist of cardinality x you encounter a symmetrical pattern (shown below). This is because saying no to two elements can be done in the same number of ways as saying no to two elements.

|0|1|2|3|4|5|
|-|-|-|-|-|-|
|1|5|10|10|5|1|
## bit strings
- A bit string is a string of bits. The length is the # of bits and the weight is the # of 1s. A set of bit strings is represented as either $B^n$ or $B^n_k$ with n representing length and k represent weight.
- so $B^2_1 = \{01, 10 \}$
- Finding the number of 5-bit strings is easy, it's $5^2$
- Finding the number of 5-bit strings with weight 3 is way harder
    - first bit is either 1 or 0 so there can be either 2 or 3 ones in the remaining 4. S basically $|B^5_3| = |B^4_3| + |B^4_2|$
    - Now we can do the same to those two
    $$|B^4_3| = |B^3_3| + |B^3_2|$$
    $$|B^4_2| = |B^3_2| + |B^3_1|$$
    - From there we can deduce $|B^3_3| = 1$ and that $|B^3_2| = 3$, so $|B^4_3| = 4$
    - With $|B^3_1| = 3$ we can also conclude that $|B^4_2| = 6$
    - So, $|B^5_3| = 6 + 4 = 10$
- overall the bit string problem is like the subset problem and the ones represent numbers included in a given subset
## lattice paths
- Integer lattices are graphs where x and y are integers, so instead of curved/sloped lines they are straight and move at 90 degree turns. It looks like snake
- Lattice path is the shortest possible path on integer lattice. Possible means to the right and up
- If movement is represented as R and U we essentially have a bit-string
- If a R = 1 and U = 0 the lattice paths between 0,0 and 3,2 can be represented as $|B^5_3|$
## binomial coefficients
- binomial coefficients are the repeating numbers seen in the previous problems
- symbol is $\binom{n}{k}$
- it's number of ways to select k items from n objects