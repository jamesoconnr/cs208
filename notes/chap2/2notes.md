- If the terms of a sequence differ  by a constant amount then it's arithmetic
- a is the initial term and the common difference is d
- for example $a_n = a_{n-1}+d, a_0 = a$ or $a_n = a + dn$
- [cool example on finding formulas without actual numbers](https://discrete.openmathbooks.org/dmoi3/sec_seq-arithgeom.html#:~:text=We%20see%20that,times.%20Thus)
- A sequence where the ratio of the difference between terms is constant is called geometric
- with r as the ratio and as the initial term a base geometric formula would be $a_n = a \cdot r^n$
- **a is always $a_0$**
- When you are creating a sequence that is summing up to n of another sequence you are making a sequence of partial sums
- If wanted to find the sum of the first 100 integers you could regroup and do $100 + 1 = 101$, $2 +99 = 101$, etc. and you would find that you would have found 50 101s. So in short, you could have done $101*50$
- > Find the sum $2 + 5 + 8 + 11 + 14 + ... + 470$

    Approaching this like the above problem, $2+470=472$. Now we just need to add 472 to itself for however many terms there are the in the sequence. If we find the formula as $2+3n$ and set it equal to our final term, making it $2+3n=470$, we can find n is equal to 156 meaning there are 157 terms in the sequence (1 for 0th term). So twice the sum ([see explanation here](https://discrete.openmathbooks.org/dmoi3/sec_seq-arithgeom.html#:~:text=472-,To%20find,We%20need%20to%20decide%20how%20many%20terms%20(summands)%20are%20in,-the%20sum.%20Since))is $157*472=74104$, meaning the sum is $37052$
- > Find a closed formula for $6+10+14+...+(4n-2)$

    This is also another arithmetic sequence, with a formula of $4n-2$. The instance above starts at $n=2$. Adding the first and last terms give you $4n+4$ and there are $n-1$ terms so $2S = (n-1)(4n+4)$ and $S=\dfrac{(n-1)(4n+4)}{2}$

- > What is $3+6+12+24+...+12288$ (geometric sequence)?

    Multiply each term by the common ratio, in this case two. Then subtract S from 2S and you'll be left with $-3+24576=24573$, or S.