# Matrices and Basic Operations — Exercise 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

## Solution

### Direct computation

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
8-2 \\
4+6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

### Linear combination of columns

The columns of $A$ are $a_1=\begin{pmatrix}2\\1\end{pmatrix}$ and $a_2=\begin{pmatrix}-1\\3\end{pmatrix}$. The coefficients are the entries of $x$:

$$
Ax = 4\begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2\begin{pmatrix} -1 \\ 3 \end{pmatrix} =
\begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} =
\begin{pmatrix} 6 \\ 10 \end{pmatrix}.
$$

## Explanation

In general, $Ax = x_1a_1 + x_2a_2$: the vector $Ax$ is a linear combination of the columns of $A$ with weights given by the entries of $x$. Both methods yield the exact same vector $\begin{pmatrix} 6 \\ 10 \end{pmatrix}$, which verifies the correctness of the result.
