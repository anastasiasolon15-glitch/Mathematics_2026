# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

### Steps

Property 1: $(cA)^{-1}=\frac1c A^{-1}$ for $c\neq0$.

$$
(3A)^{-1}=\frac13
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix}.
$$

Property 2: $(A^T)^{-1}=(A^{-1})^T$.

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}.
$$

Property 3: $(A^2)^{-1}=(A^{-1})^2$, which follows from the inverse of a product, $(AA)^{-1}=A^{-1}A^{-1}$.

$$
\begin{aligned}
(A^2)^{-1} &=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

$$
(3A)^{-1}=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix},\qquad
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix},\qquad
(A^2)^{-1}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
$$

### Method

Each property is checked by multiplying with the original matrix: $(3A)\cdot\frac13A^{-1}=AA^{-1}=I$, $A^T(A^{-1})^T=(A^{-1}A)^T=I^T=I$, and $A^2A^{-1}A^{-1}=A(AA^{-1})A^{-1}=I$.

### Verification

The matrix $A^{-1}$ has determinant $2\cdot2-(-1)(-3)=1$. Then $\det A=1$ as well, and $\det(A^2)=1$. The matrix $(A^2)^{-1}$ should have determinant $1$, and indeed $7\cdot7-(-4)(-12)=49-48=1$.
