### Exercise 5. Solution

**1. Product $Ax$ (row by column)**

Each entry of $Ax$ is a row of $A$ multiplied entry by entry with the vector $x$, and the products are added up.

$$
Ax=\begin{pmatrix} 2 & -1 \cr 1 & 3 \end{pmatrix}\begin{pmatrix} 4 \cr 2 \end{pmatrix}=\begin{pmatrix} 2\cdot4+(-1)\cdot2 \cr 1\cdot4+3\cdot2 \end{pmatrix}=\begin{pmatrix} 6 \cr 10 \end{pmatrix}
$$

**2. Linear combination of the columns of $A$**

The columns of $A$ are

$$
a_1=\begin{pmatrix} 2 \cr 1 \end{pmatrix},\qquad a_2=\begin{pmatrix} -1 \cr 3 \end{pmatrix}
$$

The coefficients are the entries of $x$: $x_1=4$ and $x_2=2$. Then

$$
Ax=4\begin{pmatrix} 2 \cr 1 \end{pmatrix}+2\begin{pmatrix} -1 \cr 3 \end{pmatrix}=\begin{pmatrix} 8 \cr 4 \end{pmatrix}+\begin{pmatrix} -2 \cr 6 \end{pmatrix}=\begin{pmatrix} 6 \cr 10 \end{pmatrix}
$$

Both methods give the same result.

**3. Meaning**

Multiplying a matrix by a vector means taking a combination of the columns of the matrix: the first entry of $x$ says how many copies of the first column to take, the second entry says how many copies of the second column to take, and so on.

**Answers:**

$$
Ax=\begin{pmatrix} 6 \cr 10 \end{pmatrix}=4a_1+2a_2
$$
