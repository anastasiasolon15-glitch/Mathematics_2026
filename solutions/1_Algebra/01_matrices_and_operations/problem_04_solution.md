### Exercise 4. Solution

**Rule.** The entry in row $i$, column $j$ of $XY$ is the row $i$ of $X$ multiplied entry by entry with the column $j$ of $Y$, and the products are added up.

**1. Product $AB$**

$$
AB=\begin{pmatrix} 1 & 2 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 2 & 0 \cr 3 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \cr 0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \end{pmatrix}=\begin{pmatrix} 8 & 2 \cr 3 & 1 \end{pmatrix}
$$

**2. Product $BA$**

$$
BA=\begin{pmatrix} 2 & 0 \cr 3 & 1 \end{pmatrix}\begin{pmatrix} 1 & 2 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \cr 3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \end{pmatrix}=\begin{pmatrix} 2 & 4 \cr 3 & 7 \end{pmatrix}
$$

**3. Comparison**

$$
AB=\begin{pmatrix} 8 & 2 \cr 3 & 1 \end{pmatrix}\neq\begin{pmatrix} 2 & 4 \cr 3 & 7 \end{pmatrix}=BA
$$

So $AB\neq BA$. Even the entries in the top-left corner differ: $8\neq2$.

**4. What noncommutativity means**

For numbers, $a\cdot b=b\cdot a$ always. For matrices this is false in general: the order of the factors matters, and in this example swapping $A$ and $B$ gives a different matrix. Both products are defined here because the matrices are square and of the same size, so the difference comes from the multiplication itself, not from incompatible dimensions. (In Exercise 3, $AB$ was defined while $BA$ was not, which is an even stronger form of the same effect.)

**Answers:**

$$
AB=\begin{pmatrix} 8 & 2 \cr 3 & 1 \end{pmatrix},\qquad BA=\begin{pmatrix} 2 & 4 \cr 3 & 7 \end{pmatrix},\qquad AB\neq BA
$$
