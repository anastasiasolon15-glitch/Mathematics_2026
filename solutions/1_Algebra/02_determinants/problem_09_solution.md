# Exercise 9. Area and the Determinant

## Question

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},\qquad v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

### Steps

Put the vectors $u,v$ as columns of a matrix and compute its determinant:

$$
\begin{aligned}
\det
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
&= 3\cdot4-1\cdot1 \\
&= 11.
\end{aligned}
$$

The area is the absolute value of the determinant, so the area equals $11$.

Reversing the order of the vectors swaps the columns:

$$
\begin{aligned}
\det
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
&= 1\cdot1-3\cdot4 \\
&= -11.
\end{aligned}
$$

### Result

$$
\det(u,v)=11,\qquad \det(v,u)=-11,\qquad \mathrm{Area}=11.
$$

### Method

The absolute value $|\det(u,v)|$ is the area of the parallelogram spanned by $u$ and $v$. The sign of the determinant records the orientation of the pair of vectors. Swapping the vectors reverses the orientation, so the determinant changes sign, while the parallelogram itself is the same figure, so its area is unchanged.

### Verification

Independent calculation with base and height. The length of the base is $|u|=\sqrt{10}$. A unit vector perpendicular to $u$ is $n=\dfrac{1}{\sqrt{10}}(-1,\ 3)$, and the height is the length of the projection of $v$ onto $n$:

$$
h=|v\cdot n|=\frac{|-1+12|}{\sqrt{10}}=\frac{11}{\sqrt{10}}.
$$

Then

$$
\mathrm{Area}=|u|\cdot h=\sqrt{10}\cdot\frac{11}{\sqrt{10}}=11,
$$

which agrees with the determinant.
