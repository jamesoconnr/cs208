1. Last term+first term is 430. How many terms are there? Well the difference between each term is 4. So if we subtract the initial term (3) from the last term (427) we get 424. Divide that by 4 and get 106, add 1 for 0th term and get 107. So we do $\dfrac{430*107}{2}$
2. .

    a. Interestingly the sequence starts at $a_{-1}$, so there are $n+2$ terms. 
    
    b. The second to last term is $4(n-1)+6$.

    c. $\dfrac{(4n+6+2)*(n+2)}{2}$

3. . 
    
    a. starting at $a_1$, $2, 10, 50, 250$. Its geometric with a ratio of 5.

    b. Well I should shift over the whole sequence by 1 and create 5S. Then do 5S-S and divide that by 4. So $\dfrac{-2+2*5^{25}}{4}$

4.
5. First diffs are $7, 9, 11$, second are $2, 2$ so its a quadratic. First term is $a_1$ so $a_0=-1=c$ Now we have a system of equations $$5=a+b$$ $$12=4a+2b$$ solve for $2=2a$, $a=1$ and $5=1+b$, $4=b$. Final formula is $a_n=n^2+4n-1$
6. 
    
    a. It will be a 4th degree polynomial

    b. It'll be arithmetic.

7. 

    a. $4, 6, 10, 16, 26, 42$

    b. First diffs are $2, 4, 6, 10, 16$. This is the original sequence so no.

8. $a_n$ diffs are $1, 2, 3, 4$, $b_n$ diffs are $6,8,10,12$. So $b_n-b_{n-1}=2(a_n-a_{n-1})+4$. In theory then, the formula TODO
9.
10. 
    
    a. $1, 2, 16, 68, 364$
    
    b. While i'll use the characteristic root technique. Formula is $r^2-3r-10$, which factors to $r=5, -2$. So $a5^n+b(-2)^n$. $$1=a+b$$ $$2=5a-2b$$ solve for $3=7a$, $\dfrac{3}{7}=a$ and $1=\dfrac{3}{7}+b$, $\dfrac{4}{7}=b$. So formula is $a_n=\dfrac{4}{7}5^2+\dfrac{3}{7}(-2)^2$

11. 

    a. $1, 3, 14, 52$

    b. So we have $r^2-2r-8$ which factors too $r=4, -2$. So we have $a_n=a4^n+b(-2)^n$. The system of equations is $$1=a+b$$ $$3=4a-2b$$ which solves to $5=6a$, $\dfrac{5}{6}=a$ so $\dfrac{1}{6}=b$. So the equation is $a_n=\dfrac{5}{6}4^n+\dfrac{1}{6}(-2)^n$.

12. 

    a. Starting at $a_0$ it is $2, 2, 6, 10$

    b. Recursive definition is $a_n=2(a_{n-2})+a_{n-1}$ with $a_0=2, a_1=2$. This is correct because the large bunnies are the ones which existed two days prior, and multiplying this number by 2 gets you the total # of new bunnies. Then you simply add the bunnies which existed the previous day.

    c. Well I can use characteristic roots so it's $r^2-r-2$ which factors to $r=2, -1$. So we have $a2^n+b(-1)^n$. System of equations is $$2=a+b$$ $$2=2a-b$$ which solves to $4=3a$, $\dfrac{4}{3}=a$ and $-\dfrac{1}{3}=b$. So our formula is $a_n=\dfrac{4}{3}2^n-\dfrac{1}{3}(-1)^n$.

13.
14.
15.
16.
17. **Statement:** Let $P(n)$ be the statement that all sets of n length have $2^n$ subsets so long as $n\geq1$. 
**Base Case:** P(1) is a set that has one length and 2 subsets (one empty and with the one element)
**Inductive Case:** Assume $P(k)$ is true, meaning that set of k elements (${a_1,a_2,...,a_k}$) has $2^k$ subsets. Now we need to prove $P(k+1)$. This will give us the set ${a_1,a_2,...,a_k,a_{k+1}}$. So if we add $a_{k+1}$ to the $P(k)$ set we can do some induction. Now we have added one more element which can be either included or excluded, so we have added two more choices for each subject. Thus we have $2^{k+1}$ subsets, proving our point.