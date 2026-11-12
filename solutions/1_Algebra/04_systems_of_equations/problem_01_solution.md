### Exercise 1. From a System to a Matrix

## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7
\end{cases}
$$

in the form $Ax=b$. Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

The coefficients of the unknowns $x,y,z$ in each equation form one row of the coefficient matrix, and the right-hand sides form the vector $b$:

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix},\qquad
x=
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix},\qquad
b=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}.
$$

So the system is

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}.
$$

**Verification.** Multiplying row by row (dot product of a row of $A$ with the vector of unknowns) gives
$2x-y+z$, $\;x+3y-2z$, $\;3x+y+z$, which are exactly the left-hand sides of the three equations. Hence row $i$ of $A$ together with entry $b_i$ encodes the $i$-th equation, and $Ax=b$ is equivalent to the original system.
