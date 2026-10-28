# Exercise 3. Swapping Two Rows

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

## Solution

### Steps

Expansion of $\det A$ along the first row:

$$
\begin{aligned}
\det A &= 1\cdot(3\cdot1-1\cdot1)-2\cdot(0\cdot1-1\cdot2)+0 \\
&= 1\cdot2-2\cdot(-2) \\
&= 2+4 \\
&= 6.
\end{aligned}
$$

The matrix after swapping the first and second rows is

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$

Prediction: swapping two rows changes the sign of the determinant, so $\det B=-\det A=-6$.

Calculation of $\det B$ along the first row:

$$
\begin{aligned}
\det B &= 0-3\cdot(1\cdot1-0\cdot2)+1\cdot(1\cdot1-2\cdot2) \\
&= -3\cdot1+1\cdot(-3) \\
&= -6.
\end{aligned}
$$

### Result

$$
\det A=6,\qquad \det B=-6.
$$

### Method

The property used: interchanging two rows of a matrix multiplies the determinant by $-1$. The prediction made from this property agrees with the direct calculation.

### Verification

Sarrus' rule for $A$: the main diagonals give $1\cdot3\cdot1+2\cdot1\cdot2+0\cdot0\cdot1=7$, and the anti diagonals give $0\cdot3\cdot2+1\cdot1\cdot1+2\cdot0\cdot1=1$. Hence $\det A=7-1=6$, which confirms the first expansion.
