# Exercise 8. Row Operations and Their Reversibility

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

### Steps

Step 1, $R_2\leftarrow R_2-2R_1$, where the new row 2 is $(2-2,\ 4-4,\ 1+2)=(0,0,3)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

Step 2, $R_3\leftarrow R_3+R_1$, where the new row 3 is $(-1+1,\ 1+2,\ 3-1)=(0,3,2)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

Step 3, interchange $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

### Result

The final matrix is upper triangular, and the reverse operations are:

1. $R_2\leftarrow R_2-2R_1$ is reversed by $R_2\leftarrow R_2+2R_1$.
2. $R_3\leftarrow R_3+R_1$ is reversed by $R_3\leftarrow R_3-R_1$.
3. The interchange of $R_2$ and $R_3$ is reversed by the same interchange.

### Method

Each elementary row operation can be undone by another elementary row operation, so row operations do not lose information about the matrix. To undo a sequence of operations, the reverse operations are applied in the reverse order.

### Verification

Applying the reverse operations to the final matrix in the order 3, 2, 1:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
\ \to\
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
\ \to\
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
\ \to\
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

The last matrix is the original $A$, so the operations are fully reversed.
