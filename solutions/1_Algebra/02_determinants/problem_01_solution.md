# Exercise 1. Determinant of a 2×2 Matrix

## Question

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},\qquad \det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$

Which matrix is invertible? Justify your answer.

## Solution

### Steps

For a $2\times2$ matrix the determinant is $ad-bc$.

$$
\begin{aligned}
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}
&= 3\cdot4-(-2)\cdot5 \\
&= 12+10 \\
&= 22.
\end{aligned}
$$

$$
\begin{aligned}
\det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}
&= 1\cdot14-7\cdot2 \\
&= 14-14 \\
&= 0.
\end{aligned}
$$

### Result

The determinants are $22$ and $0$. Only the first matrix is invertible.

### Method

A square matrix is invertible if and only if its determinant is nonzero. The first determinant is nonzero, so that matrix is invertible. The second determinant is zero, so that matrix is not invertible. This is visible in its rows: the second row is twice the first row, so the rows are dependent.

### Verification

For the first matrix the inverse exists and is given by the $2\times2$ formula:

$$
A^{-1}=\frac{1}{22}
\begin{pmatrix}
4 & 2 \\
-5 & 3 \\
\end{pmatrix}.
$$

The product of the matrix with the integer matrix $22A^{-1}$ gives

$$
\begin{aligned}
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}
\begin{pmatrix}
4 & 2 \\
-5 & 3 \\
\end{pmatrix}
&=
\begin{pmatrix}
22 & 0 \\
0 & 22 \\
\end{pmatrix} \\
&= 22I,
\end{aligned}
$$

so the inverse works. For the second matrix no inverse exists, in agreement with the zero determinant.
