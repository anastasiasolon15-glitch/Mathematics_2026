# Exercise 6. Solving a System Using the Inverse

## Question

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## Solution

### Steps

The determinant is $\det A=2\cdot3-1\cdot1=5$, so

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
3\cdot5+(-1)\cdot7 \\
-1\cdot5+2\cdot7 \\
\end{pmatrix} \\
&=\frac15
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

$$
x=
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

### Method

If $A$ is invertible, multiplying $Ax=b$ from the left by $A^{-1}$ gives $x=A^{-1}b$. This is the unique solution.

### Verification

Substituting into $Ax$:

$$
\begin{aligned}
Ax &=
\begin{pmatrix}
2\cdot\frac85+\frac95 \\
\frac85+3\cdot\frac95 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=b.
\end{aligned}
$$
