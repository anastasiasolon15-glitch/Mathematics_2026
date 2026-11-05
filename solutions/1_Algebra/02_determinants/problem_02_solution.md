# Determinants — Exercise 2. Determinant of a 3×3 Matrix

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

## Solution

### Step 1. Sarrus' rule

Sum of products along the "down-right" diagonals:

$$
1\cdot3\cdot5 + 2\cdot4\cdot2 + (-1)\cdot0\cdot1 = 15 + 16 + 0 = 31.
$$

Sum of products along the "up-right" diagonals:

$$
(-1)\cdot3\cdot2 + 1\cdot4\cdot1 + 2\cdot0\cdot5 = -6 + 4 + 0 = -2.
$$

Therefore

$$
\det A = 31 - (-2) = 33.
$$

### Step 2. Check using a determinant property

Adding a multiple of one row to another row does not change the determinant. Apply

$$
R_3 \leftarrow R_3 - 2R_1:\quad
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}
$$

and then

$$
R_3 \leftarrow R_3 + R_2:\quad
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11 \\
\end{pmatrix}.
$$

The matrix is upper triangular, so its determinant is the product of the diagonal entries:

$$
1\cdot3\cdot11 = 33.
$$

## Explanation of the result

Both methods give $\det A = 33$. Both row operations used were of the type "add a multiple of one row to another", which does not change the determinant, so the two values must agree. Since $\det A = 33 \neq 0$, the matrix $A$ is invertible.
