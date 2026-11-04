# Exercise 2. Formula for a 2×2 Matrix

## Question

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Solution

### Steps

For

$$
A=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

with $\det A=ad-bc\neq0$ the inverse is

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}.
$$

Here $\det A=3\cdot4-2\cdot5=12-10=2$, so

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$

### Result

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$

### Method

The formula swaps the diagonal entries, changes the signs of the off-diagonal entries and divides by the determinant. It requires $\det A\neq0$.

### Verification

$$
\begin{aligned}
AA^{-1} &=
\begin{pmatrix}
3\cdot2+2\cdot\left(-\frac{5}{2}\right) & 3\cdot(-1)+2\cdot\frac{3}{2} \\
5\cdot2+4\cdot\left(-\frac{5}{2}\right) & 5\cdot(-1)+4\cdot\frac{3}{2} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$
