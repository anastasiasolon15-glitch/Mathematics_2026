### Exercise 14. Solution

**Angle-sum formulas** (we use them below):

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,\qquad \sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

**1. Compute $R(\alpha)R(\beta)$**

$$
R(\alpha)R(\beta)=\begin{pmatrix} \cos\alpha & -\sin\alpha \cr \sin\alpha & \cos\alpha \end{pmatrix}\begin{pmatrix} \cos\beta & -\sin\beta \cr \sin\beta & \cos\beta \end{pmatrix}
$$

Entry by entry (row by column):

- top-left: $\cos\alpha\cos\beta-\sin\alpha\sin\beta$
- top-right: $-\cos\alpha\sin\beta-\sin\alpha\cos\beta$
- bottom-left: $\sin\alpha\cos\beta+\cos\alpha\sin\beta$
- bottom-right: $-\sin\alpha\sin\beta+\cos\alpha\cos\beta$

$$
R(\alpha)R(\beta)=\begin{pmatrix} \cos\alpha\cos\beta-\sin\alpha\sin\beta & -(\sin\alpha\cos\beta+\cos\alpha\sin\beta) \cr \sin\alpha\cos\beta+\cos\alpha\sin\beta & \cos\alpha\cos\beta-\sin\alpha\sin\beta \end{pmatrix}
$$

**2. Apply the angle-sum formulas**

The expression $\cos\alpha\cos\beta-\sin\alpha\sin\beta$ equals $\cos(\alpha+\beta)$, and the expression $\sin\alpha\cos\beta+\cos\alpha\sin\beta$ equals $\sin(\alpha+\beta)$. Therefore

$$
R(\alpha)R(\beta)=\begin{pmatrix} \cos(\alpha+\beta) & -\sin(\alpha+\beta) \cr \sin(\alpha+\beta) & \cos(\alpha+\beta) \end{pmatrix}=R(\alpha+\beta)
$$

**3. Geometric explanation**

The matrix $R(\theta)$ rotates every vector in the plane by the angle $\theta$ counterclockwise about the origin. The product $R(\alpha)R(\beta)$ means: first rotate by $\beta$, then rotate by $\alpha$. Two rotations about the same point one after another give a single rotation by the total angle $\alpha+\beta$. The calculation above confirms that matrix multiplication describes exactly this: multiplying the matrices corresponds to adding the angles.

**4. Consequences**

Since $\alpha+\beta=\beta+\alpha$, we also get $R(\beta)R(\alpha)=R(\alpha+\beta)$. So, unlike general matrices, **rotations in the plane commute**: $R(\alpha)R(\beta)=R(\beta)R(\alpha)$. (This is different from Exercise 9, where a rotation and a nonuniform scaling did not commute.)

Also $R(\theta)R(-\theta)=R(0)=I$, so $R(-\theta)$ is the inverse of $R(\theta)$.

**Check.** Take $\alpha=\beta=90^\circ$. Then $R(90^\circ)=\begin{pmatrix} 0 & -1 \cr 1 & 0 \end{pmatrix}$ and

$$
R(90^\circ)R(90^\circ)=\begin{pmatrix} 0 & -1 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} 0 & -1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} -1 & 0 \cr 0 & -1 \end{pmatrix}=R(180^\circ)
$$

Two quarter-turns give a half-turn, as expected.

**Answer:**

$$
R(\alpha)R(\beta)=\begin{pmatrix} \cos(\alpha+\beta) & -\sin(\alpha+\beta) \cr \sin(\alpha+\beta) & \cos(\alpha+\beta) \end{pmatrix}=R(\alpha+\beta)
$$
