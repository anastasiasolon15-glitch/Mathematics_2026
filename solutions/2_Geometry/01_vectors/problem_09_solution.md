# Exercise 9. Cross Product as a Perpendicular Direction

## Question

For $u=(1,2,0)$ and $v=(0,1,3)$ compute $u\times v$. Use dot products to check perpendicularity to both vectors, compute $v\times u$, and compare the results.

> **Why this exercise:** teaches the geometric meaning of the cross product and the effect of changing the order of its arguments.

## Solution

### Steps

Compute the components of $u\times v$:

$$
\begin{aligned}
(u\times v)_1 &= 2\cdot3 - 0\cdot1 = 6, \\
(u\times v)_2 &= 0\cdot0 - 1\cdot3 = -3, \\
(u\times v)_3 &= 1\cdot1 - 2\cdot0 = 1. \\
\end{aligned}
$$

Thus:

$$
u\times v = (6, -3, 1).
$$

Compute the components of $v\times u$:

$$
\begin{aligned}
(v\times u)_1 &= 1\cdot0 - 3\cdot2 = -6, \\
(v\times u)_2 &= 3\cdot1 - 0\cdot0 = 3, \\
(v\times u)_3 &= 0\cdot2 - 1\cdot1 = -1. \\
\end{aligned}
$$

Thus:

$$
v\times u = (-6, 3, -1).
$$

### Verification

Evaluate scalar products to check perpendicularity:

$$
(u\times v)\cdot u = 6\cdot1 + (-3)\cdot2 + 1\cdot0 = 6 - 6 + 0 = 0,
$$

$$
(u\times v)\cdot v = 6\cdot0 + (-3)\cdot1 + 1\cdot3 = 0 - 3 + 3 = 0.
$$

Both scalar products vanish, confirming that $u\times v$ is perpendicular to both $u$ and $v$.

### Result

$$
u\times v = (6, -3, 1),\qquad v\times u = (-6, 3, -1) = -(u\times v).
$$

### Explanation

The cross product is anticommutative: $v\times u = -(u\times v)$. Reversing the order of arguments preserves the magnitude and line of action of the resulting vector while inverting its direction along that line.
