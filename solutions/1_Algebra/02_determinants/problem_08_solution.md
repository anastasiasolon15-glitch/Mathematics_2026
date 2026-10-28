# Exercise 8. Determinant of a Product

## Question

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

## Solution

### Steps

The determinant is multiplicative, so

$$
\det(AB)=\det A\cdot\det B=3\cdot(-5)=-15.
$$

$$
\det(BA)=\det B\cdot\det A=(-5)\cdot3=-15.
$$

Since $\det A=3\neq0$, the matrix $A$ is invertible and $A^{-1}$ exists, with $\det(A^{-1})=\dfrac{1}{\det A}=\dfrac{1}{3}$. Then

$$
\det(A^{-1}B)=\det(A^{-1})\cdot\det B=\frac{1}{3}\cdot(-5)=-\frac{5}{3}.
$$

### Result

$$
\det(AB)=-15,\qquad \det(BA)=-15,\qquad \det(A^{-1}B)=-\frac{5}{3}.
$$

### Method

The matrices $AB$ and $BA$ are in general different matrices, but their determinants are products of the same two real numbers $\det A$ and $\det B$. Multiplication of numbers is commutative, so the determinants are equal. The determinant forgets most of the information about a matrix and keeps only one number.

The formula $\det(A^{-1})=1/\det A$ follows from $\det(A^{-1})\det A=\det I=1$.

### Verification

Multiplying the last result by $\det A$ should return $\det B$:

$$
\det(A^{-1}B)\cdot\det A=-\frac{5}{3}\cdot3=-5=\det B.
$$

This agrees with $\det(AA^{-1}B)=\det B$.
