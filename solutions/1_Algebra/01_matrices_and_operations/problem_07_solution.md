# Exercise 7. Identity Matrix, Zero Matrix, and Powers

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

### Steps

Here $I$ is the $2\times2$ identity matrix and $0$ is the $2\times2$ zero matrix.

$$
\begin{aligned}
AI &=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\end{aligned}
$$

Similarly $IA=A$ and $A+0=A$.

Powers:

$$
\begin{aligned}
A^2 &=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
A^3=A^2A &=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
AI=IA=A,\qquad A+0=A,
$$

$$
A^2=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},\qquad
A^3=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

### Method

The identity matrix $I$ is neutral for multiplication ($AI=IA=A$), and the zero matrix $0$ is neutral for addition ($A+0=A$).

Observed pattern: the diagonal entries are $2,4,8$, that is $2^n$, and the upper right entries are $1,4,12$, that is $n\cdot2^{n-1}$. Hence

$$
A^n=
\begin{pmatrix}
2^n & n\cdot2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

The pattern follows from the decomposition $A=2I+N$ with

$$
N=
\begin{pmatrix}
0 & 1 \\
0 & 0 \\
\end{pmatrix},\qquad N^2=0.
$$

Since $I$ commutes with $N$, the binomial formula gives $A^n=2^nI+n\cdot2^{n-1}N$.

### Verification

The formula reproduces the computed powers: for $n=2$ it gives $2^2=4$ and $2\cdot2=4$, and for $n=3$ it gives $2^3=8$ and $3\cdot4=12$. Computing $A^3=AA^2$ in the other order gives the same matrix:

$$
\begin{aligned}
AA^2 &=
\begin{pmatrix}
2\cdot4+1\cdot0 & 2\cdot4+1\cdot4 \\
0\cdot4+2\cdot0 & 0\cdot4+2\cdot4 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
\end{aligned}
$$
