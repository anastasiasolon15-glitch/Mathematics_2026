# Exercise 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

## Solution

### Steps

The condition $A^2=I$ means $A\cdot A=I$. This is exactly the definition of the inverse with $B=A$: the matrix $A$ multiplied by $A$ from either side gives $I$. Since the inverse of a matrix is unique, $A^{-1}=A$.

Example:

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Then

$$
\begin{aligned}
A^2 &=
\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

If $A^2=I$, then $A^{-1}=A$. The matrix above is an example with $A\neq I$ and $A\neq-I$.

### Method

The proof uses only the definition of the inverse and its uniqueness. Geometrically, the example is the reflection across the line $y=x$, which swaps the coordinates. Reflecting twice returns every vector to its place, so the reflection is its own inverse.

### Verification

Another example is

$$
B=
\begin{pmatrix}
1 & 0 \\
0 & -1 \\
\end{pmatrix},\qquad B^2=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

For the first example the $2\times2$ formula also agrees: $\det A=-1$, so

$$
A^{-1}=\frac{1}{-1}
\begin{pmatrix}
0 & -1 \\
-1 & 0 \\
\end{pmatrix}=A.
$$
