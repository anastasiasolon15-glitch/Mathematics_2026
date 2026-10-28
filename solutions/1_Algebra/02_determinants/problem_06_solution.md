# Exercise 6. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

### Steps

The determinant of $A(t)$ is

$$
\det A(t)=t\cdot t-1\cdot2=t^2-2.
$$

The matrix is not invertible exactly when the determinant vanishes:

$$
t^2-2=0.
$$

This gives

$$
t=\sqrt{2}\quad\mathrm{or}\quad t=-\sqrt{2}.
$$

### Result

The matrix $A(t)$ is not invertible for $t=\sqrt{2}$ and $t=-\sqrt{2}$, and it is invertible for all other values of $t$.

### Method

A square matrix is invertible if and only if its determinant is nonzero. Therefore the set of values of $t$ for which $A(t)$ fails to be invertible is the set of roots of the equation $\det A(t)=0$.

### Verification

For $t=\sqrt{2}$ the second row $(2,\ \sqrt{2})$ equals $\sqrt{2}$ times the first row $(\sqrt{2},\ 1)$, because $\sqrt{2}\cdot\sqrt{2}=2$ and $\sqrt{2}\cdot1=\sqrt{2}$. The rows are dependent, as expected for a zero determinant. For $t=0$, for example, $\det A(0)=-2\neq0$, so the matrix is invertible.
