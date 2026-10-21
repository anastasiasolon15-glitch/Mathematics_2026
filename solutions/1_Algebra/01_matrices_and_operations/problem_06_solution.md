# Exercise 6. Transpose

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

## Solution

### Steps

The transpose swaps rows and columns: $(A^T)_{ij} = a_{ji}$.

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix},\qquad
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

The product $AB$ has size $2\times2$:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
\end{aligned}
$$

Left side of the identity:

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Right side of the identity:

$$
\begin{aligned}
B^TA^T &=
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$(AB)^T=B^TA^T$ holds in this example, with both sides equal to

$$
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

### Method

The identity $(AB)^T=B^TA^T$ reverses the order of factors. The entry $(i,j)$ of $(AB)^T$ is the dot product of row $j$ of $A$ with column $i$ of $B$. This equals the dot product of row $i$ of $B^T$ with column $j$ of $A^T$, which is the entry $(i,j)$ of $B^TA^T$.

### Verification

The sizes are consistent: $B^T$ is $2\times3$ and $A^T$ is $3\times2$, so $B^TA^T$ is $2\times2$, the size of $(AB)^T$. The other order $A^TB^T$ is also defined, but it has size $3\times3$, which differs from the size of $(AB)^T$, so only the reversed order can match.
