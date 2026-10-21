# Exercise 14. Rotation Matrices

## Question

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

## Solution

### Steps

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & -\sin\alpha\sin\beta+\cos\alpha\cos\beta \\
\end{pmatrix}
$$

The angle-sum formulas are

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
$$

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

Entries $(1,1)$ and $(2,2)$ equal $\cos(\alpha+\beta)$. Entry $(2,1)$ equals $\sin(\alpha+\beta)$. Entry $(1,2)$ equals $-(\cos\alpha\sin\beta+\sin\alpha\cos\beta)=-\sin(\alpha+\beta)$.

### Result

$$
\begin{aligned}
R(\alpha)R(\beta) &=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix} \\
&= R(\alpha+\beta).
\end{aligned}
$$

### Method

Geometrically, $R(\beta)$ rotates a vector by the angle $\beta$ and $R(\alpha)$ then rotates the result by $\alpha$. The total effect is a rotation by $\alpha+\beta$, which is the transformation given by $R(\alpha+\beta)$. Matrix multiplication is composition of transformations, and the angle-sum formulas are exactly what makes the algebra agree with this geometry. Since $\alpha+\beta=\beta+\alpha$, rotations in the plane commute: $R(\alpha)R(\beta)=R(\beta)R(\alpha)$.

### Verification

For $\alpha=\beta=90^\circ$:

$$
\begin{aligned}
R(90^\circ)R(90^\circ) &=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 & 0 \\
0 & -1 \\
\end{pmatrix} \\
&= R(180^\circ).
\end{aligned}
$$
