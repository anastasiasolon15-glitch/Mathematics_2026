### Exercise 15. Solution

Sizes: $A$ is $2\times3$, $B$ is $3\times2$, $C$ is $2\times2$. Both $(AB)C$ and $A(BC)$ are defined and have size $2\times2$.

**1. Path 1: $(AB)C$**

First $AB$ (size $2\times2$):

$$
AB=\begin{pmatrix} 1 & 2 & 0 \cr 0 & 1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \cr 2 & 1 \cr -1 & 3 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot2+0\cdot(-1) & 1\cdot0+2\cdot1+0\cdot3 \cr 0\cdot1+1\cdot2+1\cdot(-1) & 0\cdot0+1\cdot1+1\cdot3 \end{pmatrix}=\begin{pmatrix} 5 & 2 \cr 1 & 4 \end{pmatrix}
$$

Then multiply by $C$:

$$
(AB)C=\begin{pmatrix} 5 & 2 \cr 1 & 4 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 0 & -1 \end{pmatrix}=\begin{pmatrix} 5\cdot2+2\cdot0 & 5\cdot1+2\cdot(-1) \cr 1\cdot2+4\cdot0 & 1\cdot1+4\cdot(-1) \end{pmatrix}=\begin{pmatrix} 10 & 3 \cr 2 & -3 \end{pmatrix}
$$

**2. Path 2: $A(BC)$**

First $BC$ (size $3\times2$):

$$
BC=\begin{pmatrix} 1 & 0 \cr 2 & 1 \cr -1 & 3 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 0 & -1 \end{pmatrix}=\begin{pmatrix} 1\cdot2+0\cdot0 & 1\cdot1+0\cdot(-1) \cr 2\cdot2+1\cdot0 & 2\cdot1+1\cdot(-1) \cr -1\cdot2+3\cdot0 & -1\cdot1+3\cdot(-1) \end{pmatrix}=\begin{pmatrix} 2 & 1 \cr 4 & 1 \cr -2 & -4 \end{pmatrix}
$$

Then multiply $A$ by $BC$:

$$
A(BC)=\begin{pmatrix} 1 & 2 & 0 \cr 0 & 1 & 1 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 4 & 1 \cr -2 & -4 \end{pmatrix}=\begin{pmatrix} 1\cdot2+2\cdot4+0\cdot(-2) & 1\cdot1+2\cdot1+0\cdot(-4) \cr 0\cdot2+1\cdot4+1\cdot(-2) & 0\cdot1+1\cdot1+1\cdot(-4) \end{pmatrix}=\begin{pmatrix} 10 & 3 \cr 2 & -3 \end{pmatrix}
$$

**3. Comparison of results**

$$
(AB)C=\begin{pmatrix} 10 & 3 \cr 2 & -3 \end{pmatrix}=A(BC)
$$

The results are identical.

**4. Comparison of the amount of work**

Multiplying a $p\times q$ matrix by a $q\times r$ matrix takes $p\cdot q\cdot r$ multiplications.

| Path | Step 1 | Step 2 | Total multiplications |
|---|---|---|---|
| $(AB)C$ | $AB$: $2\cdot3\cdot2=12$ | $(AB)C$: $2\cdot2\cdot2=8$ | $20$ |
| $A(BC)$ | $BC$: $3\cdot2\cdot2=12$ | $A(BC)$: $2\cdot3\cdot2=12$ | $24$ |

The first path is cheaper: $20$ multiplications against $24$. The additions follow the same trend: $8+4=12$ for the first path and $6+8=14$ for the second.

**5. What associativity means**

Associativity says that $(AB)C=A(BC)$: when three matrices are multiplied, it does not matter which pair is multiplied first, as long as the order of the matrices $A,B,C$ is kept. The final matrix is always the same, but the intermediate matrices differ ($AB$ is $2\times2$, while $BC$ is $3\times2$) and so does the amount of work. Associativity does not mean that the order of the factors can be changed: $ACB$ would be a different (and here undefined) product, because multiplication is not commutative.

**Answer:**

$$
(AB)C=A(BC)=\begin{pmatrix} 10 & 3 \cr 2 & -3 \end{pmatrix}
$$
