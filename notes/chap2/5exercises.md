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
5. **Statement:** $P(n)$ is the statement that $F_0+F_2+F_4+...+F_{2n}=F_{2n+1}-1$ is true when n is a natural number.
**Base Case:** $P(0)$ is $$F_0+F_{0}=F_{2(0)+1}-1$$ $$0=F_1-1$$ $$0=1-1$$ $$0=0$$
**Inductive Case:** Assume $P(k)$, as in $F_0+F_2+F_4+...+F_{2k}=F_{2k+1}-1$, is true. We know to increase the index of the fibonacci number on the right by one, so to prove $P(k+1)$ we can can add $F_2k+2$. $$F_0+F_2+F_4+...+F_{2k}+F_{2k+2}=F_{2k+1}-1+F_{2k+2}$$ Now note that two sequential fibonacci numbers added is the next fibonacci number $$F_0+F_2+F_4+...+F_{2k}+F_{2k+2}=F_{2k+3}-1$$ now we can see that the right side has the last term on the left plus one just like $P(k)$, meaning this is true.

6. **Statement:** $P(n)$ is the statement that $2^n<n!$ is true for all $n\geq4$
**Base Case:** $P(4)$ is $$2^4<4!$$ $$16<14$$
**Inductive Case:** Assume $P(k)$, as in $2^k<k!$, is true. We want to prove $P(k+1)$, or $2^{k+1}=(k+1)!$ To get $P(k+1)$ we can multiply $P(k)$ by 2 because for each n the left side doubles $$2^{k+1}<2*k!$$ I need to come back to this TODO. How does the 2 magically become a $(k+1)$?

7. 

8.

9.

10.

11.

12. There is no base case and ideally they would have written out $P(k+1)$ first.

13. **Statement:** Let $P(n)$ be the statement that $n+3<n+7$ for all $n\in\mathbb{n}$. 
**Base Case:** $P(0)$ is $$0+3<0+7$$ $$3<7$$
**Inductive Case:** Assume $P(k)$, as in $k+3<k+7$ is true. We want to prove $P(k+1)$, or $(k+1)+3<(k+1)+7$. If we add 1 to both sides of $P(k)$ we get $$k+3+1<k+7+1$$ $$(k+1)+3<(k+1)+7$$ so $P(k+1)$ is true.

14. It is clearly only true up to 99.

15.

16.  There is no base case.

17.

18.

19. **Statement:** Let $P(n)$ be the statement that n, a positive integer, is either a power of 2 or can be written as the sum of two distinct powers of 2. 
**Base Case:** $P(1) is $2^0$
**Inductive Case:** Assume $P(k)$ is true for all $k < n$ with n being an arbitrary integer. If n is a power of 2, then we have proved our case. If not let $2^x$ be the largest power of 2 less than n. Now think about $n-2^x$. This number is smaller than both n and $2^x$. So then it is the sum of two distinct powers of two.

20.

21.

22.

23.

24.

25. **Statement:** Let $P(n)$ be the statement that $log(a^n)=n*log(a)$ for all natural numbers greater than two.
**Base Case:** $P(2)$ is $$log(a^2)=2log(a)$$ $$log(a*a)=2log(a)$$ $$log(a)+log(a)=2log(a)$$ $$2log(a)=2log(a)$$
**Inductive Case:** Suppose $P(k)$, as in $log(a^k)=klog(a)$, is true. We must prove $P(k+1)$, or $log(a^{k+1})=(k+1)log(a)$. Well using the product rule I know I can get $a^{k+1}$ on the left side by adding $log(a)$. $$log(a^k)+log(a)=klog(a)+log(a)$$ $$log(a^{k+1})=(k+1)log(a)$$ meaning it is true.