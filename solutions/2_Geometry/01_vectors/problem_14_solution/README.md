# Exercise 14. Closest Point on a Line

## Question

Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$. Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

> **Why this exercise:** shows projection as a complete solution to a minimum-distance problem.

## Solution

### Steps

Let $p=(4, 1)$ be the position vector of point $P$. The line through the origin in direction $v=(1, 2)$ consists of all points of the form $tv$ for $t\in\mathbb{R}$.

Compute the projection of $p$ onto the direction $v$:

$$
\mathrm{proj}_v\,p = \left(\frac{p\cdot v}{v\cdot v}\right)v.
$$

Evaluate the scalar products:

$$
p\cdot v = 4\cdot1 + 1\cdot2 = 6,
$$

$$
v\cdot v = 1^2 + 2^2 = 5.
$$

The position vector of the closest point $Q$ on the line is:

$$
Q = \mathrm{proj}_v\,p = \frac{6}{5}(1, 2) = \left(\frac{6}{5}, \frac{12}{5}\right).
$$

Compute the displacement vector from $Q$ to $P$:

$$
\overrightarrow{QP} = P - Q = (4, 1) - \left(\frac{6}{5}, \frac{12}{5}\right) = \left(\frac{14}{5}, -\frac{7}{5}\right).
$$

Compute the distance $d$ from $P$ to the line as the norm of $\overrightarrow{QP}$:

$$
d = \|\overrightarrow{QP}\| = \sqrt{\left(\frac{14}{5}\right)^2 + \left(-\frac{7}{5}\right)^2} = \sqrt{\frac{196 + 49}{25}} = \sqrt{\frac{245}{25}} = \frac{7\sqrt{5}}{5}.
$$

### Verification

Verify that the displacement $\overrightarrow{QP}$ is perpendicular to the line direction $v$:

$$
\overrightarrow{QP}\cdot v = \frac{14}{5}\cdot1 + \left(-\frac{7}{5}\right)\cdot2 = \frac{14}{5} - \frac{14}{5} = 0.
$$

The scalar product is zero, confirming that $\overrightarrow{QP}$ is perpendicular to $v$.

### Result

The closest point on the line is $Q = (6/5, 12/5)$, and the distance from $P$ to the line is $\frac{7\sqrt{5}}{5}$.

### Explanation

For any point $X$ on the line other than $Q$, the displacement $\overrightarrow{QX}$ is collinear with $v$. Since $\overrightarrow{QP}\perp v$, the triangle $\triangle PQX$ is a right triangle with right angle at $Q$ and hypotenuse $PX$. By the Pythagorean theorem:

$$
\|P - X\|^2 = \|\overrightarrow{QP}\|^2 + \|\overrightarrow{QX}\|^2.
$$

Because $X \neq Q$, $\|\overrightarrow{QX}\|^2 > 0$, which yields:

$$
\|P - X\| > \|\overrightarrow{QP}\|.
$$

Thus the orthogonal projection point $Q$ uniquely minimizes the distance from $P$ to the line.
