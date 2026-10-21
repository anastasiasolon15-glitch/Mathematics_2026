# Exercise 9. Composing Transformations

## Question

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

### Steps

In $RSx=R(Sx)$ the matrix $S$ acts first. In $SRx=S(Rx)$ the matrix $R$ acts first.

$$
\begin{aligned}
Sx &=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix} \\
RSx &= R
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
Rx &=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix} \\
SRx &= S
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
RSx=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},\qquad
SRx=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix},\qquad
RSx\neq SRx.
$$

### Method

Geometrically, $S$ stretches the plane by a factor of 2 along the $x$-axis only. In $RSx$ the stretch is applied first, along the original horizontal direction, and the rotation then turns the stretched picture by $90^\circ$. In $SRx$ the rotation is applied first, and the stretch then acts along the horizontal direction of the rotated picture. Since the stretching direction is fixed in the plane while the rotation moves the vector relative to it, different parts of the vector get stretched, and the final vectors differ. Equivalently, the products of the matrices differ:

$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0 \\
\end{pmatrix},\qquad
SR=
\begin{pmatrix}
0 & -2 \\
1 & 0 \\
\end{pmatrix}.
$$

### Verification

Applying the product matrices directly to $x$:

$$
\begin{aligned}
RSx &=
\begin{pmatrix}
0\cdot1-1\cdot2 \\
2\cdot1+0\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
SRx &=
\begin{pmatrix}
0\cdot1-2\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
\end{aligned}
$$

This agrees with the step-by-step computation.
