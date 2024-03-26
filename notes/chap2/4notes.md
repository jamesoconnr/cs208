- Investigate!
    
    1. $1, 2, 4, 8, 16$, so clearly the the numbers is double the previous. This is just the powers of two, $a_n=2^n$

    2. $1, 3, 9, 27$ So now it triples every time. $a_n=3^n$

    3. $2, 5, 13, 35, 97$ i don't see a pattern.

- Example 2.4.1

    1. diffs are $4, 12, 36$, multiplying by 3 everytime. $a_n=3a_{n-1}+2$ with $a_0=1$

- Example 2.4.2

    1. They both produce the sequence $3, 5, 9, ...$. Supposedly you can plug in and simplify, but i don't understand step two
    $$2a_{n-1}-1=2(2^{n-1}+1)-1$$
    $$=2^n+2-1$$
    $$=2^n+1$$
    $$a_n$$

- Telescoping is when many terms in a large sum cancel out $$(2-1) + (3-2) + (4-3) + ... + (100-99) + (101-100) = -1 + 101$$

- Example 2.4.3

    1. first few terms are $4, 5, 7, 10, 14, 19$. I did not understand this, [solution here is a good explanation](https://discrete.openmathbooks.org/dmoi3/sec_recurrence.html#:~:text=%F0%9F%94%97-,Example%202.4.3.,-Solve%20the%20recurrence)

- Above example solving method only works when recurrence relations are written like $a_n=a_n{n-1}+f(n)$ and the closed formula for the sum (in the above it is $\dfrac{n(n+1)}{2}$ because the difference between terms is $1,2,3,...$)

- Telescoping will not work on all recurrence relations, like $a_n=3a_{n-1}+2$. Instead iterate

- Iteration is when you plug in (iterate) terms until have $a_n$.

- Example 2.4.4

    1. So we iterate by plugging values starting at $n=1$
    $$a_1=a_0+1 $$
    $$a_2=(a_0+1)+2 $$
    $$a_3=((a_0+1)+2)+3 $$
    by now you may see this pattern
    $$a_n=((a_0+1)+...+n-1)+n$$ 
    and we know $a_0=4$, and that summing natural numbers up to $n$ is $\dfrac{n(n+1)}{2}$, so we really just have $$a_n=4+\dfrac{n(n+1)}{2}$$

- Example 2.4.5

    1. Well ill try iteration
    $$a_1=3a_0+2$$
    $$a_2=3(3a_0+2)+2$$
    $$a_3=3(3(3a_0+2)+2)+2$$
    i don't see a pattern so im going to simplify 
    $$a_1=3a_0+2$$
    $$a_2=3^2a_0+2*3+2$$
    $$a_3=3^3a_0+2*3^2+2*3+2$$
    a pattern is visible
    $$a_n=3^na_0+2*3^{n-1}+...+2*3+2$$
   Because $a_0=1$ we have $3^n$ and then just a sum of $2+2*3+2*3^2+...+2*3*n-1$. Use [this](https://discrete.openmathbooks.org/dmoi3/sec_seq-arithgeom.html#:~:text=%F0%9F%94%97-,Example%202.2.7.,-What%20is) to find that it is equal to $3n-1$. Formula is then just $3_n+3_n-1$ or $2*3_n-1$