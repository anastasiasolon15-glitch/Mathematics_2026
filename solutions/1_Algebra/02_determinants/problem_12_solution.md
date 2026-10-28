# Exercise 12. A Parameter Revealed by a Row Operation

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

### Steps

The operation $R_2\leftarrow R_2-2R_1$ does not change the determinant. The new second row is $(2-2,\ 4-4,\ t-6)=(0,\ 0,\ t-6)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

Expanding along the first column, only the entry $1$ is nonzero:

$$
\begin{aligned}
\det A(t) &= 1\cdot\det
\begin{pmatrix}
0 & t-6 \\
1 & 1 \\
\end{pmatrix} \\
&= 0\cdot1-(t-6)\cdot1 \\
&= 6-t.
\end{aligned}
$$

The determinant is zero exactly when $t=6$.

### Result

The matrix $A(t)$ is not invertible if and only if $t=6$.

### Method

A matrix is not invertible exactly when its determinant is $0$. After the row operation, the first two entries of the second row are already zero, so the whole determinant depends on the single parameter entry $t-6$.

For $t=6$ the transformed second row becomes $(0,0,0)$. This means that the original second row is $(2,4,6)=2\cdot(1,2,3)$, so the first two rows are proportional, which is a linear dependence of the rows.

### Verification

Expansion of the original matrix along the third row $(0,1,1)$:

$$
\begin{aligned}
\det A(t) &= -1\cdot\det
\begin{pmatrix}
1 & 3 \\
2 & t \\
\end{pmatrix}
+1\cdot\det
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix} \\
&= -(t-6)+0 \\
&= 6-t.
\end{aligned}
$$

This agrees with the first calculation.
