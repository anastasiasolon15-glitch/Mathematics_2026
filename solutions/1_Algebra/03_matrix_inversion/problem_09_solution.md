# Exercise 9. Matrix Equation

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

### Steps

In $AX=B$ the matrix $A$ stands to the left of $X$. To cancel it, $A^{-1}$ must be multiplied from the left on both sides:

$$
A^{-1}(AX)=A^{-1}B,\qquad\text{so}\qquad X=A^{-1}B.
$$

Since $\det A=1$,

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$

Then

$$
\begin{aligned}
X=A^{-1}B &=
\begin{pmatrix}
1\cdot3-2\cdot2 & 1\cdot1-2\cdot4 \\
2 & 4 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

$$
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$

### Method

Matrix multiplication is not commutative, so $A^{-1}$ has to be placed on the same side as $A$ appears in the equation. Multiplying from the right would give $BA^{-1}$, which is a different matrix and does not solve $AX=B$.

### Verification

$$
\begin{aligned}
AX &=
\begin{pmatrix}
1\cdot(-1)+2\cdot2 & 1\cdot(-7)+2\cdot4 \\
2 & 4 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=B.
\end{aligned}
$$
