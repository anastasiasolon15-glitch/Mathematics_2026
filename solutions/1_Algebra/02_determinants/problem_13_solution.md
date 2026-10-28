# Exercise 13. Determinant by Elimination

## Question

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

### Steps

Step 1, $R_2\leftarrow R_2-2R_1$. The determinant does not change. The new row 2 is $(0,\ 1,\ 1)$.

Step 2, $R_3\leftarrow R_3-R_1$. The determinant does not change. The new row 3 is $(0,\ -2,\ -1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

Step 3, $R_3\leftarrow R_3+2R_2$. The determinant does not change. The new row 3 is $(0,\ 0,\ 1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

The matrix is upper triangular, so the determinant is the product of the diagonal entries:

$$
1\cdot1\cdot1=1.
$$

### Result

$$
\det A=1.
$$

### Method

Each of the three operations adds a multiple of one row to another, which leaves the determinant unchanged. No swaps or row scalings occurred, so no correction factor is needed, and $\det A$ equals the determinant of the final triangular matrix.

### Verification

Expansion of the original matrix along the first row:

$$
\begin{aligned}
\det A &= 1\cdot(5\cdot2-7\cdot0)-2\cdot(2\cdot2-7\cdot1)+3\cdot(2\cdot0-5\cdot1) \\
&= 10-2\cdot(-3)+3\cdot(-5) \\
&= 10+6-15 \\
&= 1.
\end{aligned}
$$
