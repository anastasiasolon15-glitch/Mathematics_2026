# Exercise 2. Addition and Scalar Multiplication

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

## Solution

### Steps

Addition, subtraction and scalar multiplication are performed entry by entry.

$$
\begin{aligned}
A+B &=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
A-B &=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
\end{aligned}
$$

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},\qquad
2B=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
$$

$$
\begin{aligned}
3A-2B &=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
A+B=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix},\qquad
A-B=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix},\qquad
3A-2B=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

### Method

The entry in position $(i,j)$ of $A+B$ is defined as $a_{ij}+b_{ij}$. This requires that both matrices have an entry in every position $(i,j)$. If the sizes differ, some position exists in one matrix but has no counterpart in the other, so the sum is not defined.

### Verification

The sum of the two results should be $2A$:

$$
\begin{aligned}
(A+B)+(A-B) &=
\begin{pmatrix}
2 & 4 \\
-2 & 6 \\
\end{pmatrix} \\
&= 2A.
\end{aligned}
$$

The identity $3A-2B=3(A-B)+B$ gives the same result:

$$
\begin{aligned}
3(A-B)+B &=
\begin{pmatrix}
-9 & 12 \\
-3 & -6 \\
\end{pmatrix}
+
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
\end{aligned}
$$
