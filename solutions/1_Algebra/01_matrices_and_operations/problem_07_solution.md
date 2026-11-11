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

### Neutral elements

Here $I$ is the $2\times2$ identity matrix and $0$ is the $2\times2$ zero matrix. Multiplying by $I$ changes nothing, and adding $0$ changes nothing:

$$
AI=IA=A=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix},\qquad
A+0=A.
$$

So $I$ is the neutral element for multiplication and $0$ is the neutral element for addition.

### Powers

$$
A^2=A\cdot A=
\begin{pmatrix}
4 & 2+2 \\
0 & 4
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix},
$$

$$
A^3=A^2\cdot A=
\begin{pmatrix}
8 & 4+8 \\
0 & 8
\end{pmatrix}
=
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}.
$$

### Pattern

The diagonal entries are $2,\,4,\,8$, that is $2^n$. The upper-right entries are $1,\,4,\,12$, that is $n\cdot2^{n-1}$. This suggests

$$
A^n=
\begin{pmatrix}
2^n & n\,2^{n-1} \\
0 & 2^n
\end{pmatrix},
$$

which matches $n=1,2,3$.
