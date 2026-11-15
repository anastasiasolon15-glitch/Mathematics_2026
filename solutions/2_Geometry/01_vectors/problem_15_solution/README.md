# Exercise 15. Comparing Directions Using the Cosine of the Angle

## Question

Given

$$
a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3).
$$

For each pair, compute

$$
\frac{u\cdot v}{\|u\|\,\|v\|}.
$$

Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

> **Why this exercise:** reinforces the connection between the dot product and angle, and the distinction between direction and length.

## Solution

### Steps

Compute the norms of the vectors:

$$
\|a\| = \sqrt{1^2 + 2^2 + 1^2} = \sqrt{6},
$$

$$
\|b\| = \sqrt{2^2 + 4^2 + 2^2} = \sqrt{24} = 2\sqrt{6},
$$

$$
\|c\| = \sqrt{2^2 + 0^2 + 3^2} = \sqrt{13}.
$$

Compute the direction cosine for each pair:

Pair $(a, b)$:

$$
a\cdot b = 1\cdot2 + 2\cdot4 + 1\cdot2 = 12,
$$

$$
\frac{a\cdot b}{\|a\|\,\|b\|} = \frac{12}{\sqrt{6}\sqrt{24}} = \frac{12}{12} = 1.
$$

The angle is $\theta_{ab} = \arccos(1) = 0$.

Pair $(a, c)$:

$$
a\cdot c = 1\cdot2 + 2\cdot0 + 1\cdot3 = 5,
$$

$$
\frac{a\cdot c}{\|a\|\,\|c\|} = \frac{5}{\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}}.
$$

The angle is $\theta_{ac} = \arccos(5/\sqrt{78})$.

Pair $(b, c)$:

$$
b\cdot c = 2\cdot2 + 4\cdot0 + 2\cdot3 = 10,
$$

$$
\frac{b\cdot c}{\|b\|\,\|c\|} = \frac{10}{\sqrt{24}\sqrt{13}} = \frac{10}{2\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}}.
$$

The angle is $\theta_{bc} = \arccos(5/\sqrt{78})$.

### Ordering

On $[0, \pi]$, the function $\arccos(x)$ is strictly decreasing, so a larger cosine corresponds to a smaller angle:

$$
\cos\theta_{ab} = 1 > \cos\theta_{ac} = \cos\theta_{bc} = \frac{5}{\sqrt{78}}.
$$

The pairs in order of increasing angle:
1. $(a, b)$ with angle $\theta = 0$.
2. $(a, c)$ and $(b, c)$ tied with angle $\theta = \arccos(5/\sqrt{78})$.

### Result

$$
\frac{a\cdot b}{\|a\|\,\|b\|} = 1,\qquad \frac{a\cdot c}{\|a\|\,\|c\|} = \frac{5}{\sqrt{78}},\qquad \frac{b\cdot c}{\|b\|\,\|c\|} = \frac{5}{\sqrt{78}}.
$$

### Explanation

For the pair $(a, b)$, notice that $b=2a$. When one vector is a positive scalar multiple of another ($b=ka$ with $k=2>0$):

$$
\frac{a\cdot(ka)}{\|a\|\,\|ka\|} = \frac{k(a\cdot a)}{k\|a\|^2} = \frac{\|a\|^2}{\|a\|^2} = 1.
$$

The scalar $k$ cancels completely. The cosine measures relative direction, which is independent of length. Because $a$ and $b$ point in the same direction, the angle between them is $0$, and $\cos(0)=1$.
