# Exercise 10. Detecting Dependence

## Question

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

### Steps

Denote the rows by $r_1=(1,2,3)$, $r_2=(2,4,6)$, $r_3=(0,1,5)$. The second row is twice the first:

$$
r_2=2r_1.
$$

Equivalently, $2r_1-r_2+0\cdot r_3=0$ is a nontrivial linear dependence between the rows.

The operation $R_2\leftarrow R_2-2R_1$ does not change the determinant and produces the matrix

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}.
$$

A matrix with a zero row has determinant $0$, because each term of the determinant contains one entry from every row.

### Result

The determinant is $0$.

### Method

Linearly dependent rows always give determinant $0$. By the theorem relating determinants and invertibility, a matrix with determinant $0$ is not invertible. The dependence among the rows also means that the rows do not span the whole space, and the matrix cannot be inverted.

### Verification

A direct expansion along the first column confirms the result:

$$
\begin{aligned}
\det &= 1\cdot(4\cdot5-6\cdot1)-2\cdot(2\cdot5-3\cdot1)+0 \\
&= 14-2\cdot7 \\
&= 0.
\end{aligned}
$$
