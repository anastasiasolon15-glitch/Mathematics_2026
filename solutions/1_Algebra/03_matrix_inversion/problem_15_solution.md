# Exercise 15. Two Methods for Solving the Same System

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### Steps

Method 1, the inverse. Since $\det A=2\cdot3-1\cdot1=5$,

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Then

$$
\begin{aligned}
x=A^{-1}b &=\frac15
\begin{pmatrix}
3\cdot7-1\cdot8 \\
-1\cdot7+2\cdot8 \\
\end{pmatrix} \\
&=\frac15
\begin{pmatrix}
13 \\
9 \\
\end{pmatrix}.
\end{aligned}
$$

Method 2, Gaussian elimination. The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}.
$$

Interchange $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

Then $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

The second row gives $x_2=\frac95$. Back substitution into the first row gives

$$
x_1=8-3\cdot\frac95=\frac{40-27}{5}=\frac{13}{5}.
$$

### Result

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

### Method

Both methods give the same vector. The inverse method needs the determinant, the formula for $A^{-1}$ (four entries to compute) and a matrix-vector product. Gaussian elimination needs one row interchange, one row operation and one back substitution. In this example elimination was shorter and did not require the inverse, which is a larger object than the single solution needed. The inverse is worth computing when the same $A$ is used with many right-hand sides $b$.

### Verification

Substituting the solution:

$$
\begin{aligned}
Ax &=
\begin{pmatrix}
2\cdot\frac{13}{5}+\frac95 \\
\frac{13}{5}+3\cdot\frac95 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac{35}{5} \\
\frac{40}{5} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}=b.
\end{aligned}
$$
