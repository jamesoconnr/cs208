## Which of the following graphs are trees?
a. $G = (V, E)$ with $V = \{a, b, c, d, e\}$ and $E = \{\{a, b\}, \{a,e\}, \{b, c\}, \{c,d\}, \{d,e\} \}$
```mermaid
graph TD;
    A --> B;
    A --> E;
    B --> C;
    C --> D;
    D --> E;
```
    no it has an obvious cycle

b. What if $E = \{\{a, b\}, \{b, c\}, \{c,d\}, \{d,e\}\}$?
```mermaid
graph TD;
    A --> B;
    B --> C;
    C --> D;
    D --> E;
```

    yes, there are no cycle. It is also a path, and all paths are trees

c. What if $E = \{\{a, b\}, \{a, c\}, \{a,d\}, \{a,e\}\}$?
```mermaid
graph TD;
    A --> B;
    A --> C;
    A --> D;
    A --> E;
```

    yes, there are no cycles and it is a star. All stars are trees

d. What if $E = \{\{a, b\}, \{a, c\}, \{d,e\}\}$?
```mermaid
graph TD;
    A --> B;
    A --> C;
    D --> E;
```
There are not enough edges (should be $v-1$) and it should be connected, so it is not a tree
