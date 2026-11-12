### Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

## Solution

Apply $R_2\leftarrow R_2-aR_1$:

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
a & a & 4
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 4-2a
\end{array}\right).
$$

The second row reads $0=4-2a$. Two cases:

- $a=2$: the row becomes $0=0$. The system reduces to $x+y=2$, so $y=t$ is free and $(x,y)=(2-t,\;t)$. **Infinitely many solutions.**
- $a\ne 2$ (including $a=0$): the row becomes $0=4-2a\neq 0$, a contradiction. **No solution.**

**Exactly one solution never occurs.** After elimination the second column never gets a pivot: the coefficients of $y$ and $x$ are equal in both rows, so the rows of the coefficient matrix are proportional and there is at most one pivot for two unknowns. Then $y$ is always free or the system is inconsistent. Geometrically, the lines $x+y=2$ and $a(x+y)=4$ are parallel (or coincide), so they cannot meet in exactly one point.
