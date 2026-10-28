# Exercise 11. Shortening the Calculation with Row Operations

## Question

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

### Steps

The first column has the entry $1$ in every row, so subtracting the first row from the other two rows creates zeros below the pivot.

Step 1, $R_2\leftarrow R_2-R_1$, gives the new row $(0,\ 1,\ 1)$.

Step 2, $R_3\leftarrow R_3-R_1$, gives the new row $(0,\ 2,\ 3)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

Step 3, $R_3\leftarrow R_3-2R_2$, gives the new row $(0,\ 0,\ 1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

The matrix is upper triangular, so the determinant is $1\cdot1\cdot1=1$.

### Result

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}=1.
$$

### Method

All three operations add a multiple of one row to another row. Such operations do not change the determinant. Only a row swap (sign change) or multiplying a row by a number (the determinant is multiplied by that number) would change it, and neither was used.

### Verification

Expansion of the original matrix along the first row:

$$
\begin{aligned}
\det &= 1\cdot(3\cdot6-4\cdot4)-2\cdot(1\cdot6-4\cdot1)+3\cdot(1\cdot4-3\cdot1) \\
&= 2-4+3 \\
&= 1.
\end{aligned}
$$
