# Exercise 6. Projection and Perpendicular Component

## Question

Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute

$$
r=u-\mathrm{proj}_v\,u
$$

and verify that $r\cdot v=0$. Explain this result geometrically.

> **Why this exercise:** shows projection as a decomposition into parallel and perpendicular components.

## Solution

### Steps

Compute the projection of $u$ onto $v$:

$$
\mathrm{proj}_v\,u = \left(\frac{u\cdot v}{v\cdot v}\right)v.
$$

Evaluate the scalar products:

$$
u\cdot v = 4\cdot1 + 2\cdot1 = 6,
$$

$$
v\cdot v = 1^2 + 1^2 = 2.
$$

Then:

$$
\mathrm{proj}_v\,u = \frac{6}{2}(1, 1) = 3(1, 1) = (3, 3).
$$

Compute the residual vector $r$:

$$
r = u - \mathrm{proj}_v\,u = (4, 2) - (3, 3) = (1, -1).
$$

### Verification

Evaluate the scalar product $r\cdot v$:

$$
r\cdot v = (1, -1)\cdot(1, 1) = 1\cdot1 + (-1)\cdot1 = 1 - 1 = 0.
$$

The scalar product is zero, confirming that $r$ is perpendicular to $v$.

### Result

$$
\mathrm{proj}_v\,u = (3, 3),\qquad r = (1, -1),\qquad r\cdot v = 0.
$$

### Geometric Interpretation

The projection $\mathrm{proj}_v\,u=(3, 3)$ is the orthogonal projection of $u$ onto the line spanned by $v$, forming the component parallel to $v$. The residual $r=(1, -1)$ connects the head of the projection to the head of $u$. The relation $r\cdot v=0$ confirms that $r$ is perpendicular to the reference direction, establishing the orthogonal decomposition:

$$
u = \mathrm{proj}_v\,u + r.
$$
