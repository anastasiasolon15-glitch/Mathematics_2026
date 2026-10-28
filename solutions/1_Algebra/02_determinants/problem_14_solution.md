# Exercise 14. A System of Equations and the Determinant

## Question

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

### Steps

The determinant of the coefficient matrix is

$$
\det A=1\cdot4-2\cdot k=4-2k.
$$

If $\det A\neq0$, that is $k\neq2$, then $A$ is invertible and $x=A^{-1}b$ is the unique solution for every $b$.

If $k=2$, then $\det A=0$ and

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix}.
$$

The system $Ax=b$ with $b=(b_1,b_2)$ reads

$$
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2.
\end{cases}
$$

The second equation is twice the left side of the first equation. Hence the system is consistent exactly when $b_2=2b_1$.

Example with infinitely many solutions, $b=(1,2)$:

$$
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=2.
\end{cases}
$$

Both equations say the same thing, so every pair with $x_1=1-2x_2$ is a solution.

Example with no solution, $b=(1,0)$:

$$
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=0.
\end{cases}
$$

The second equation gives $x_1+2x_2=0$, which contradicts the first equation.

### Result

The system has exactly one solution for every $b$ if and only if $k\neq2$. For $k=2$ the choice $b=(1,2)$ gives infinitely many solutions, and the choice $b=(1,0)$ gives no solution.

### Method

For a square matrix, $\det A\neq0$ means that $A$ is invertible, and then $Ax=b$ has exactly one solution for each $b$. When $\det A=0$, the columns of $A$ are dependent, so the vectors $Ax$ fill only a line. A right-hand side $b$ on this line gives infinitely many solutions, and a right-hand side off this line gives none.

### Verification

For $b=(1,2)$ two different solutions are $x=(1,0)$ and $x=(-1,1)$. Check for the second: $-1+2\cdot1=1$ and $2\cdot(-1)+4\cdot1=2$, which matches $b$. For $b=(1,0)$ the vector $b$ is not on the line spanned by the column $(1,2)$ of $A$, since $b_2\neq2b_1$, so no solution exists.
