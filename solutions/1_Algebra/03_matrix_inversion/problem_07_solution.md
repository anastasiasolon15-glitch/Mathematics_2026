# Exercise 7. Inverse of a Product

## Question

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

### Steps

The product is

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix},\qquad \det(AB)=6.
$$

By the $2\times2$ formula:

$$
\begin{aligned}
(AB)^{-1} &=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
\end{aligned}
$$

The individual inverses are

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}.
$$

Their product in the reversed order:

$$
\begin{aligned}
B^{-1}A^{-1} &=
\begin{pmatrix}
\frac12\cdot1 & \frac12\cdot(-1) \\
0 & \frac13 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

$$
(AB)^{-1}=B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

### Method

The product $AB$ means "first apply $B$, then apply $A$". To undo it, the last step has to be undone first, so $A^{-1}$ acts first and $B^{-1}$ second. Algebraically,

$$
(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AA^{-1}=I.
$$

### Verification

The other order gives a different matrix:

$$
\begin{aligned}
A^{-1}B^{-1} &=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
\frac12 & -\frac13 \\
0 & \frac13 \\
\end{pmatrix}.
\end{aligned}
$$

This differs from $(AB)^{-1}$ in position $(1,2)$, so the reversed order is essential.
