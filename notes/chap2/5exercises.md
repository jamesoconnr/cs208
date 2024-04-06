1. . 
    a. Well every midnight our collection doubles but at 8 we eat 5. Any number ending in 5 doubled will end in a 0, and any number ending in 0 minus 5 will end in 5.
    b. I would need the initial bean count. If the initial bean count is >5 and ends in 5 everything will go according to plan.
    c. Well lets say I start with 15 beans. Day 2 I wake up with 30 beans and after I eat I am left with 25. Day 3 I have 45 and day 4 I have 85. Induction works because I can prove $k+1$ in a very similar manor to example 2.5.2.

2. Statement: P(n) represents the statement that  $\sum_{n=0}^n2^n=2^{k+1}-1$ is true for all $n\geq0$
Base Case: P(0) is $$2^0=2^1-1$$ $$1=1$$
Inductive Case: Assume $P(k)$ is true, that is that $1+2+4+...+2^k=2^{k+1}-1$ is true. Now we need to to prove $P(k+1)$, which is $1+2+4+...+2^{k+1}=2^{k+2}-1$. Now, we know that the difference between $P(k)$ and $P(k+1)$ is $2^{k+1}$. So we add $2^{k+1}$ to left side, meaning we also have to do it to the right. We get $$1+2+4+...2^k+2^{k+1}=2^{k+1}-1+2^{k+1}$$
see here we have two of the $2^{k+1}$ terms. Remember that every time we do $2^n$ we are doubling so $2*2^{k+1}$ is really just $2^{k+2}$, thus our right side becomes $$2^{k+2}-1$$ proving $P(k+1)$ is true.

3. Statement: $P(n)$ represents the statement that $7^n-1$ is a multiple of 6 when n is a natural number
Base Case: $P(0)$ is $7^0-1=1-1=0$ which is a multiple of 6.
Inductive Case: Assume P(k) is true where k is some natural number $>0$. That is, $7^k-1=6j$ where j is some integer. It is advantageous to write $P(k)$ as $7^k=6j+1$. Now we need to prove $P(k+1)$. We know to go up by one k on the left side we should multiply by 7 and subtract 1, so $P(k+1)$ is $7^{k+1}-1=42j+6$, which is equal to $7^{k+1}-1=6(7j+1)$. This proves $P(k+1)$ is multiple of 6.
4. Statement: $P(n)$ represents that $1+3+5+...+(2n-1)=n^2$ is true for all $n\geq1$ 
Base Case: $P(1)$ is $1=1^2$ which is (hopefully) obviously true.
Inductive Case: Assume P(k) is true where k represents some natural numbers. So $P(k)$ is $1+3+5+...+(2k-1)=k^2$. We need to prove $P(k+1)$ which is $1+3+5+...+(2(k+1)-1)=(k+1)^2$. We know then that to get $P(k+1)$ on the left side we must add $(2(k+1)-1)$ so we get $$1+3+5+...+(2k-1)+(2(k+1)-1)=k^2+(2(k+1)-1)$$
$$=k^2+2k+1$$
$$=(k+1)^2$$ 
thus $P(k+1)$ is true.
5. TODO
6. TODO
7. 
8.
9.
10.
11.
12. TODO
13. TODO
14.
15.
16. TODO
17.
18.
19. TODO
20.
21.
22.
23.
24.
25. TODO