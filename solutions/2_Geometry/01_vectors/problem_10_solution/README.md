# Exercise 10. Triangle Area from Vectors

## Question

The points $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$ form a triangle. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor $\frac12$.

> **Why this exercise:** shows the interpretation of the length of the cross product as area.

## Solution

### Steps

Construct the side vectors:

$$
\overrightarrow{AB} = B - A = (2, 1, 0),
$$

$$
\overrightarrow{AC} = C - A = (1, 3, 2).
$$

Compute the cross product $\overrightarrow{AB}\times\overrightarrow{AC}$:

$$
\begin{aligned}
(\overrightarrow{AB}\times\overrightarrow{AC})_1 &= 1\cdot2 - 0\cdot3 = 2, \\
(\overrightarrow{AB}\times\overrightarrow{AC})_2 &= 0\cdot1 - 2\cdot2 = -4, \\
(\overrightarrow{AB}\times\overrightarrow{AC})_3 &= 2\cdot3 - 1\cdot1 = 5. \\
\end{aligned}
$$

Thus:

$$
\overrightarrow{AB}\times\overrightarrow{AC} = (2, -4, 5).
$$

Compute the area of the parallelogram:

$$
S_{\mathrm{parallelogram}} = \|\overrightarrow{AB}\times\overrightarrow{AC}\| = \sqrt{2^2 + (-4)^2 + 5^2} = \sqrt{4 + 16 + 25} = \sqrt{45} = 3\sqrt{5}.
$$

Compute the area of the triangle:

$$
S_{\triangle ABC} = \frac{1}{2}\|\overrightarrow{AB}\times\overrightarrow{AC}\| = \frac{3\sqrt{5}}{2}.
$$

### Result

The area of the parallelogram is $3\sqrt{5}$, and the area of the triangle is $\frac{3\sqrt{5}}{2}$.

### Explanation

The norm of the cross product equals $\|\overrightarrow{AB}\|\,\|\overrightarrow{AC}\|\sin\theta$, representing the base times height of the parallelogram spanned by $\overrightarrow{AB}$ and $\overrightarrow{AC}$. The diagonal segment $BC$ divides this parallelogram into two congruent triangles of equal area, which explains the factor $\frac{1}{2}$.
