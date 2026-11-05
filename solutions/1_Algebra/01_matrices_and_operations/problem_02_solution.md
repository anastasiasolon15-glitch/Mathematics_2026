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

### Why matrices must be of the same size for addition
Matrix addition is defined entry by entry (element-wise), meaning that corresponding entries in the same position are added together. If two matrices had different sizes, some entries would have no corresponding partner in the other matrix, making the sum undefined.

### Verification Check
We can check our results using the property $(A+B)+(A-B)=2A$:

$$
(A+B) + (A-B) = 
\begin{pmatrix}
5 & 0 \\
-1 & 8 
\end{pmatrix} + 
\begin{pmatrix}
-3 & 4 \\
-1 & -2 
\end{pmatrix} = 
\begin{pmatrix}
2 & 4 \\
-2 & 6 
\end{pmatrix}
$$

And for $2A$:

$$
2A = 2 \begin{pmatrix} 1 & 2 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix} 2 & 4 \\ -2 & 6 \end{pmatrix}.
$$

Since both results match, the calculations are correct.
