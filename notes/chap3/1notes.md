- Investigate!: I think they are both knights because if the first one is a knight the statement is still true and 2 is can be true if both are false
- Propositional logic = study of how statements interact
- $\lor$ is or
- Example 3.1.1:
    ```
    ttg_cli.py "['p', 'q', 'r']" -p "['(p => q) or (q => r)']" -i False
    +-------+-------+-----------+
    |   p   |   q   |  ~p or q  |
    |-------+-------+-----------|
    | True  | True  |   True    |
    | True  | False |   False   |
    | False | True  |   True    |
    | False | False |   True    |
    +-------+-------+-----------+
    ```
- Example 3.1.2:
    ```
    ttg_cli.py "['p', 'q', 'r']" -p "['(p => q) or (q => r)']" -i False
    +-------+-------+-----------+
    |   p   |   q   |  ~p or q  |
    |-------+-------+-----------|
    | True  | True  |   True    |
    | True  | False |   False   |
    | False | True  |   True    |
    | False | False |   True    |
    +-------+-------+-----------+
    ```
- Tautology is when a statement is logically true with no actual relation to the real world
- When two statements have the same truth value regardless of combination they are logically equivalent
- Example 3.1.3:
    Ill generate a true table to check
    ```
    ttg_cli.py "['r', 's']" -p "['~(r or s)', '~r and ~s']" -i False 
    +-------+-------+-------------+-------------+
    |   r   |   s   |  ~(r or s)  |  ~r and ~s  |
    |-------+-------+-------------+-------------|
    | True  | True  |    False    |    False    |
    | True  | False |    False    |    False    |
    | False | True  |    False    |    False    |
    | False | False |    True     |    True     |
    +-------+-------+-------------+-------------+
    ```
- Implications are equivalent to disjunctions, $P\implies Q = \neg P\lor Q$
- Example 3.1.4:
    We know that implications are really disjunctions, so the left is $\neg (\neg P \lor Q)$ which distributes too $P \land \neg Q$
- Example 3.1.5
    ```
    tg_cli.py "['p', 'q', 'r']" -p "['(p or q) => r', '(p=>r) or (q=>r)']" -i False
    +-----+-----+-----+-----------------+--------------------+
    |  p  |  q  |  r  |  (p or q) => r  |  (p=>r) or (q=>r)  |
    |-----+-----+-----+-----------------+--------------------|
    |  1  |  1  |  1  |        1        |         1          |
    |  1  |  1  |  0  |        0        |         0          |
    |  1  |  0  |  1  |        1        |         1          |
    |  1  |  0  |  0  |        0        |         1          |
    |  0  |  1  |  1  |        1        |         1          |
    |  0  |  1  |  0  |        0        |         1          |
    |  0  |  0  |  1  |        1        |         1          |
    |  0  |  0  |  0  |        1        |         1          |
    +-----+-----+-----+-----------------+--------------------+
    ```