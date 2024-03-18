1. .

	a. Everything is a square + 1 so we have $a_n = n^2 + 1$

	b. This looks like triangular numbers - 1 so $a_n = \dfrac{n(n+1)}{2} - 1$

	c. These are triangular numbers +2 starting at 6, so its $a_n = \dfrac{(n+2)(n+3)}{2} + 2$

	d. Its factorials - 1 and seemingly starting at 2. $a_n = (n+1)-1$ 
2. .

	a. This is a tough one. The between numbers doubles everytime, but writing this out would be recursive. The difference between triangular numbers also doubles everytime. Its just triangles numbers + 4 so $\dfrac{n(n+1)}{2} + 4$
	
	b. The differences are 3, 5, 7, 9, 11, they start at 3 and increase by 2 everytime. We this same pattern in in square numbers so this one is but this one is one position left and down one. So its $a_n = (n + 1)^2 - 1$.

	c. Once again the difference is increasing by 2 every time, so I recognize this as some sort of square number sequence. I think it is $(n+3)^2 - 3 - 1n$

	d. Very confusing. No discernable patter in the plain numbers or the difference between them. I will come back to this.

3. .

	a. 0, 1, 3, 6, 10. $a_n = a_{n-1} + n$ given $a_0 = 0$

	b. 0, 1, 2, 3, 4. $a_n = n$

	c. 1, 1, 2, 6, 24. $a_n = n!$
4. .

	a. recursive is $a_n = a_{n-1} + 2$ with $a_0 = 1$. The closed formula is $a_n = 2n - 1$.

	b. 4, 9, 16, 25 ... or recursively $b_n = b_{n-1} + a_n$ with $a_n = 2n - 1$. It looks like squares to me so the closed formula is $b_n = n^2$
5. .

	a. 0, 1, 2, 4, 7, 12, 20, 33

	b. Seemingly it is $F_{n+2}$

6. Assuming these all start at $ a_0 $ ...

	a. $a_n = a_{n-2} + a_n{n-1}$ with $a_0 = 2, a_1 = 4$. I am putting in my guess that they will all be fibonacci
	b. I am correct. $a_n = a_{n-2} + a_n{n-1}$ with $a_0 = 5, a_1 = 6$ 
	c. $a_n = a_{n-2} + a_n{n-1}$ with $a_0 = 0, a_1 = 0$

7. 3, 10, 24, 52, 108 ... . The second sequence the same damn sequence as the first one so its $a_n = 2a_{n-1} + 4$ with $a_1 = 10$

8. 1, -1, -1, 1, 5, 11. Closed formula for the second set is $a_n = n^2 - n$. Answering is just yapping my formula works

9. Ill start by writing out some of $a_n$ starting at $a_0$: $$ 10, 41, 187, 899 $$
Now time to test it out on $a_3$, which when plugged in is $$7(41) - 10(10)$$ which does equal 187 or $a_3$. So the initial conditions needed are $a_0 = 10$ and $a_1 = 41$

10. Ill start by writing out some of $a_n$ starting at $a_0$ just like in 9: $$ 0, -3, -21, -17 $$ Testing out $a_2$ with the recurrence relation is $7(-3) - 10(0)$ which is indeed equal to $-21$. Initial conditions needed are $a_0 = 0, a_1 = -3$

11. First few terms are $1, 2, 3, 4$. I can count so I can see the formula is $a_n = n$

12. .

13. . just imagine the latex works and you see summations symbols and stuff

	a. $ \displaystyle\sum_{k=1}^n {2k} $

	b. $ \displaystyle\sum_{k=1}^{107} {1+4(k-1)} $

	c. $ \displaystyle\sum_{k=1}^{50} {\dfrac{1}{k}} $

	d. $ \displaystyle\prod_{k=1}^n {2k} $

	e. $ \displaystyle\prod_{k=1}^{101} {\dfrac{k}{k+1}} $

14. .

	a. 7 + 11 + 15 + ... + 403

	b. 1 + 2 + 4 + 8 + ... + $2^n$

	c. $1 + \dfrac{1}{3} + \dfrac{1}{8} + \dfrac{1}{15} + ... + \dfrac{1}{2499}$ 

	d. $\dfrac{4}{3} * \dfrac{9}{8} * \dfrac{16}{15} * ... * \dfrac{10000}{9999}$

	e. $2 * 5 * 8 * ... * 2+3n$

15.

16.

17. ***Consider bit strings with length l and weight k (so strings of l 0’s and 1’s, including k 1’s). We know how to count the number of these for a fixed l and k. Now, we will count the number of strings for which the sum of the length and the weight is fixed. For example, let’s count all the bit strings for which l + k = 11***
	
	a. ***Find examples of these strings of different lengths. What is the longest string possible? What is the shortest?***

	The longest string is $l = 11, k = 0$. The shortest is $l = 6, k = 5$

	b. ***How many strings are there of each of these lengths. Use this to count the total number of strings (with sum 11)***
 
 	There are ${11 \choose 0}$ and ${6 \choose 5}$ of these, respectively. So we just fill in the blanks and get the sum by doing: $${11 \choose 0}+{10 \choose 1}+{9 \choose 2}+{8 \choose 3}+{7 \choose 4}+{6 \choose 5} = 144$$

	c. ***The other approach: Let l + k = n vary. How many strings have sum n = 1? How many have sum 2? And so on. Find and explain a recurrence relation for the sequence which gives the number of strings with sum n?***

	Well making this into a sequence, the first few terms, starting at $a_1$, are 1, 2, 3, 5, 8, 13, 21. i see the pattern. A recursive formula is difficult to find here but I think it's $a_n = a_{n-1} + a_n{n-2}$ with $a_1 = 1, a_2 = 2$

	d. ***Describe what you have found above in terms of Pascal's Triangle. What pattern have you discovered?***

	$a_n$ in this case follows the same rule as pascal's triangle  where two numbers in the same row add up to the number below them. Here, $a_1 + a_2 = a_3$, $a_3 + a_4 = a_5$, and so on. This pattern happens indefinitely.

![pattern](https://github.com/thirdball/csc208/blob/main/ch2_sequences/17d.png)
