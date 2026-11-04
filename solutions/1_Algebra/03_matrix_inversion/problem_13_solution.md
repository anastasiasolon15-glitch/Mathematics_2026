# Exercise 13. Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## Solution

### Steps

Way 1. The product is

$$
T=HS=
\begin{pmatrix}
1\cdot2+1\cdot0 & 1\cdot0+1\cdot1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad \det T=2.
$$

By the $2\times2$ formula:

$$
T^{-1}=\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

Way 2. The individual inverses are

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

Then

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

The incorrect order:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1\cdot\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

### Result

$$
T^{-1}=S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix},
$$

while $H^{-1}S^{-1}$ is a different matrix, which differs in position $(1,2)$.

### Method

The transformation $T=HS$ first applies the scaling $S$ and then the shear $H$. To undo it, the last operation must be undone first: apply $H^{-1}$ and then $S^{-1}$. In matrix notation, the operation applied first is written on the right, so $T^{-1}=S^{-1}H^{-1}$. This is like taking off socks and shoes: shoes were put on last, so they come off first.

### Verification

$$
\begin{aligned}
TT^{-1} &=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & -1+1 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$
