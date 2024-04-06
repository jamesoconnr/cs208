1. . 
    a. Well every midnight our collection doubles but at 8 we eat 5. Any number ending in 5 doubled will end in a 0, and any number ending in 0 minus 5 will end in 5.
    b. I would need the initial bean count. If the initial bean count is >5 and ends in 5 everything will go according to plan.
    c. Well lets say I start with 15 beans. Day 2 I wake up with 30 beans and after I eat I am left with 25. Day 3 I have 45 and day 4 I have 85. Induction works because I can prove $k+1$ in a very similar manor to example 2.5.2.

2. Statement: P(n) represents the statement that  $\sum_{n=0}^n2^n=2^{k+1}-1$ is true for all $n\geq0$
Base Case: P(0) is $$2^0=2^1-1$$ $$1=1$$
Inductive Case: Assume $P(k)$ is true, that is that $1+2+4+...+2^k=2^{k+1}-1$ is true. Now we need to to prove $P(k+1)$, which is $1+2+4+...+2^{k+1}=2^{k+2}-1$. Now, we know that the difference between $P(k)$ and $P(k+1)$ is $2^{k+1}$. So we add $2^{k+1}$ to left side, meaning we also have to do it to the right. We get $$1+2+4+...2^k+2^{k+1}=2^{k+1}-1+2^{k+1}$$
see here we have two of the $2^{k+1}$ terms. Remember that every time we do $2^n$ we are doubling so $2*2^{k+1}$ is really just $2^{k+2}$, thus our right side becomes $$2^{k+2}-1$$ proving $P(k+1)$ is true.

