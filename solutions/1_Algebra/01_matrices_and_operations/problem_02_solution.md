# Matrices and Basic Operations — Exercise 2. Addition and Scalar Multiplication

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

All operations are performed entry by entry.

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}.
$$

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}.
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
\end{pmatrix},
$$

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

## Explanation

Matrices are added by adding entries in the same position. If the matrices had different sizes, some entries would have no partner in the other matrix, so the sum would not be defined. Check: $(A+B)+(A-B)=2A=\begin{pmatrix}2&4\\-2&6\end{pmatrix}$, and indeed $\begin{pmatrix}5&0\\-1&8\end{pmatrix}+\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}=\begin{pmatrix}2&4\\-2&6\end{pmatrix}$.
