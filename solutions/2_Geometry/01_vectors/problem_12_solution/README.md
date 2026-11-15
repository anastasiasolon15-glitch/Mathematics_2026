# Exercise 12. A Normal Vector to a Plane

## Question

Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$. Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

> **Why this exercise:** creates a direct bridge from vectors to the description of a plane.

## Solution

### Steps

Construct two in-plane displacement vectors from point $A$:

$$
\overrightarrow{AB} = B - A = (2-1,\; 1-0,\; 0-2) = (1, 1, -2),
$$

$$
\overrightarrow{AC} = C - A = (0-1,\; 3-0,\; 1-2) = (-1, 3, -1).
$$

Compute a normal vector $n = \overrightarrow{AB}\times\overrightarrow{AC}$:

$$
\begin{aligned}
n_1 &= 1\cdot(-1) - (-2)\cdot3 = -1 + 6 = 5, \\
n_2 &= (-2)\cdot(-1) - 1\cdot(-1) = 2 + 1 = 3, \\
n_3 &= 1\cdot3 - 1\cdot(-1) = 3 + 1 = 4. \\
\end{aligned}
$$

Thus:

$$
n = (5, 3, 4).
$$

### Verification

Evaluate scalar products to confirm perpendicularity:

$$
n\cdot\overrightarrow{AB} = 5\cdot1 + 3\cdot1 + 4\cdot(-2) = 5 + 3 - 8 = 0,
$$

$$
n\cdot\overrightarrow{AC} = 5\cdot(-1) + 3\cdot3 + 4\cdot(-1) = -5 + 9 - 4 = 0.
$$

Both scalar products vanish, confirming that $n$ is perpendicular to both in-plane vectors.

### Result

Two in-plane vectors are $\overrightarrow{AB}=(1, 1, -2)$ and $\overrightarrow{AC}=(-1, 3, -1)$. A normal vector to the plane is $n=(5, 3, 4)$.

### Explanation

In three dimensions, any plane can be characterized by a point and a normal vector perpendicular to every displacement within the plane. The cross product of two non-collinear in-plane vectors yields this normal vector directly.
