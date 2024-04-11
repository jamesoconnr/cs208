1. . 

    a. P is the event of your birthday, Q is the presence of a cake

    b. 
        ```
        ttg_cli.py "['p', 'q']" -p "['(p or q) => q']" -i False
        +-----+-----+-----------------+
        |  p  |  q  |  (p or q) => q  |
        |-----+-----+-----------------|
        |  1  |  1  |        1        |
        |  1  |  0  |        0        |
        |  0  |  1  |        1        |
        |  0  |  0  |        1        |
        +-----+-----+-----------------+
        ```
    
    c. If there is cake I can conclude there will be cake

    d. I can conclude that its not your birthday because the scenario in which it is your birthday and there is cake is false.

    e. Then I can conclude there will only be cake if it is not your birthday and there will not be cake

2. 
    ```
    ttg_cli.py "['p', 'q']" -p "['(p or q) => (p and q)']" -i False
    +-----+-----+-------------------------+
    |  p  |  q  |  (p or q) => (p and q)  |
    |-----+-----+-------------------------|
    |  1  |  1  |            1            |
    |  1  |  0  |            0            |
    |  0  |  1  |            0            |
    |  0  |  0  |            1            |
    +-----+-----+-------------------------+
    ```
3. 
    ```
    ttg_cli.py "['p', 'q', 'r']" -p "['~p and (q=>p)']" -i False
    +-----+-----+-----+-----------------+
    |  p  |  q  |  r  |  ~p and (q=>p)  |
    |-----+-----+-----+-----------------|
    |  1  |  1  |  1  |        0        |
    |  1  |  1  |  0  |        0        |
    |  1  |  0  |  1  |        0        |
    |  1  |  0  |  0  |        0        |
    |  0  |  1  |  1  |        0        |
    |  0  |  1  |  0  |        0        |
    |  0  |  0  |  1  |        1        |
    |  0  |  0  |  0  |        1        |
    +-----+-----+-----+-----------------+
    ```
    I can conclude that when P and Q are true the statement is true, otherwise it is false.
4. 
5. 
6. Well I know that $\neg(P\implies Q)=\neg P \land Q$ from example 3.1.4
7. 
8. . 

    a. $P \land Q$

    b. $$\neg(\neg P \lor \neg Q) \lor \neg(\neg Q \land R)$$
    $$(P \land Q) \lor (Q \lor \neg R)$$

    c. $$\neg (P \implies \neg Q) \land (R \land \neg R)$$
    $$\neg (P \lor Q) \land (R \land \neg R)$$
    $$(\neg P \land \neg Q) \neg (R \land \neg R)$$

    d. $$\neg((\neg M \implies W) \land \neg W)$$
    $$\neg (\neg M \implies W) \lor W$$
    $$\neg (M \lor W) \lor W$$
    $$ (\neg M \land \neg W) \lor W$$

9. 
10. 
11. 
12.
    ```
    ttg_cli.py "['p', 'q']" -p "['p or q', '~p']" -i False

    +-----+-----+----------+------+
    |  p  |  q  |  p or q  |  ~p  |
    |-----+-----+----------+------|
    |  1  |  1  |    1     |  0   |
    |  1  |  0  |    1     |  0   |
    |  0  |  1  |    1     |  1   |
    |  0  |  0  |    0     |  1   |
    +-----+-----+----------+------+
    ```
    when both are true q is true
13. 
14. 
15. 
16. 