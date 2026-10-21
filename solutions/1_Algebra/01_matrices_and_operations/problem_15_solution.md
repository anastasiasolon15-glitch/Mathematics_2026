# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

### Steps

Path 1, $(AB)C$:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
(AB)C &=
\begin{pmatrix}
5\cdot2+2\cdot0 & 5\cdot1+2\cdot(-1) \\
1\cdot2+4\cdot0 & 1\cdot1+4\cdot(-1) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
\end{aligned}
$$

Path 2, $A(BC)$:

$$
\begin{aligned}
BC &=
\begin{pmatrix}
1\cdot2+0\cdot0 & 1\cdot1+0\cdot(-1) \\
2\cdot2+1\cdot0 & 2\cdot1+1\cdot(-1) \\
-1\cdot2+3\cdot0 & -1\cdot1+3\cdot(-1) \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
A(BC) &=
\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
\begin{aligned}
(AB)C &= A(BC) \\
&=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
\end{aligned}
$$

### Method

Counting scalar multiplications (a product of sizes $m\times n$ and $n\times q$ needs $m\cdot n\cdot q$ of them):

- $AB$: $2\cdot3\cdot2=12$, then $(AB)C$: $2\cdot2\cdot2=8$, in total $20$.
- $BC$: $3\cdot2\cdot2=12$, then $A(BC)$: $2\cdot3\cdot2=12$, in total $24$.

Associativity means that the final matrix does not depend on how the factors are grouped, so the product $ABC$ is well defined without parentheses. The amount of work can still differ: here the first path is cheaper (20 against 24 multiplications), although the result is the same.

### Verification

The two paths give identical matrices entry by entry. The sizes also agree: $(2\times3)(3\times2)(2\times2)$ gives $2\times2$ in both groupings.
