# Matrices and Basic Operations — Exercise 1. Matrix Size and Entries

## Question

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

## Solution

### 1. Sizes

$A$ has 2 rows and 3 columns, so $A$ is $2\times3$.
$B$ has 3 rows and 2 columns, so $B$ is $3\times2$.

### 2. Entries

The entry $a_{ij}$ is in row $i$, column $j$.

$$
a_{12}=-1,\qquad a_{23}=5,\qquad b_{21}=-2,\qquad b_{32}=1.
$$

### 3. Row and column as vectors

$$
\text{row 2 of }A=\begin{pmatrix}0 & 4 & 5\end{pmatrix},\qquad
\text{column 1 of }B=\begin{pmatrix}1\\-2\\4\end{pmatrix}.
$$

## Explanation

The size is written as (number of rows) × (number of columns), and the first index of an entry is its row, the second is its column. Check: the second row of $A$ has 3 entries (as many as $A$ has columns), and the first column of $B$ has 3 entries (as many as $B$ has rows).
