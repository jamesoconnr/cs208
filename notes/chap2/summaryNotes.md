- Investigate: 
    1. Assuming I don't eat from my initial bean collection, $10, 15, 25, 45, 85$ Recursive definition is $a_n=2a_{n-1}-5$ with $a_0=10$. I know this is correct because the number of beans after day 1 always ends in 5. When you double a number ending 5 you get a number ending in 0. Eat 5 beans and now you have another number ending in 5.
    2. All numbers ending in 5 are factors of 5. So lets say I have k beans, and k ends in 5. So, in other words, $k=5j$ where j is an integer. Now lets double my k beans ($k=5j$) and eat (subtract) 5 beans $2k-5=5j$. Doubling and subtracting 5 beans gives us our pre-breakfast bean count for the next day, so it is $(k+1)$. Now we have $(k+1)=5j$ meaning all days after day 0 have a bean count ending in 5.
    3. Well we can see the difference between terms is doubling every time. So the difference is $5*2^n$. TODO

- If there is a constant difference we can use our arithmetic/geometric formulas and initial conditions to find a recursive relation
