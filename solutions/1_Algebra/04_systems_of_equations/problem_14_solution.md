### Exercise 14. A Small Change in the Right-Hand Side

## Question

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
\qquad\text{and}\qquad
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

Both systems can be treated at once: let the last right-hand side be $c$ ($c=3$ for the first system, $c=3.1$ for the second).

Step 1: apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-3R_1$.

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
2 & -1 & 1 \\
3 & 0 & c
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -3 & -3 \\
0 & -3 & c-6
\end{array}\right).
$$

Step 2: apply $R_3\leftarrow R_3-R_2$.

$$
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -3 & -3 \\
0 & -3 & c-6
\end{array}\right)
\to
\left(\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -3 & -3 \\
0 & 0 & c-3
\end{array}\right).
$$

**First system ($c=3$).** The last row is $0=0$, so the system is consistent. Then $y=1$, $x=1$: the unique solution is $(1,1)$. Check: $1+1=2$, $2-1=1$, $3\cdot1=3$.

**Second system ($c=3.1$).** The last row is $0=0.1$, a contradiction, so the system is **inconsistent**. Check: the first two equations force $(1,1)$, but $3\cdot1=3\neq3.1$.

**Explanation.** There are three equations for only two unknowns, so the system is overdetermined. Geometrically, three lines must pass through one common point. For $c=3$ the third line $x=1$ passes exactly through the intersection point $(1,1)$ of the first two. For $c=3.1$ it is shifted slightly, so no point lies on all three lines. Consistency of such a system requires an exact compatibility condition, which a tiny change can destroy.
