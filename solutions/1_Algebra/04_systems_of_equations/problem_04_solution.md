### Exercise 4. Infinitely Many Solutions

## Question

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
2 & 2 & 2 & 4 \\
1 & -1 & 1 & 0
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 2 \\
0 & 0 & 0 & 0 \\
0 & -2 & 0 & -2
\end{array}\right).
$$

The zero row means the second equation was redundant (twice the first). The remaining equations are

$$
-2y=-2\Rightarrow y=1,\qquad x+y+z=2\Rightarrow x+z=1.
$$

The columns of $x$ and $y$ contain pivots, the column of $z$ does not, so $z$ is a **free variable**. Put $z=t$:

$$
(x,y,z)=(1-t,\;1,\;t),\qquad t\in\mathbb{R}.
$$

The system is consistent and has a free variable, so it has infinitely many solutions.

**Verification.** For $t=2$ we get $(-1,1,2)$:

$$
-1+1+2=2,\qquad -2+2+4=4,\qquad -1-1+2=0.
$$

All three equations hold.
