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

### Sarrus' rule

For a $3\times3$ matrix, Sarrus' rule adds the products along the three "main" diagonals and subtracts the products along the three "anti-diagonals":

$$
\det A = a_{11}a_{22}a_{33}+a_{12}a_{23}a_{31}+a_{13}a_{21}a_{32}-a_{13}a_{22}a_{31}-a_{11}a_{23}a_{32}-a_{12}a_{21}a_{33}.
$$

Positive terms:

$$
1\cdot3\cdot5=15,\qquad 2\cdot4\cdot2=16,\qquad (-1)\cdot0\cdot1=0,
$$

which sum to $31$.

Negative terms:

$$
(-1)\cdot3\cdot2=-6,\qquad 1\cdot4\cdot1=4,\qquad 2\cdot0\cdot5=0,
$$

which sum to $-2$.

Therefore

$$
\det A = 31-(-2)=33.
$$

### Check using a determinant property

Adding a multiple of one row to another row does not change the determinant. We use this to create zeros below the first pivot and then below the second pivot.

First, $R_3\leftarrow R_3-2R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}.
$$

Next, $R_3\leftarrow R_3+R_2$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11 \\
\end{pmatrix}.
$$

Both operations leave the determinant unchanged, and the resulting matrix is upper triangular. The determinant of a triangular matrix is the product of its diagonal entries:

$$
\det A = 1\cdot3\cdot11=33.
$$

This agrees with the result from Sarrus' rule.

### Answer

$$
\det A = 33.
$$

Since $\det A\neq0$, the matrix $A$ is invertible.
