### Exercise 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2
\end{pmatrix}.
$$

1. Compute $Ax$.
2. Express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the entries of the vector $x$.

## Solution

**Step 1: computing $Ax$.** The matrix $A$ has size $2\times 2$ and $x$ has size $2\times 1$, so the product is defined and is a $2\times 1$ vector. Each entry of $Ax$ is the dot product of a row of $A$ with $x$:

$$
Ax=
\begin{pmatrix}
2\cdot 4+(-1)\cdot 2 \\
1\cdot 4+3\cdot 2
\end{pmatrix}=
\begin{pmatrix}
8-2 \\
4+6
\end{pmatrix}=
\begin{pmatrix}
6 \\
10
\end{pmatrix}.
$$

**Step 2: linear combination of columns.** Denote the columns of $A$ by

$$
a_1=
\begin{pmatrix}
2 \\
1
\end{pmatrix},\qquad a_2=
\begin{pmatrix}
-1 \\
3
\end{pmatrix}.
$$

For $x=(x_1,x_2)^T$ we have $Ax=x_1a_1+x_2a_2$: the first entry of $x$ multiplies the first column, and the second entry multiplies the second column. Here $x_1=4$ and $x_2=2$, so

$$
Ax=4
\begin{pmatrix}
2 \\
1
\end{pmatrix}+
2
\begin{pmatrix}
-1 \\
3
\end{pmatrix}=
\begin{pmatrix}
8 \\
4
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6
\end{pmatrix}=
\begin{pmatrix}
6 \\
10
\end{pmatrix}.
$$

**Verification.** Both methods give the same vector $(6,10)^T$. The row-wise computation and the column-wise computation are two views of the same operation, which is why the results agree.

**Conclusion.** Multiplying a matrix by a vector produces a linear combination of the columns of the matrix, with the entries of the vector as coefficients. Here, $Ax=4a_1+2a_2=(6,10)^T$.
