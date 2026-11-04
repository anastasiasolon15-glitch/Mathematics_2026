# Exercise 8. Inverse of a Transformation

## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## Solution

### Steps

For a diagonal matrix with nonzero diagonal entries the inverse is diagonal with reciprocal entries:

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

Action on the vector $v=(1,1)$:

$$
Sv=
\begin{pmatrix}
2 \\
\frac12 \\
\end{pmatrix},\qquad
S^{-1}(Sv)=
\begin{pmatrix}
\frac12\cdot2 \\
2\cdot\frac12 \\
\end{pmatrix}=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}.
$$

### Result

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

### Method

The transformation $S$ stretches the plane by a factor $2$ in the $x$ direction and compresses it by a factor $\frac12$ in the $y$ direction. The inverse transformation does the opposite: it compresses by a factor $\frac12$ in the $x$ direction and stretches by a factor $2$ in the $y$ direction. Each direction is scaled by the reciprocal factor, so every vector returns to its original position.

### Verification

Both products give the identity:

$$
SS^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 \\
0 & \frac12\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}=S^{-1}S.
$$

Also $\det S=2\cdot\frac12=1$, so $S$ preserves areas, and $S^{-1}$ preserves them too.
