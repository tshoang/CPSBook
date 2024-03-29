Validity, Satisfiablity, and Unsatifiability
=============================================
This folder contains the discussion about *valid*, *satisifiable*, and
*unsatisfiable* as in *Exercise 4.11* of the CPS book. A dL formula is
- valid: if it holds for all states
- satisfiable: if it holds for some states
- unsatisfiable: if it holds for none states.
As a result, if a formula valid then it is satisfiable. If a formula
is valid then its negation is unsatisfiable and vice versa.
```
For each j;k {satisfiable; unsatisfiable;valid} answer whether there
is a formula that is j but not k. Also answer for each such j;k
whether there is a formula that is j but its negation is not
k. Briefly justify each answer.
```

j but not k
-----------
The following table j is the rows and k is the columns. Each cell
represents the example/no example for j but not k. 
|                | Valid | Satisfiable | Unsatisfiable |
|----------------|-------|-------------|---------------|	
| Valid          |       |   NONE      |     true      |
| Satisfiable    | x >=0 |             |     x >= 0    |
| Unsatisfiable  | false |  false      |               |


!j is not k
-----------
The following table j is the rows and k is the columns.  Each cell
represents the example/no example for negation of j is not k. 
|                | Valid | Satisfiable | Unsatisfiable |
|----------------|-------|-------------|---------------|	
| Valid          |       |   true      |     NONE      |
| Satisfiable    | x >=0 |             |    x >= 0     |
| Unsatisfiable  | NONE  |   NONE      |               |
