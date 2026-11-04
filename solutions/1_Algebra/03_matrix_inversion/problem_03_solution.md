# Exercise 3. When Does the Inverse Not Exist?

## Question

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Solution

### Steps

Way 1, the determinant:

$$
\det A=2\cdot2-4\cdot1=0.
$$

A square matrix is invertible if and only if its determinant is nonzero, so $A^{-1}$ does not exist.

Way 2, dependence of rows. The first row is twice the second row:

$$
(2,\ 4)=2\cdot(1,\ 2).
$$

Hence $R_1-2R_2=0$ is a nontrivial linear dependence between the rows.

### Result

$A$ is not invertible, because $\det A=0$ and, equivalently, its rows are linearly dependent.

### Method

The two arguments describe the same fact. Dependent rows mean that row operations can produce a zero row, and a matrix with a zero row has determinant $0$. Moreover, every product $XA$ has rows that are combinations of the rows of $A$, so $XA$ also has dependent rows and can never equal $I$, whose rows are independent.

### Verification

Try to find a matrix $X$ with $AX=I$. The rows of $AX$ are $R_1(A)X$ and $R_2(A)X$, and because $R_1(A)=2R_2(A)$, the first row of $AX$ is twice the second row. For $I$ this is false, since $(1,0)\neq2\cdot(0,1)$. So no such $X$ exists.
