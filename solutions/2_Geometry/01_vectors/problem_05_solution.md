# Exercise 5. Angle Between Vectors

## Question

Given $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

> **Why this exercise:** teaches how to extract qualitative information first and only then perform the exact calculation.

## Solution

### Steps

Compute the scalar product $u\cdot v$:

$$
u\cdot v = 1\cdot1 + 1\cdot0 + 0\cdot1 = 1.
$$

Since the norms $\|u\|$ and $\|v\|$ are strictly positive, the sign of $\cos\theta = \frac{u\cdot v}{\|u\|\,\|v\|}$ is determined by the sign of $u\cdot v$. Because $u\cdot v = 1 > 0$, the angle $\theta\in[0,\pi]$ is predicted to be acute ($0 \le \theta < \pi/2$).

Compute the norms of $u$ and $v$:

$$
\|u\| = \sqrt{1^2 + 1^2 + 0^2} = \sqrt{2},
$$

$$
\|v\| = \sqrt{1^2 + 0^2 + 1^2} = \sqrt{2}.
$$

Compute the cosine of the angle:

$$
\cos\theta = \frac{u\cdot v}{\|u\|\,\|v\|} = \frac{1}{\sqrt{2}\sqrt{2}} = \frac{1}{2}.
$$

Determine the angle:

$$
\theta = \arccos\left(\frac{1}{2}\right) = \frac{\pi}{3}.
$$

### Result

The angle is $\theta = \pi/3$ ($60^\circ$).

### Explanation

The exact value $\theta = \pi/3$ lies in the interval $(0, \pi/2)$, which confirms the qualitative prediction that the angle is acute.
