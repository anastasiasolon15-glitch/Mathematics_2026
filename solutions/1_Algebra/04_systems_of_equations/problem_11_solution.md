### Exercise 11. A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

Apply $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
1 & t & 1 & 2 \\
1 & 1 & t & 3
\end{array}\right)
\to
\left(\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
0 & t-1 & 0 & 1 \\
0 & 0 & t-1 & 2
\end{array}\right).
$$

The resulting equations are $(t-1)y=1$ and $(t-1)z=2$. The standard step is division by $t-1$, which is valid only for $t\neq1$.

**Case $t\neq1$.** Then

$$
y=\frac{1}{t-1},\qquad z=\frac{2}{t-1},\qquad x=1-y-z=\frac{t-4}{t-1}.
$$

**Exactly one solution.** Check for $t=2$: $(x,y,z)=(-2,1,2)$ gives $-2+1+2=1$, $-2+2+2=2$, $-2+1+4=3$.

**Case $t=1$.** The second row becomes $0=1$, a contradiction. **No solution.**

**Conclusion.** For $t\ne1$ the solution is unique; for $t=1$ there is none. Infinitely many solutions never occur.
