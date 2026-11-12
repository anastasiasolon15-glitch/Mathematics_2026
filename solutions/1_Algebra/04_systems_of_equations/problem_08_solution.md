### Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
\qquad
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

Both systems have the coefficient matrix $A=\begin{pmatrix}2&1\\1&-1\end{pmatrix}$ and differ only in the right-hand side. Apply $R_2\leftarrow R_2-\tfrac12R_1$.

**System 1:**

$$
\left(\begin{array}{cc|c}
2 & 1 & 5 \\
1 & -1 & 1
\end{array}\right)
\to
\left(\begin{array}{cc|c}
2 & 1 & 5 \\
0 & -\tfrac32 & -\tfrac32
\end{array}\right)
\Rightarrow y=1,\; x=2.
$$

**System 2:**

$$
\left(\begin{array}{cc|c}
2 & 1 & 1 \\
1 & -1 & 4
\end{array}\right)
\to
\left(\begin{array}{cc|c}
2 & 1 & 1 \\
0 & -\tfrac32 & \tfrac72
\end{array}\right)
\Rightarrow y=-\tfrac73,\; x=\tfrac53.
$$

**Verification.** System 1: $4+1=5$, $2-1=1$. System 2: $\tfrac{10}{3}-\tfrac73=1$, $\tfrac53+\tfrac73=4$.

**What is the same.** The row operation and the coefficient part of the resulting matrix, $\begin{pmatrix}2&1\\0&-\tfrac32\end{pmatrix}$, are identical in both systems. The multiplier $\tfrac12$ is determined only by the entries of $A$. Only the last column (the right-hand side) changes. So the elimination for $A$ can be done once and reused for any right-hand side.
