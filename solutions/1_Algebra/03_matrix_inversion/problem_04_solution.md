# Exercise 4. Gauss–Jordan

## Question

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

### Steps

Start with the augmented matrix:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

Step 1, $R_2\leftarrow R_2-3R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

Step 2, $R_2\leftarrow -R_2$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Step 3, $R_1\leftarrow R_1-2R_2$:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

### Result

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$

### Method

Every row operation is multiplication from the left by an invertible elementary matrix. If $E$ is the product of all the elementary matrices used, then $EA=I$ and $EI=E$. The first equality says $E=A^{-1}$, and the second says that the right block of the augmented matrix is exactly $E$. So the same operations that turn $A$ into $I$ turn $I$ into $A^{-1}$.

### Verification

$$
\begin{aligned}
AA^{-1} &=
\begin{pmatrix}
1\cdot(-5)+2\cdot3 & 1\cdot2+2\cdot(-1) \\
3\cdot(-5)+5\cdot3 & 3\cdot2+5\cdot(-1) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$

The $2\times2$ formula agrees: $\det A=5-6=-1$, so

$$
A^{-1}=\frac{1}{-1}
\begin{pmatrix}
5 & -2 \\
-3 & 1 \\
\end{pmatrix}.
$$
