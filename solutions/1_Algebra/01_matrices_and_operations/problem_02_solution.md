### Exercise 2. Solution

Matrices are added, subtracted and multiplied by a number **entry by entry**.

**1. Sum $A+B$**

$$
A+B=\begin{pmatrix} 1+4 & 2+(-2) \cr -1+0 & 3+5 \end{pmatrix}=\begin{pmatrix} 5 & 0 \cr -1 & 8 \end{pmatrix}
$$

**2. Difference $A-B$**

$$
A-B=\begin{pmatrix} 1-4 & 2-(-2) \cr -1-0 & 3-5 \end{pmatrix}=\begin{pmatrix} -3 & 4 \cr -1 & -2 \end{pmatrix}
$$

**3. Combination $3A-2B$**

First multiply each matrix by its number:

$$
3A=\begin{pmatrix} 3 & 6 \cr -3 & 9 \end{pmatrix},\qquad 2B=\begin{pmatrix} 8 & -4 \cr 0 & 10 \end{pmatrix}
$$

Then subtract entry by entry:

$$
3A-2B=\begin{pmatrix} 3-8 & 6-(-4) \cr -3-0 & 9-10 \end{pmatrix}=\begin{pmatrix} -5 & 10 \cr -3 & -1 \end{pmatrix}
$$

**4. Why addition needs matrices of the same size**

Addition works entry by entry: the entry $a_{ij}$ is added to the entry $b_{ij}$ in the same position. If $A$ and $B$ have different sizes, some entries of one matrix have no partner in the other matrix, so the sum is not defined. For example, a $2 \times 2$ matrix and a $2 \times 3$ matrix cannot be added, because the third column has nothing to be added to.

**Answers:**

$$
A+B=\begin{pmatrix} 5 & 0 \cr -1 & 8 \end{pmatrix},\quad A-B=\begin{pmatrix} -3 & 4 \cr -1 & -2 \end{pmatrix},\quad 3A-2B=\begin{pmatrix} -5 & 10 \cr -3 & -1 \end{pmatrix}
$$
