1. I guess each term is its previous plus double that ones previous. So $a_n=a_{n-1}+2a_{n-2}$. Next terms are 171 and 341. Relation becomes $r^2-r-2=0$, which has roots $r=2, r=-1$ so we have formula $a_n=a(2)^n+b(-1)^n$. $$3=a+b$$ $$5=2a-b$$. $5=2(3-b)-b$, $5=6-3b$, $-1=-3b$, $\dfrac{1}{3}=b$. $3=a+\dfrac{1}{3}$, so $b=\dfrac{8}{3}$. So the formula is $a_n=\dfrac{8}{3}2^n+\dfrac{1}{3}(-1)^n$

2. .

3. To use telescoping we can see that $$a_1-a_0=2^1$$ $$a_2-a_1=2^2$$ $$...$$ $$a_n-a_{n-1}=2^n$$ I multiply another the sequence to shift it over and do $2S-S$ which leaves us with $-2+2^{n+1}$ for the right side and everything on the left cancels out except for $-a_0$ and a $a_n$. So we have $a_n=a_0-2+2^{n+1}$. We know that $a_0=5$, so the formula is just $a_n=3+2^{n+1}$

4. Plug it in and get $$4^n=3(4^{n-1})+4(4^{n-2})$$ $$4^n=12^{n}+16^{n-1}$$ TODO

5. Im gonna use characteristic roots. So ill move everything to the left side and plug in $r^n$, so it's $$r^n-3r^{n-1}-4r^{n-2}=0$$ $$r^{n-2}(r^2-3r-4)=0$$ so now we can see that $r=4, r=-1, r=0$. Se we know that for some $a, b$ $a_n=a4^n+b(-1)^n$. Plug in the initial values to get $$2=a+b$$ $$3=4a-b$$ so we can solve this system of equations and get $a=1$ and $b=1$ so the equation is $a_n=4^n+(-1)^n$

6. Its the same as #5 but with different initial conditions, so ill just find the new a and b values. $$5=a+b$$ $$8=4a-b$$ solve the system for $a=\frac{13}{5}$ and $b=\frac{12}{5}$ and get the formula of $a_n=\frac{13}{5}4^n+\frac{12}{5}(-1)^n$

7. So im gonna end up with $r^2-3r-10r$, which means $r=5, r=-2$ and $a_n=a5^n+b(-2)^n$. plug in initial conditions to get $$4=a+b$$ $$1=5a-2b$$. Solve to get $\frac{9}{7}=a$ and $b=\frac{19}{7}$. Formula is $a_n=\frac{9}{7}5^n+\frac{19}{7}(-2)^n$

8.

9.

10. .

    a. I have no idea, TODO.

11. 

12. . 

    a. Using characteristic roots ts gonna become $r^2-2r+1$, which factors to $r=1$ multiplicity two. So we the other formula $a_n=a+bn$ (no r because $1^n$ is always 1). So $$1=a+b(0)$$ $$2=a+b$$. So $a=1, b=1$ and the formula is $a_n=1+n$

    b. Well I mean it just needs to start from a later position so I guess $a_0=21, a_1=22$

    c. All natural numbers greater than 9. Solution includes negative but I thought we were working in only natural numbers.