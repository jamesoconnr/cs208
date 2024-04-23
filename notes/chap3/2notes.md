- Investigate: I only know induction so I'll say that 4 is right because it kinda looks like induction and it makes sense.
- I do not understanding the prime proof, TODO
- You can prove something by contradiction
- A direct proof is a simple proof in which you assume one thing is true and explain how that proves the other
- Example 3.2.2:
    wheel assuming $n$ is even the it is equal to some $2m$. Se if we square this we get $4k^2$, which can be factored to $2(2k^2)$, which is even
- Example 3.2.3:
    Assume $a|b$ and $b|c$. so $b=na$ for some int n and $c=mb$ for some int m. in other words $c=mna$ and because m and n are ints mn is one too, meaning that c is a multiple of a
- A proof by contrapositive is when you prove a statements contrapostive, as $p\implies q = \neg q \implies \neg p$. The actual structure of a proof by contrapositive is similar to that of a direct proof (assume a, explain, therefore b)
- Example 3.2.4:
    Taking the contrapositive we need to prove that if n is odd then $n^2$ is odd. Assume n is odd, that $n=2k+1$ for some int k. Square that and get $4k^2+4k+1$, which we can factor to $2(2k^2+2k)+2$. $2k^2+2k$ is an integer, so we see that $n^2$ is even. 
- Example 3.2.5:
    Contrapositive is if a and b are even a+ b is even. Assume a and b are even,  $a=2k$ and $b=2j$. Add $2k+2j$ and factor out 2 for $2(k+j)$. Because $k+j$ is an int $2(k+j)$ is even. 
- Example 3.2.6:
    p is a prime number and is not odd, meaning it is divisible by 2. Prime numbers only have 2 divisors, one of which is 2 here. One prime divisor is always 1 and the other is always the number, so 2 must be the number.
- Not all statement can be written as implications. So if we want to prove p, when prove that $\neg p \implies q$ where q is false. This implies that $\neg p$ is false, meaning that p is true. This is proof by contradiction
- Example 3.2.7:
    Assume that $\sqrt{2}$ is rational. Then it is equal to $\dfrac{a}{b}$, which is in the lowest terms. SO $2=\dfrac{a^2}{b^2}$. So multiplying both sides by $b^2$ you get $2b^2=a^2$. Now $b^2$ is an int we know that $a^2$ is even and thus a is even. So $a=2k$ for some int k. So plugging that into the original equation we get $2b^2=4k^2$, which is equal to $b^2=2k^2$ meaning that $b^2$ and b are even. So if both a and b are even then $\dfrac{a}{b}$ is not in the simplest terms, contradicting our argument and prove $\sqrt{2}$ is irrational.
- Example 3.2.8:
    Assume that $x^2=4y+2$. You can factor out 2 on the left side, so $x^2$ and x are even. So we know that $x=2k$. Plug this back in and get $2k^2=2y+1$. This is false as the left is even and the right is odd, therefore proving the original argument by contradiction
- Example 3.2.9:
    Assume each pigeonhole only can hold one pigeon. If there are n pigeonholes and $>n$ pigeons, then either the pigeonholes must hold more than one pigeon or some pigeons must be holeless.
- Very rarely can you prove something by example. You can do it cases where you just need to find one to prove something
- Example 3.2.10:
    So we are trying to prove that if a or b are odd integers then $a+b$ is also an odd integer. All we need is a counter example, which could be 3 and 1. Both 3 and 1 are odd but added together are 4, an even number.
- Proving by cases is proving that $q \implies p$ and $\neg q \implies p$, meaning that p is true regardless of q. The trick is to show that some q implies p regardless of its negation.
- Example 3.2.11:
    n can be either even or odd, thus giving us our regular and negated P. So for the even $n=2k$, meaning $$8k^3-2k$$ $$2(4k^3-k)$$
    and for our odd case we know that $n=2k+1$ so $$(2k+1)^3-2k-1$$ $$8k^3+6k^2+6k+1-2k-1$$ $$2(4k^3+3k^2+2k)$$