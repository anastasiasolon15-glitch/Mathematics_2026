# Exercise 1. Definition of the Inverse

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

### Steps

By definition, $B=A^{-1}$ if and only if $AB=I$ and $BA=I$.

$$
\begin{aligned}
AB &=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
BA &=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
-1\cdot2+2\cdot1 & -1\cdot1+2\cdot1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
AB=BA=I,
$$

so $B=A^{-1}$.

### Method

The inverse of $A$ is a matrix that undoes $A$ from both sides. Both products must give the identity matrix, and for square matrices one of them already implies the other. Here both were computed.

### Verification

The inverse is unique, so no other matrix can satisfy the definition for $A$. As an independent check, $\det A=2\cdot1-1\cdot1=1\neq0$, so $A$ is invertible, which is consistent with the existence of $B$.
