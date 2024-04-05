1. I guess each term is its previous plus double that ones previous. So $a_n=a_{n-1}+2a_{n-2}$. Next terms are 171 and 341. Relation becomes $r^2-r-2=0$, which has roots $r=2, r=-1$ so we have formula $a_n=a(2)^n+b(-1)^n$. $$3=a+b$$ $$5=2a-b$$. $5=2(3-b)-b$, $5=6-3b$, $-1=-3b$, $\dfrac{1}{3}=b$. $3=a+\dfrac{1}{3}$, so $b=\dfrac{8}{3}$. So the formula is $a_n=\dfrac{8}{3}2^n+\dfrac{1}{3}(-1)^n$

2. .

3. To use telescoping we can see that $$a_1-a_0=2^1$$ $$a_2-a_1=2^2$$ $$...$$ $$a_n-a_{n-1}=2^n$$ I multiply another the sequence to shift it over and do $2S-S$ which leaves us with $-2+2^{n+1}$ for the right side and everything on the left cancels out except for $-a_0$ and a $a_n$. So we have $a_n=a_0-2+2^{n+1}$. We know that $a_0=5$, so the formula is just $a_n=3+2^{n+1}$

4. Plug it in and get $a_n=3(4^{n-1})+4(4^{n-2})$. 