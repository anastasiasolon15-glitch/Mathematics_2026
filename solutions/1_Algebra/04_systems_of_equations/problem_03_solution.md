### Exercise 3. Inconsistent System

## Question

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## Solution

Write the augmented matrix and apply $R_2\leftarrow R_2-2R_1$:

$$
\left(\begin{array}{cc|c}
1 & 2 & 3 \\
2 & 4 & 7
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 2 & 3 \\
0 & 0 & 1
\end{array}\right).
$$

The second row says $0\cdot x+0\cdot y=1$, i.e. $0=1$, which is impossible for any $x,y$. Therefore the system has **no solution**.

**Interpretation.** The left-hand side of the second equation is twice the left-hand side of the first, so if $x+2y=3$, then $2x+4y$ must equal $6$, not $7$. The equations contradict each other. Geometrically, the lines $x+2y=3$ and $2x+4y=7$ are parallel and distinct, so they never meet.
