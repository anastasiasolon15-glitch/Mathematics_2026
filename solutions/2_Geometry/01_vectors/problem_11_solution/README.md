# Exercise 11. Decomposition into Parallel and Perpendicular Components

## Question

Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check

$$
u=u_{\parallel}+u_{\perp},\qquad u_{\perp}\cdot v=0.
$$

Explain why these are two independent checks of correctness.

> **Why this exercise:** deepens the idea of projection through construction and verification.

## Solution

### Steps

Compute the parallel component $u_{\parallel} = \mathrm{proj}_v\,u$:

$$
u\cdot v = 3\cdot1 + 4\cdot2 = 11,
$$

$$
v\cdot v = 1^2 + 2^2 = 5.
$$

Then:

$$
u_{\parallel} = \frac{11}{5}(1, 2) = \left(\frac{11}{5}, \frac{22}{5}\right).
$$

Compute the perpendicular component $u_{\perp}$:

$$
u_{\perp} = u - u_{\parallel} = (3, 4) - \left(\frac{11}{5}, \frac{22}{5}\right) = \left(\frac{4}{5}, -\frac{2}{5}\right).
$$

### Verification

Check 1 (reconstruction):

$$
u_{\parallel} + u_{\perp} = \left(\frac{11}{5}, \frac{22}{5}\right) + \left(\frac{4}{5}, -\frac{2}{5}\right) = \left(\frac{15}{5}, \frac{20}{5}\right) = (3, 4) = u.
$$

Check 2 (orthogonality):

$$
u_{\perp}\cdot v = \frac{4}{5}\cdot1 + \left(-\frac{2}{5}\right)\cdot2 = \frac{4}{5} - \frac{4}{5} = 0.
$$

### Result

$$
u_{\parallel} = \left(\frac{11}{5}, \frac{22}{5}\right),\qquad u_{\perp} = \left(\frac{4}{5}, -\frac{2}{5}\right).
$$

### Explanation

The two checks are independent because they test distinct requirements:
1. Reconstruction $u_{\parallel}+u_{\perp}=u$ confirms that the full vector $u$ is conserved.
2. Orthogonality $u_{\perp}\cdot v=0$ confirms that $u_{\perp}$ is perpendicular to $v$.

Neither check implies the other. An incorrect parallel component combined with $u-u_{\parallel}$ satisfies reconstruction automatically but fails orthogonality. Conversely, an arbitrary vector orthogonal to $v$ fails reconstruction. Both conditions must hold simultaneously to ensure a correct orthogonal decomposition.
