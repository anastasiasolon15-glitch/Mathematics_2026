### Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\left(\begin{array}{ccc|c}
1 & 2 & -1 & 3 \\
0 & 1 & 2 & 1 \\
0 & 0 & 0 & 0
\end{array}\right)
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

The matrix is already in row echelon form. It has two nonzero rows, so there are two pivots (in columns 1 and 2), and the third row $0=0$ is harmless, so the system is consistent. The equations are

$$
x+2y-z=3,\qquad y+2z=1.
$$

There are $3$ unknowns and $2$ pivots, so $3-2=1$ variable is free. The column of $z$ has no pivot, so put $z=t$. Then

$$
y=1-2t,\qquad x=3-2y+z=3-2(1-2t)+t=1+5t.
$$

Hence the system has infinitely many solutions:

$$
(x,y,z)=(1+5t,\;1-2t,\;t),\qquad t\in\mathbb{R}.
$$

**Verification.** For $t=0$ we get $(1,1,0)$: $1+2-0=3$ and $1+0=1$. Both equations hold.

**Rule.** For a consistent system, the number of free variables equals the number of unknowns minus the number of pivots.
