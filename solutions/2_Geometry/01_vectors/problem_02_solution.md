# Exercise 2. Distance as the Length of a Vector

## Question

The points are $A=(1,2,3)$ and $B=(4,-2,6)$.

1. Construct $\overrightarrow{AB}$.
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

> **Why this exercise:** shows that the point-distance formula comes directly from the length of a difference vector.

## Solution

### Steps

1. Construct the displacement vector $\overrightarrow{AB}$:

$$
\overrightarrow{AB} = B - A = (4-1,\; -2-2,\; 6-3) = (3, -4, 3).
$$

2. Compute the Euclidean length of $\overrightarrow{AB}$:

$$
\|\overrightarrow{AB}\| = \sqrt{3^2 + (-4)^2 + 3^2} = \sqrt{9 + 16 + 9} = \sqrt{34}.
$$

3. Compute the distance $d(A, B)$ using the coordinate distance formula:

$$
d(A, B) = \sqrt{(4-1)^2 + (-2-2)^2 + (6-3)^2} = \sqrt{3^2 + (-4)^2 + 3^2} = \sqrt{34}.
$$

### Result

$$
\overrightarrow{AB} = (3, -4, 3),\qquad \|\overrightarrow{AB}\| = \sqrt{34},\qquad d(A, B) = \sqrt{34}.
$$

### Explanation

Both calculations yield the identical result because the distance between two points in Euclidean space is defined as the geometric length of the displacement vector connecting them:

$$
\overrightarrow{AB} = (\Delta x,\; \Delta y,\; \Delta z) = (x_B - x_A,\; y_B - y_A,\; z_B - z_A).
$$

Applying the three-dimensional Pythagorean theorem to the component differences gives:

$$
\|\overrightarrow{AB}\| = \sqrt{(\Delta x)^2 + (\Delta y)^2 + (\Delta z)^2} = d(A, B).
$$

The coordinate distance formula is directly the Euclidean norm of the difference vector $\overrightarrow{AB} = B - A$.
