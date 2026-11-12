### Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary.

## Solution

**Case 1: triangular system, back substitution.** The matrix is already triangular (the second equation contains only $y$), so no elimination is needed:

$$
4y=8\Rightarrow y=2,\qquad 2x-2=3\Rightarrow x=\tfrac52.
$$

Check: $2\cdot\tfrac52-2=3$ and $4\cdot 2=8$. The solution is $(\tfrac52,\,2)$.

**Case 2: three right-hand sides, $A^{-1}$ known.** Use $x_i=A^{-1}b_i$ for $i=1,2,3$. The expensive part (finding $A^{-1}$, or an elimination of $A$) is already done and is reused for all three systems. Only three matrix–vector products remain. No new elimination is needed.

**Case 3: one right-hand side, no inverse given.** Use Gaussian elimination on the augmented matrix $(A\mid b)$ followed by back substitution. Computing $A^{-1}$ would be unnecessary work: finding the inverse costs about as much as solving three systems at once, but only one solution vector is needed.

**Conclusion.** The choice depends on the structure of the matrix (triangular, already factored or inverted) and on the number of right-hand sides (one versus many), not on the name of the method.
