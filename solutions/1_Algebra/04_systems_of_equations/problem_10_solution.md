### Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

Each point gives one linear equation in the unknown coefficients $a,b,c$:

$$
\begin{cases}
p(0)=c=1, \\
p(1)=a+b+c=3, \\
p(2)=4a+2b+c=9.
\end{cases}
$$

From the first equation $c=1$. Substituting into the other two:

$$
\begin{cases}
a+b=2, \\
4a+2b=8.
\end{cases}
$$

Eliminate: $R_2\leftarrow R_2-4R_1$ gives $-2b=0$, so $b=0$, and then $a=2$.

$$
p(x)=2x^2+1.
$$

**Verification.**

$$
p(0)=1,\qquad p(1)=2+1=3,\qquad p(2)=8+1=9.
$$

All three points lie on the graph. Since the system has a unique solution, this is the only such polynomial of degree at most $2$.
