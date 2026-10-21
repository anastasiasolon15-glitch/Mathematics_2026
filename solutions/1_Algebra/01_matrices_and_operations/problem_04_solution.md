# Exercise 4. Matrix Multiplication and Noncommutativity

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

### Steps

Each entry of a product is the dot product of a row of the left factor with a column of the right factor.

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
BA &=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
AB=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix},\qquad
BA=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix},\qquad
AB\neq BA.
$$

### Method

Both products are defined and have the same size, yet they differ. Noncommutativity means that in general $AB\neq BA$, so the order of factors cannot be swapped. One counterexample, such as this one, is enough to show that the property fails in general. (For some special pairs of matrices the equality does hold, see Exercise 11.)

### Verification

The entries in position $(1,1)$ already differ: $8\neq2$. The trace and the determinant of the two products agree, as they should for these invariants:

$$
\mathrm{tr}(AB)=8+1=9=2+7=\mathrm{tr}(BA),
$$

$$
\det(AB)=8\cdot1-2\cdot3=2=2\cdot7-4\cdot3=\det(BA).
$$

Thus $AB$ and $BA$ are different matrices that share these invariants.
