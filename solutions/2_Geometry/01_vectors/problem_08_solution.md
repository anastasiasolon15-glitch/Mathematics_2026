# Exercise 8. Linear Combination and Checking the Result

## Question

Check whether $w=(5,1)$ can be written as

$$
w=au+bv,
$$

where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$ from them, and explain the geometric meaning of the existence of such coefficients.

> **Why this exercise:** connects linear combinations with the geometry of directions.

## Solution

### Steps

Equating coordinates in $w = au + bv$ gives the system of linear equations:

$$
\begin{cases}
a + 2b = 5, \\
a - b = 1. \\
\end{cases}
$$

Subtract the second equation from the first:

$$
3b = 4 \implies b = \frac{4}{3}.
$$

Substitute $b = \frac{4}{3}$ into the second equation:

$$
a = 1 + b = 1 + \frac{4}{3} = \frac{7}{3}.
$$

### Verification

Reconstruct $w$ from the computed coefficients:

$$
au + bv = \frac{7}{3}(1, 1) + \frac{4}{3}(2, -1) = \left(\frac{7}{3} + \frac{8}{3},\; \frac{7}{3} - \frac{4}{3}\right) = \left(\frac{15}{3},\; \frac{3}{3}\right) = (5, 1) = w.
$$

The reconstruction confirms the coefficients.

### Result

$$
a = \frac{7}{3},\qquad b = \frac{4}{3}.
$$

### Geometric Meaning

Because $u$ and $v$ are not parallel ($1\cdot(-1) - 1\cdot2 = -3 \neq 0$), they span the entire plane $\mathbb{R}^2$ and form a basis. The coefficients $(a, b) = (7/3, 4/3)$ are the coordinates of $w$ in this basis, representing the unique combination of displacements along directions $u$ and $v$ needed to reach $w$.
