### Exercise 12. Homogeneous System

## Question

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

For a homogeneous system the right-hand side stays zero during elimination, so it is enough to reduce the coefficient matrix. Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & -2 \\
1 & -1 & 2
\end{pmatrix}
\to
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 0 \\
0 & -3 & 3
\end{pmatrix}.
$$

From the third row: $-3y+3z=0$, so $y=z$. From the first row: $x=-2y+z=-z$. The variable $z$ is free; put $z=t$:

$$
(x,y,z)=t(-1,\,1,\,1),\qquad t\in\mathbb{R}.
$$

**Verification.** For $t=1$ we get $(-1,1,1)$: $-1+2-1=0$, $-2+4-2=0$, $-1-1+2=0$.

**Why $(0,0,0)$ always works.** Every equation has the form $a_1x+a_2y+a_3z=0$. Substituting zeros gives $0=0$, so the zero vector (the trivial solution) is always a solution. Here there are also nonzero solutions, because there is a free variable.
