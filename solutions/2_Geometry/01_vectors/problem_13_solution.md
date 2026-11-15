# Exercise 13. Do Four Points Lie in One Plane?

## Question

Given

$$
A=(0,0,0),\qquad B=(1,2,0),\qquad C=(0,1,1),\qquad D=(2,5,1).
$$

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Find $n=\overrightarrow{AB}\times\overrightarrow{AC}$.
3. Construct $\overrightarrow{AD}$ and check whether $\overrightarrow{AD}\cdot n=0$.
4. Based on this, decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

> **Why this exercise:** combines the known cross and dot products into a geometric criterion needed for planes, without introducing a separate concept used only once.

## Solution

### Steps

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$:

$$
\overrightarrow{AB} = B - A = (1, 2, 0),
$$

$$
\overrightarrow{AC} = C - A = (0, 1, 1).
$$

2. Compute $n = \overrightarrow{AB}\times\overrightarrow{AC}$:

$$
\begin{aligned}
n_1 &= 2\cdot1 - 0\cdot1 = 2, \\
n_2 &= 0\cdot0 - 1\cdot1 = -1, \\
n_3 &= 1\cdot1 - 2\cdot0 = 1. \\
\end{aligned}
$$

Thus:

$$
n = (2, -1, 1).
$$

3. Construct $\overrightarrow{AD}$ and evaluate $\overrightarrow{AD}\cdot n$:

$$
\overrightarrow{AD} = D - A = (2, 5, 1).
$$

$$
\overrightarrow{AD}\cdot n = 2\cdot2 + 5\cdot(-1) + 1\cdot1 = 4 - 5 + 1 = 0.
$$

4. Decision: Since $\overrightarrow{AD}\cdot n = 0$, point $D$ lies in the plane determined by $A, B$, and $C$.

### Result

The four points $A, B, C$, and $D$ are coplanar.

### Explanation

The normal vector $n = \overrightarrow{AB}\times\overrightarrow{AC}$ is perpendicular to all displacement vectors lying in the plane of $A, B$, and $C$. Point $D$ belongs to this plane if and only if the displacement $\overrightarrow{AD}$ is perpendicular to $n$, which corresponds to $\overrightarrow{AD}\cdot n = 0$. This scalar triple product represents the volume of the parallelepiped spanned by the three vectors; a volume of zero implies the vectors lie in a single plane.
