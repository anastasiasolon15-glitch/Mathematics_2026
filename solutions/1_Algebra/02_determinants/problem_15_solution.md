# Exercise 15. Combining Determinant Properties

## Question

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

## Solution

### Steps

Property 1, multiplicativity: the determinant of a product is the product of the determinants.

$$
\det\left(B^{-1}A^TB\right)=\det(B^{-1})\cdot\det(A^T)\cdot\det B.
$$

Property 2, inverse: $\det(B^{-1})=\dfrac{1}{\det B}=\dfrac{1}{3}$.

Property 3, transpose: $\det(A^T)=\det A=-2$.

Substituting the values:

$$
\begin{aligned}
\det\left(B^{-1}A^TB\right) &= \frac{1}{3}\cdot(-2)\cdot3 \\
&= -2.
\end{aligned}
$$

### Result

$$
\det\left(B^{-1}A^TB\right)=-2.
$$

### Method

The determinants of $B^{-1}$ and $B$ are ordinary numbers, and numbers can be multiplied in any order. Hence the product of the two $B$ factors is $\det(B^{-1})\cdot\det B=\dfrac{1}{3}\cdot3=1$, and only $\det(A^T)=\det A$ remains. This holds for any invertible $B$, so the result does not depend on $B$ at all, and the determinant of $B^{-1}A^TB$ always equals $\det A$.

### Verification

The result is consistent with $\det(B^{-1})\det B=\det(B^{-1}B)=\det I=1$. The size of the matrices does not matter for this argument, only that all three factors are square matrices of the same size, and here that size is $2\times2$.
