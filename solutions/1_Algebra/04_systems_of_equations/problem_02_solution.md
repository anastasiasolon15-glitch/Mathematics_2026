### Exercise 2. Gaussian Elimination — One Solution

## Question

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

## Solution

Gaussian elimination uses row operations (which do not change the solution set) to bring the augmented matrix to row echelon form, and then back substitution finds the unknowns.

Step 1: apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$.

$$
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}\right).
$$

Step 2: interchange $R_2$ and $R_3$.

$$
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & -3 & -1 & -9
\end{array}\right).
$$

Step 3: apply $R_3\leftarrow R_3+3R_2$.

$$
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & -3 & -1 & -9
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & -7 & -21
\end{array}\right).
$$

Back substitution:

$$
-7z=-21\Rightarrow z=3,\qquad
y-2z=-4\Rightarrow y=2,\qquad
x+y+z=6\Rightarrow x=1.
$$

**Verification.** Substituting $(x,y,z)=(1,2,3)$:

$$
1+2+3=6,\qquad 2-2+3=3,\qquad 1+4-3=2.
$$

All three equations hold, so the unique solution is $(1,2,3)$.
