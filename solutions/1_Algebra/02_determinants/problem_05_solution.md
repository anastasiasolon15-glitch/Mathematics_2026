# Determinants — Exercise 5. Row Operations

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### Step 1. $R_2 \leftarrow R_2 - 2R_1$

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

Adding a multiple of one row to another: the determinant **does not change**.

### Step 2. $R_3 \leftarrow R_3 + R_1$

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

Again adding a multiple of one row to another: the determinant **does not change**.

### Step 3. $R_3 \leftarrow R_3 + 2R_2$

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

The determinant **does not change**.

### Step 4. Triangular matrix

The matrix is upper triangular, so the determinant is the product of the diagonal entries:

$$
\det A = 1\cdot(-3)\cdot(-7) = 21.
$$

### Check by cofactor expansion along the first row

$$
\det A = 1\cdot(1\cdot2-0\cdot4) - 2\cdot(2\cdot2-0\cdot(-1)) + 3\cdot(2\cdot4-1\cdot(-1)) = 2 - 8 + 27 = 21.
$$

## Explanation of the result

All three operations were of the type "add a multiple of one row to another", so the determinant stayed the same at every step and $\det A$ equals the determinant of the final triangular matrix, $21$. Since $\det A \neq 0$, the matrix $A$ is invertible.
