# Exercise 1. Vector Operations and Their Meaning

## Question

For $u=(2,-1,3)$ and $v=(-1,4,2)$ compute

$$
u+v,\qquad u-v,\qquad 3u-2v.
$$

Then verify that $(u+v)-v=u$, and explain geometrically what adding two vectors means.

> **Why this exercise:** reinforces basic operations and immediately connects them with their geometric meaning.

## Solution

### Steps

Vector operations are performed component by component.

Compute $u+v$:

$$
u+v = (2+(-1),\; -1+4,\; 3+2) = (1, 3, 5).
$$

Compute $u-v$:

$$
u-v = (2-(-1),\; -1-4,\; 3-2) = (3, -5, 1).
$$

Compute $3u-2v$:

$$
3u = (6, -3, 9),\qquad 2v = (-2, 8, 4),
$$

$$
3u-2v = (6-(-2),\; -3-8,\; 9-4) = (8, -11, 5).
$$

### Verification

Substitute the computed sum $u+v=(1, 3, 5)$ and $v=(-1, 4, 2)$:

$$
(u+v)-v = (1, 3, 5) - (-1, 4, 2) = (1-(-1),\; 3-4,\; 5-2) = (2, -1, 3) = u.
$$

The identity holds algebraically.

### Result

$$
u+v = (1, 3, 5),\qquad u-v = (3, -5, 1),\qquad 3u-2v = (8, -11, 5).
$$

### Geometric Interpretation

Geometrically, adding two vectors corresponds to concatenating displacements:
- Under the tip-to-tail rule, placing the tail of $v$ at the tip of $u$ yields a vector $u+v$ running from the tail of $u$ to the tip of $v$.
- Under the parallelogram rule, $u+v$ is the directed main diagonal of the parallelogram formed by $u$ and $v$ with a shared initial point.

The identity $(u+v)-v=u$ reflects that translating by $v$ and subsequently by $-v$ cancels the displacement $v$, returning to the tip of $u$.
