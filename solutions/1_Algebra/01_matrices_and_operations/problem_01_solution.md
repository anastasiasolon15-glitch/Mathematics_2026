# Exercise 1. Matrix Size and Entries

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

### Steps

A matrix with $m$ rows and $n$ columns has size $m\times n$. The entry $a_{ij}$ lies in row $i$ and column $j$.

- $A$ has 2 rows and 3 columns.
- $B$ has 3 rows and 2 columns.
- $a_{12}$ is in row 1, column 2 of $A$.
- $a_{23}$ is in row 2, column 3 of $A$.
- $b_{21}$ is in row 2, column 1 of $B$.
- $b_{32}$ is in row 3, column 2 of $B$.

### Result

Sizes: $A$ is $2\times3$, $B$ is $3\times2$.

Entries:

$$
a_{12}=-1,\qquad a_{23}=5,\qquad b_{21}=-2,\qquad b_{32}=1.
$$

The second row of $A$ is the row vector $(0,\ 4,\ 5)$.

The first column of $B$ is

$$
\begin{pmatrix}
1 \\
-2 \\
4 \\
\end{pmatrix}.
$$

### Method

The first index always denotes the row and the second index the column. A row of a matrix is a row vector, a column is a column vector.

### Verification

The number of entries equals the product of the dimensions: $A$ has $2\cdot3=6$ entries and $B$ has $3\cdot2=6$ entries, which matches the displayed matrices. The second row of $A$ has 3 entries (the number of columns of $A$), and the first column of $B$ has 3 entries (the number of rows of $B$).
