### Exercise 6. Solution

**Rule.** The transpose $X^T$ is obtained by turning rows into columns: the entry in row $i$, column $j$ of $X$ becomes the entry in row $j$, column $i$ of $X^T$. If $X$ is $m\times n$, then $X^T$ is $n\times m$.

**1. Transposes**

$$
A^T=\begin{pmatrix} 1 & 4 \cr 2 & 5 \cr 3 & 6 \end{pmatrix},\qquad B^T=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 1 & 3 \end{pmatrix}
$$

Sizes: $A$ is $2\times3$, so $A^T$ is $3\times2$; $B$ is $3\times2$, so $B^T$ is $2\times3$.

**2. Product $AB$**

$A$ is $2\times3$ and $B$ is $3\times2$, so $AB$ is defined and has size $2\times2$.

$$
AB=\begin{pmatrix} 1 & 2 & 3 \cr 4 & 5 & 6 \end{pmatrix}\begin{pmatrix} 1 & 0 \cr 2 & 1 \cr -1 & 3 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot2+3\cdot(-1) & 1\cdot0+2\cdot1+3\cdot3 \cr 4\cdot1+5\cdot2+6\cdot(-1) & 4\cdot0+5\cdot1+6\cdot3 \end{pmatrix}=\begin{pmatrix} 2 & 11 \cr 8 & 23 \end{pmatrix}
$$

**3. Left side: $(AB)^T$**

$$
(AB)^T=\begin{pmatrix} 2 & 11 \cr 8 & 23 \end{pmatrix}^T=\begin{pmatrix} 2 & 8 \cr 11 & 23 \end{pmatrix}
$$

**4. Right side: $B^TA^T$**

$B^T$ is $2\times3$ and $A^T$ is $3\times2$, so the product is defined and has size $2\times2$.

$$
B^TA^T=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 1 & 3 \end{pmatrix}\begin{pmatrix} 1 & 4 \cr 2 & 5 \cr 3 & 6 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot2+(-1)\cdot3 & 1\cdot4+2\cdot5+(-1)\cdot6 \cr 0\cdot1+1\cdot2+3\cdot3 & 0\cdot4+1\cdot5+3\cdot6 \end{pmatrix}=\begin{pmatrix} 2 & 8 \cr 11 & 23 \end{pmatrix}
$$

**5. Conclusion**

Both sides are equal, so the property is verified in this example:

$$
(AB)^T=B^TA^T=\begin{pmatrix} 2 & 8 \cr 11 & 23 \end{pmatrix}
$$

Note that the order of the factors reverses. Writing $A^TB^T$ instead would give a $3\times3$ matrix, which cannot equal the $2\times2$ matrix $(AB)^T$.

**Answers:**

$$
A^T=\begin{pmatrix} 1 & 4 \cr 2 & 5 \cr 3 & 6 \end{pmatrix},\quad B^T=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 1 & 3 \end{pmatrix},\quad AB=\begin{pmatrix} 2 & 11 \cr 8 & 23 \end{pmatrix}
$$
