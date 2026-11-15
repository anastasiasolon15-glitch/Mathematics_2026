# Exercise 7. Linear Dependence Without Heavy Computation

## Question

Given

$$
u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1).
$$

Identify a specific relation between $u$ and $v$, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

> **Why this exercise:** develops the habit of recognizing structure before applying a computational procedure.

## Solution

### Steps

Comparing components of $u$ and $v$:

$$
v = (2, 4, 6) = 2(1, 2, 3) = 2u.
$$

This relation can be written as:

$$
2u - v + 0w = \mathbf{0}.
$$

Because there exists a linear combination with coefficients $(2, -1, 0) \neq (0, 0, 0)$ equal to the zero vector, the set $\{u, v, w\}$ is linearly dependent.

### Result

The relation between $u$ and $v$ is $v = 2u$. The three vectors $\{u, v, w\}$ are linearly dependent.

### Explanation

No Gaussian elimination or determinant calculation is required:
1. Two vectors are linearly dependent if and only if one is a scalar multiple of the other. The relation $v=2u$ establishes that $\{u, v\}$ is linearly dependent.
2. Any set containing a linearly dependent subset is itself linearly dependent. The additional vector $w$ cannot eliminate the linear dependence already present between $u$ and $v$.
