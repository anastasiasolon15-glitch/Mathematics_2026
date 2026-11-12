### Exercise 9. A System from a Sum Condition

## Question

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

## Solution

Apply $R_2\leftarrow R_2-2R_1$:

$$
\left(\begin{array}{cc|c}
1 & 1 & 10 \\
2 & 5 & 32
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 10 \\
0 & 3 & 12
\end{array}\right).
$$

Back substitution: $3y=12\Rightarrow y=4$, and $x=10-y=6$.

**Verification.** $6+4=10$ and $2\cdot6+5\cdot4=12+20=32$. Both conditions hold.

**Geometric explanation.** Each equation describes a line in the plane. Their slopes are $-1$ and $-\tfrac25$, which are different, so the lines are not parallel and intersect in exactly one point, $(6,4)$. Algebraically, elimination gives two pivots for two unknowns, so there are no free variables.
