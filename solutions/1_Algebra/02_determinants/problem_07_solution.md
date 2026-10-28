# Exercise 7. Using Properties Instead of Recomputing

## Question

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

## Solution

### Steps

For an $n\times n$ matrix, $\det(cA)=c^n\det A$. Here $n=3$.

$$
\det(2A)=2^3\cdot(-4)=8\cdot(-4)=-32.
$$

Transposition does not change the determinant:

$$
\det(A^T)=\det A=-4.
$$

The determinant of a product is the product of determinants:

$$
\det(A^2)=\det A\cdot\det A=(-4)^2=16.
$$

Taking $c=-1$ in the first property:

$$
\det(-A)=(-1)^3\cdot(-4)=4.
$$

### Result

$$
\det(2A)=-32,\qquad \det(A^T)=-4,\qquad \det(A^2)=16,\qquad \det(-A)=4.
$$

### Method

Multiplying a matrix by $c$ multiplies each of its $n$ rows by $c$, and each such row multiplication multiplies the determinant by $c$. This gives the factor $c^n$. The other two rules are the standard properties $\det(A^T)=\det A$ and $\det(AB)=\det A\cdot\det B$.

### Verification

The first and fourth results are consistent with each other and with the factor rule: $\det(2A)=\det(2I)\det A=8\cdot(-4)=-32$, and $\det(-A)=\det(-I)\det A=(-1)\cdot(-4)=4$. The sign of $\det(A^2)$ is positive, as it must be for a square of a real number.
