- Induction is a proof method
- Investigate: Seemingly any multiple of 8 and any multiple of 5 is whats possible. I don't know where to go from here as clearly other values are possible (such as 13), but IDK how to describe that. I mean generally where x and y are natural numbers it is $5x+8y$
    -Could be represented as $P(1),P(2),P(3),P(4),P(5)$ where the number is the cents you are trying to make from 8 and 5. So the sequence above would be $F, F, F, F, T$
    - So we find that at a certain point we know the value is true because the previous one is. We know this because you can just rearrange the 5s and 8s.
    - This process starts at 28, so we know that $P(K)$ is true for all $k\geq 28$
    - 28 is the base case and every other term is the inductive case
    - Revisit these notes, TODO
- Induction is good for proving things about natural numbers, especially when there is a clear why to go from case to the next.
- "When you are asked to provide a proof by induction, you are being asked to think about the problem dynamically; how does increasing n change the problem?"
- Format for inductive proofs is statement you are trying to prove, base case, and inductive case (i.e how if $P(k)$ then $P(k+1)$)
- Example 2.5.1: So we know that when summing a sequence that last sum $+ a_n$ is equal to the sum of $n$. Lets assume that $P(k)=1+2+3+...+k=\frac{k(k+1)}{2}$ is true. So because of what i said in the first sentence we can just add $(k+1)$ to both sides and hope we get $\dfrac{(k+1)(k+2)}{2}$, as that is what you get when you plug in $(k+1)$. So we add $(k+1)$ to both sides $$1+2+3+...+k+(k+1)=\frac{k(k+1)}{2}$$ $$\dfrac{k(k+1)+2(k+1)}{2}$$ $$\dfrac{k^2+k+2k+2}{2}$$ $$\dfrac{k^2+3k+2}{2}$$ $$\dfrac{(k+2)(k+1)}{2}$$ so we have proved it.
- Example 2.5.2: Every time we increase n we multiple the previous value + 1 times 6. Every time we multiply by 6 we get a number that ends in 6, so naturally by subtracting 1 we get a number that ends in 5. Our statement will be "$6^n-1$ is a multiple of 5$ to where n is a natural number (im on plane so i cannot look up the latex for this). Our base will be $P(0)=6^0-1=0$ which is true. Let k be some n and assume $P(k)$ is true. So $6^k-1=5j$ where j is an integer. So we know that $6^k=5j+1$ and multiply the right by 6 and subtract 1. $30j+5=6^{k+1}-1$ and we can factor out 5 get $6^{k+1}-1=5(6j+1)$, which just says $6^{k+1}-1$ is a multiple of 5.
- Example 2.5.3: Well every time we increase n we square the left side and double the right. Consider that the difference between two consecutive squares is $(n+1)^2-n^2$, which factors to $(n+1-n)(n+1-n)$, which is equal to $2n+1$. Now consider that when doubling the right side it increases by $2^n$, because $2^{n+1}=2^n+2^n$. So once n is larger than or equal to 5, $2^n>2n+1$. So in the original statement, the left hand side grows less than the right hand side so if n starts smaller the left will never catch up. Proof statement is: Let $P(n) be the statement $n^2<2^n$ for all integers $n\geq5$. Base case: $P(5)$ is $5^2<2^5$, $25<32$. Inductive case: Let $k\geq5$ be an int. Assume $P(k)$ is true. I don't understand the rest, TODO
- Inductions isn't magic, if the case after the base case is clearly false induction doesn't work
### Strong Induction
- Suppose you have a chocolate bar made up of n squares. How many times will you have to break it.
    - it is immediately pretty obvious that it will take n-1 breaks to turn it into squares
    - When you break a bar, you are left with smaller chocolate bars. This act of reducing to smaller cases is what induction is all about. 
    - If we are trying to prove our conjecture (the first sub-bullet point) inductively, we don't know after we break $(k+1)$-square bar we will be left with $k$ squares, so we must assume our conjecture is right for all squares less than $k+1$
    - Our final proof is:
    **Statement:** it takes $n-1$ breaks to reduce and n-square chocolate bar to single squares
    
    **Base Case:** Consider $P(2)$. In one break ($n-1$) you have reduced the bar into single squares
    
    **Inductive case:** Choose an arbitrary $n\geq2$ and assume $P(k)$ is true for all $k<n$. Consider an n-square bar. You break it in half and get two pieces, a and b. You know $a+b=n$ and that $a<n$, $b<n$. So by our inductive hypothesis we know that both are reduced to single squares in $a-$ and $b-1$ breaks. So, including the original break, we can represent this as $$1+a-1+b-1$$ $$a+b-1$$ $$n-1$$ thus proving $P(n)$ is true.
- So in strong induction you assume $P(k)$ is true for $k<n$, prove $P(n)$ is true, and then assume $P(n)$ is true for all $n>$ base case (that last n is not the arbitrary n, it is all numbers)