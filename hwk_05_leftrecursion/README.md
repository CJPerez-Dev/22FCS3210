# Left Recursion Elimination
- By Chase Perez

Eliminate any left-recursive productions (including indirect ones). When you are done, submit this README.md file with your answers on Canvas. 

## Q1

```
X -> XYz | Xw | w
Y -> Yp | q

Solution:
X -> wX'
X' -> YzX' | wX' | ε
Y -> qY'
Y' -> pY' | ε
```


## Q2

```
S -> aA | Sd
A -> b

Solution:
S -> aAS'
S' -> dS' | ε
A -> b
```

## Q3

```
A -> Bxy | x
B -> CD
C -> A | c
D -> d 

Solution:
A -> cDxyA' | xA'
A' -> DxyA' | ε
B -> CD
C -> A | c
D -> d
```
