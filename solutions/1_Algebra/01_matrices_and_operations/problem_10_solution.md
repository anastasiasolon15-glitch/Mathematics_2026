### Exercise 10. Solution

The columns of $B$ are

$$
b_1=\begin{pmatrix} 1 \cr -1 \cr 3 \end{pmatrix},\qquad b_2=\begin{pmatrix} 2 \cr 0 \cr 1 \end{pmatrix}
$$

$A$ is $2\times3$ and each $b_j$ is $3\times1$, so $Ab_1$ and $Ab_2$ are defined and have size $2\times1$.

**1. Products $Ab_1$ and $Ab_2$**

$$
Ab_1=\begin{pmatrix} 1 & 2 & 0 \cr 0 & 1 & 1 \end{pmatrix}\begin{pmatrix} 1 \cr -1 \cr 3 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot(-1)+0\cdot3 \cr 0\cdot1+1\cdot(-1)+1\cdot3 \end{pmatrix}=\begin{pmatrix} -1 \cr 2 \end{pmatrix}
$$

$$
Ab_2=\begin{pmatrix} 1 & 2 & 0 \cr 0 & 1 & 1 \end{pmatrix}\begin{pmatrix} 2 \cr 0 \cr 1 \end{pmatrix}=\begin{pmatrix} 1\cdot2+2\cdot0+0\cdot1 \cr 0\cdot2+1\cdot0+1\cdot1 \end{pmatrix}=\begin{pmatrix} 2 \cr 1 \end{pmatrix}
$$

**2. Product $AB$**

$A$ is $2\times3$ and $B$ is $3\times2$, so $AB$ is defined and has size $2\times2$.

$$
AB=\begin{pmatrix} 1 & 2 & 0 \cr 0 & 1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 2 \cr -1 & 0 \cr 3 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot(-1)+0\cdot3 & 1\cdot2+2\cdot0+0\cdot1 \cr 0\cdot1+1\cdot(-1)+1\cdot3 & 0\cdot2+1\cdot0+1\cdot1 \end{pmatrix}=\begin{pmatrix} -1 & 2 \cr 2 & 1 \end{pmatrix}
$$

**3. Comparison and explanation**

The first column of $AB$ is $\begin{pmatrix} -1 \cr 2 \end{pmatrix}=Ab_1$, and the second column is $\begin{pmatrix} 2 \cr 1 \end{pmatrix}=Ab_2$. So

$$
AB=\begin{pmatrix} Ab_1 & Ab_2 \end{pmatrix}
$$

**Why this is true.** The entry in row $i$, column $j$ of $AB$ is (row $i$ of $A$) multiplied by (column $j$ of $B$). Column $j$ of $B$ is $b_j$, so the whole column $j$ of $AB$ is made of the entries (row $i$ of $A$)$\cdot b_j$ for $i=1,2$. But these are exactly the entries of the vector $Ab_j$. Therefore column $j$ of $AB$ equals $Ab_j$.

In other words, $A$ acts on each column of $B$ separately, and the results are placed side by side as the columns of $AB$.

**Answers:**

$$
Ab_1=\begin{pmatrix} -1 \cr 2 \end{pmatrix},\qquad Ab_2=\begin{pmatrix} 2 \cr 1 \end{pmatrix},\qquad AB=\begin{pmatrix} -1 & 2 \cr 2 & 1 \end{pmatrix}
$$
