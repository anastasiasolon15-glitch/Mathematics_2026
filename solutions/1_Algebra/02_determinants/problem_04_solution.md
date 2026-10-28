# Exercise 4. Triangular Matrix

## Question

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

## Solution

### Steps

The matrix is upper triangular, so its determinant is the product of the diagonal entries:

$$
2\cdot(-3)\cdot7=-42.
$$

### Result

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}=-42.
$$

### Method

Rule: the determinant of an upper or lower triangular matrix equals the product of its diagonal entries.

Explanation in this example: expanding along the first column, only the entry $2$ is nonzero, so the determinant equals $2$ times the determinant of the remaining $2\times2$ block. That block is again triangular, and expanding it along its first column gives $-3$ times the remaining entry $7$. Thus the diagonal entries multiply one after another.

### Verification

Expansion along the first column written out:

$$
\begin{aligned}
\det &= 2\cdot\det
\begin{pmatrix}
-3 & 5 \\
0 & 7 \\
\end{pmatrix} \\
&= 2\cdot\bigl((-3)\cdot7-5\cdot0\bigr) \\
&= 2\cdot(-21) \\
&= -42.
\end{aligned}
$$

The result agrees with the product of the diagonal entries.
