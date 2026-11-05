# Matrices and Basic Operations — Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

## Solution

With $I=\begin{pmatrix}1&0\\0&1\end{pmatrix}$ and $0=\begin{pmatrix}0&0\\0&0\end{pmatrix}$:

$$
AI=IA=A+0=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$

$$
A^2=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}.
$$

$$
A^3=A^2A=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0 & 4\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

## Explanation

$I$ is the neutral element for multiplication ($AI=IA=A$), and $0$ is the neutral element for addition ($A+0=A$).

Pattern: the diagonal entries are $2,4,8$, that is $2^n$, and the upper right entries are $1,4,12$, that is $n\cdot2^{n-1}$. So

$$
A^n=
\begin{pmatrix}
2^n & n\cdot2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

Check: for $n=2$ we get $2^2=4$ and $2\cdot2=4$; for $n=3$ we get $2^3=8$ and $3\cdot4=12$, matching the computed matrices.
