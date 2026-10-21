# Exercise 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

## Solution

### Steps

Row by row (dot products):

$$
\begin{aligned}
Ax &=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
\end{aligned}
$$

Column by column, with the entries of $x$ as coefficients:

$$
\begin{aligned}
Ax &= 4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix} + 2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix} +
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
\end{aligned}
$$

### Result

$$
Ax=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
\quad\mathrm{with}\quad
Ax=4a_1+2a_2,
$$

where $a_1,a_2$ are the columns of $A$.

### Method

For a matrix with columns $a_1,\dots,a_n$ and a vector $x=(x_1,\dots,x_n)$ the product satisfies $Ax=x_1a_1+\dots+x_na_n$. Hence $Ax$ always lies in the set of linear combinations of the columns of $A$.

### Verification

Both methods, the row dot products and the combination of columns, give the same vector $(6,10)$.
```[cite: 1]
