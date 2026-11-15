# Exercise 4. Dot Product and Perpendicularity

## Question

For $u=(1,2,-1)$ and $v=(2,-1,3)$ compute $u\cdot v$ and determine whether the vectors are perpendicular. Then find $a$ so that $w=(2,-1,a)$ is perpendicular to $u$, and check the result.

> **Why this exercise:** shows the dot product as both a test and a tool for constructing a perpendicularity condition.

## Solution

### Steps

Compute the scalar product $u\cdot v$:

$$
u\cdot v = 1\cdot2 + 2\cdot(-1) + (-1)\cdot3 = 2 - 2 - 3 = -3.
$$

Two nonzero vectors are perpendicular if and only if their scalar product is zero. Since $u\cdot v = -3 \neq 0$, the vectors $u$ and $v$ are not perpendicular.

Find $a$ such that $w=(2, -1, a)$ satisfies $u\cdot w = 0$:

$$
u\cdot w = 1\cdot2 + 2\cdot(-1) + (-1)\cdot a = 2 - 2 - a = -a.
$$

Setting $-a = 0$ gives:

$$
a = 0.
$$

Thus $w = (2, -1, 0)$.

### Verification

Evaluate $u\cdot w$ for $w=(2, -1, 0)$:

$$
u\cdot w = 1\cdot2 + 2\cdot(-1) + (-1)\cdot0 = 2 - 2 + 0 = 0.
$$

The scalar product is zero, confirming that $w$ is perpendicular to $u$.

### Result

The vectors $u$ and $v$ are not perpendicular ($u\cdot v = -3$). The required value is $a = 0$, giving $w = (2, -1, 0)$.

### Explanation

The dot product translates geometric perpendicularity directly into an algebraic condition: $u\perp w \iff u\cdot w = 0$. This provides both a verification test and an equation for solving unknown parameters.
