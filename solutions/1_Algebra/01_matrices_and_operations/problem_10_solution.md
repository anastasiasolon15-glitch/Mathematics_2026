# Exercise 10. Columns of a Matrix Product

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

## Solution

### Steps

The columns of $B$ are

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},\qquad
b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

Matrix-vector products:

$$
\begin{aligned}
Ab_1 &=
\begin{pmatrix}
1\cdot1+2\cdot(-1)+0\cdot3 \\
0\cdot1+1\cdot(-1)+1\cdot3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
\end{aligned}
$$

$$
\begin{aligned}
Ab_2 &=
\begin{pmatrix}
1\cdot2+2\cdot0+0\cdot1 \\
0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
\end{aligned}
$$

Full product, with rows of $A$ times columns of $B$:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
1-2+0 & 2+0+0 \\
0-1+3 & 0+0+1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix},
$$

and its columns are $Ab_1=(-1,2)$ and $Ab_2=(2,1)$.

### Method

Entry $(i,j)$ of $AB$ is the dot product of row $i$ of $A$ with column $j$ of $B$. Collecting these entries for fixed $j$ over all $i$ gives exactly the vector $Ab_j$, the dot products of all rows of $A$ with the single vector $b_j$. Therefore column $j$ of $AB$ equals $Ab_j$. In other words, the matrix $A$ is applied to each column of $B$ separately.

### Verification

The first column of $AB$ is $(-1,2)$ and equals $Ab_1$. The second column is $(2,1)$ and equals $Ab_2$. Both ways of computing agree.
