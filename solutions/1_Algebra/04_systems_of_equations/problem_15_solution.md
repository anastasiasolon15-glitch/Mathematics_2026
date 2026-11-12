### Exercise 15. Classifying Three Systems

## Question

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

## Solution

One elimination step in each case is enough.

**System 1.** $R_2\leftarrow R_2-R_1$:

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
1 & -1 & 0
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -2 & -2
\end{array}\right).
$$

There are two pivots for two unknowns, so there is **exactly one solution**: $y=1$, $x=1$. Check: $1+1=2$, $1-1=0$.

**System 2.** $R_2\leftarrow R_2-2R_1$:

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
2 & 2 & 4
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 0
\end{array}\right).
$$

The row $0=0$ is consistent, and there is one pivot for two unknowns, so $y=t$ is free. **Infinitely many solutions:** $(x,y)=(2-t,\;t)$.

**System 3.** $R_2\leftarrow R_2-2R_1$:

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
2 & 2 & 5
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 1
\end{array}\right).
$$

The row $0=1$ is a contradiction, so there is **no solution**.

**Summary.** After elimination, look at the rows: a row $0=c$ with $c\neq0$ means no solution; otherwise, the number of pivots equals the number of unknowns for a unique solution and is smaller for infinitely many solutions.
