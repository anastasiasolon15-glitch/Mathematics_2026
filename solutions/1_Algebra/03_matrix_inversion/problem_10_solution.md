# Exercise 10. Inverse of a Diagonal Matrix

## Question

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

### Steps

The determinant of a diagonal matrix is the product of its diagonal entries.

$$
\det D=2\cdot(-3)\cdot5=-30\neq0,\qquad \det E=2\cdot0\cdot5=0.
$$

So $D$ is invertible and $E$ is not. Also, $E$ has a zero row, so the rows of $E$ are dependent.

The inverse of $D$ is the diagonal matrix with reciprocal entries:

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}.
$$

### Result

The matrix $D$ is invertible with the inverse given above, and $E$ is not invertible.

### Method

A diagonal matrix is invertible if and only if all diagonal entries are nonzero, and then the inverse is obtained by taking reciprocals of the diagonal entries. The matrix $E$ has the entry $0$ on the diagonal, and a zero row cannot be turned into a row of $I$.

### Verification

$$
\begin{aligned}
DD^{-1} &=
\begin{pmatrix}
2\cdot\frac12 & 0 & 0 \\
0 & (-3)\cdot\left(-\frac13\right) & 0 \\
0 & 0 & 5\cdot\frac15 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$

For $E$, any product $EX$ has a zero second row, so it can never equal $I$.
