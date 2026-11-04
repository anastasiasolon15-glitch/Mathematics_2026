# Exercise 11. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## Solution

### Steps

The determinant is

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2=(1-t)(1+t).
$$

It vanishes exactly for $t=1$ and $t=-1$. Hence $A(t)$ is invertible if and only if $t\neq1$ and $t\neq-1$.

For such $t$ the $2\times2$ formula gives

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}.
$$

### Result

The matrix is invertible for all $t\neq\pm1$, and the inverse is the formula above.

### Method

At $t=1$ and $t=-1$ the factor $\frac{1}{1-t^2}$ is not defined, since the denominator is zero. This is not a flaw of the formula. At these values the matrix really has no inverse: for $t=1$ the two rows are equal, and for $t=-1$ the rows are $(1,-1)$ and $(-1,1)$, so one is the negative of the other. In both cases the rows are dependent.

### Verification

$$
\begin{aligned}
A(t)\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix} &=
\begin{pmatrix}
1-t^2 & -t+t \\
t-t & -t^2+1 \\
\end{pmatrix} \\
&=(1-t^2)I.
\end{aligned}
$$

Dividing by $1-t^2\neq0$ gives $A(t)A(t)^{-1}=I$.
