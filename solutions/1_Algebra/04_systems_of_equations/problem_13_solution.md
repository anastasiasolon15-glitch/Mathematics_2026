### Exercise 13. Does Every Equation Add New Information?

## Question

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## Solution

Step 1: apply $R_3\leftarrow R_3-R_1$.

$$
\left(\begin{array}{ccc|c}
1 & 1 & 0 & 10 \\
0 & 1 & 1 & 8 \\
1 & 0 & -1 & 2
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 0 & 10 \\
0 & 1 & 1 & 8 \\
0 & -1 & -1 & -8
\end{array}\right).
$$

Step 2: apply $R_3\leftarrow R_3+R_2$.

$$
\left(\begin{array}{ccc|c}
1 & 1 & 0 & 10 \\
0 & 1 & 1 & 8 \\
0 & -1 & -1 & -8
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 0 & 10 \\
0 & 1 & 1 & 8 \\
0 & 0 & 0 & 0
\end{array}\right).
$$

The system is consistent with two pivots and three unknowns, so $x_3=t$ is free:

$$
x_2=8-t,\qquad x_1=10-x_2=2+t,\qquad (x_1,x_2,x_3)=(2+t,\;8-t,\;t).
$$

**Verification.** For $t=0$ we get $(2,8,0)$: $2+8=10$, $8+0=8$, $2-0=2$.

**Redundancy.** The zero row shows that one equation carries no new information. Indeed, subtracting the second equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8\ \Rightarrow\ x_1-x_3=2,
$$

which is exactly the third equation. So the third equation follows from the first two and can be dropped without changing the solution set (a line in space).
