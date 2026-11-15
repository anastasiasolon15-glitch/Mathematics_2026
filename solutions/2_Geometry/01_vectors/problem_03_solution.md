# Exercise 3. Vector Normalization

## Question

For $v=(3,4)$ find a unit vector $e$ with the same direction and orientation. Check that $\|e\|=1$, reconstruct $v$ in the form $v=\|v\|e$, and explain what changes during normalization and what remains unchanged.

> **Why this exercise:** teaches how to separate direction from vector length.

## Solution

### Steps

Compute the Euclidean length of $v$:

$$
\|v\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5.
$$

Scale $v$ by the reciprocal of its length to obtain the unit vector $e$:

$$
e = \frac{v}{\|v\|} = \frac{1}{5}(3, 4) = \left(\frac{3}{5}, \frac{4}{5}\right).
$$

### Verification

Check the length of $e$:

$$
\|e\| = \sqrt{\left(\frac{3}{5}\right)^2 + \left(\frac{4}{5}\right)^2} = \sqrt{\frac{9}{25} + \frac{16}{25}} = \sqrt{\frac{25}{25}} = 1.
$$

Reconstruct $v$ from $\|v\|$ and $e$:

$$
\|v\|e = 5\left(\frac{3}{5}, \frac{4}{5}\right) = (3, 4) = v.
$$

### Result

The unit vector is:

$$
e = \left(\frac{3}{5}, \frac{4}{5}\right).
$$

### Explanation

During normalization:
- The magnitude changes: the original length $\|v\|=5$ is scaled to $1$.
- The direction and orientation remain unchanged: dividing by the strictly positive scalar $\|v\|=5>0$ preserves the line of action and does not reverse the sense of the vector.

Normalization decomposes a nonzero vector into two independent factors: magnitude $\|v\|$ and direction $e$.
