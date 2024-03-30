1. .
	
	a. $a_n = a_{n-1} + 5$ with $a_0 = 0$

	b. $a_n = 5 + 4(n -1)$

	c. Yes it's the 504th (add 1 one for 0th term) term because $2013 = 5+4(n-1)$, $2008 = 4(n-1)$, $502 = n-1$, $503 = n$

	d. There are 133 terms because $533 = 5+4(n-1)$, $528 = 4(n-1)$, $132 = n-1$, $133 = n$

	e. Well $5+533=538$ so we can do $538*133$ and divide that by $2$ and get $3577$

	f. $b_n = 1+\dfrac{n(4n+6)}{2}$

2. . 

	a. $32$

	b. $a_n = 8 + 6n$

	c. $a_1 = 8$ and $a_{99} = 602$, so we do $\dfrac{610*100}{2}$ which is $30500$

3. . 

	a. Well the recursive formula (assuming this starts at 0) is $4+7n$ so $249=4+7n$, $245=7n$, $35 = n$, so there are 36 terms

	b. $\dfrac{253*36}{2}=4554$

4. . 

	a. I suppose we have $n+2$ terms because we have to start at $n = -1$ for it to work

	b. $6n -1$

	c. $\dfrac{(1+6n+7)*n+2}{2}$

5. diff is two every time, so formula is $a_n = 2n+5$. $521 = 2n+5$, $516=2n$, $n=258$. There are 259 terms, so ill do $\dfrac{(5+521)*259}{2} = 68117$

6. method used in 5 and others didn't work for me. Instead find a recursive relation, in this case $a_n = a_{n-1}*3$ and apply it to S (original sequence) to "shift" it over one to the right (i.e. $a_0=15$ now instead of $5$). Now simply subtract 3S from S to be left with -2S. All terms execept for first S and last of 3S cancel out, so you are left with $5-5*3^{21}=-2S$. We want S so we divide by -2 to get $S=\dfrac{-5+5*3^{21}}{2}$

7. This one is very confusing, why do the signs flop back and forth. Either way, we use the method shown in 6 and multiply everyting by $\dfrac{2}{3}$ for $\dfrac{2}{3}2$. Because of the alternating signs, we add it to $S$. $\dfrac{5}{3}S = 1+\dfrac{2^{31}}{3^{31}}$, divide by $\dfrac{5}{3}$ and get $S = \dfrac{1+\dfrac{2^{31}}{3^{31}}}{\dfrac{5}{3}}$

8. .
	a. So its asking what can be subtracted from 27 twice to get 1. $27-1=26$ so $\dfrac{26}{3}$ is our difference. $x = \dfrac{55}{3} \ and \ y = \dfrac{29}{3}$

	b. With d being ratio we have $27*d^3=1$, $d^3=\dfrac{1}{27}$, $d=\dfrac{1}{3}$. $x = 9, y = 4$

9. .
	
	a. Well $5-32=27$ and $\dfrac{27}{3}=9$, so $d=0$. $x=14, y=23$

	b. Our first term is 5 and we know that the last term times 3 of the ratio (r) must be the last term (32). So, mathematically, $5*r^3=32$, $r^3=\dfrac{32}{5}$, $r=\sqrt[3]{\dfrac{32}{5}}$. Im not going to calculate the actual answers but $x=5*\sqrt[3]{\dfrac{32}{5}}$, $x=5*(\sqrt[3]{\dfrac{32}{5}})^2$

10.

11. The differences are $5, 8, 11, 14$, and we can see the difference increases by 3 every time. So we can express this as a sequence of partial sums, $a_n = 2 + 5 + 11 + 14 + ... + (2 + 3n)$. Reverse and add yada yada you get $\dfrac{(4+3n)(n+1)}{2}$