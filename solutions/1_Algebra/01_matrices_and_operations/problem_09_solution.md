### Exercise 9. Solution

**Important:** in $RSx$ the vector $x$ is acted on first by $S$, and then by $R$. The matrix closest to $x$ acts first.

**1. Compute $RSx$ (first scale, then rotate)**

$$
Sx=\begin{pmatrix} 2 & 0 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 1 \cr 2 \end{pmatrix}=\begin{pmatrix} 2 \cr 2 \end{pmatrix}
$$

$$
R(Sx)=\begin{pmatrix} 0 & -1 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} 2 \cr 2 \end{pmatrix}=\begin{pmatrix} 0\cdot2+(-1)\cdot2 \cr 1\cdot2+0\cdot2 \end{pmatrix}=\begin{pmatrix} -2 \cr 2 \end{pmatrix}
$$

**2. Compute $SRx$ (first rotate, then scale)**

$$
Rx=\begin{pmatrix} 0 & -1 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} 1 \cr 2 \end{pmatrix}=\begin{pmatrix} -2 \cr 1 \end{pmatrix}
$$

$$
S(Rx)=\begin{pmatrix} 2 & 0 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} -2 \cr 1 \end{pmatrix}=\begin{pmatrix} -4 \cr 1 \end{pmatrix}
$$

**3. Check via the product matrices**

$$
RS=\begin{pmatrix} 0 & -1 \cr 2 & 0 \end{pmatrix},\qquad SR=\begin{pmatrix} 0 & -2 \cr 1 & 0 \end{pmatrix}
$$

$$
RSx=\begin{pmatrix} 0 & -1 \cr 2 & 0 \end{pmatrix}\begin{pmatrix} 1 \cr 2 \end{pmatrix}=\begin{pmatrix} -2 \cr 2 \end{pmatrix},\qquad SRx=\begin{pmatrix} 0 & -2 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} 1 \cr 2 \end{pmatrix}=\begin{pmatrix} -4 \cr 1 \end{pmatrix}
$$

**4. Comparison**

$$
RSx=\begin{pmatrix} -2 \cr 2 \end{pmatrix}\neq\begin{pmatrix} -4 \cr 1 \end{pmatrix}=SRx
$$

The results are different, so $RS\neq SR$. The lengths differ too: $|RSx|=\sqrt{8}$, while $|SRx|=\sqrt{17}$.

**5. Geometric explanation**

The scaling $S$ stretches the plane only in the horizontal direction (the $x$-axis) by a factor of $2$ and leaves the vertical direction unchanged. The rotation $R$ turns every vector by $90^\circ$ counterclockwise, so it changes which direction is "horizontal".

- $RSx$: first we stretch the original vector horizontally, $(1,2)\to(2,2)$, and then rotate it. The stretched part (horizontal) becomes vertical after the rotation, so the result is $(-2,2)$.
- $SRx$: first we rotate, $(1,2)\to(-2,1)$, and then stretch. Now the horizontal part of the rotated vector is the one that gets doubled, so the result is $(-4,1)$.

The same stretch is applied to different parts of the vector, because the rotation in between changes the directions. This is why the order of transformations matters, and why matrix multiplication is not commutative.

**Answers:**

$$
RSx=\begin{pmatrix} -2 \cr 2 \end{pmatrix},\qquad SRx=\begin{pmatrix} -4 \cr 1 \end{pmatrix},\qquad RSx\neq SRx
$$
