### Exercise 7. Solution

Here $I$ is the $2\times2$ identity matrix and $0$ is the $2\times2$ zero matrix:

$$
I=\begin{pmatrix} 1 & 0 \cr 0 & 1 \end{pmatrix},\qquad 0=\begin{pmatrix} 0 & 0 \cr 0 & 0 \end{pmatrix}
$$

**1. Products with $I$**

$$
AI=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}\begin{pmatrix} 1 & 0 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 2\cdot1+1\cdot0 & 2\cdot0+1\cdot1 \cr 0\cdot1+2\cdot0 & 0\cdot0+2\cdot1 \end{pmatrix}=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=A
$$

$$
IA=\begin{pmatrix} 1 & 0 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=\begin{pmatrix} 1\cdot2+0\cdot0 & 1\cdot1+0\cdot2 \cr 0\cdot2+1\cdot0 & 0\cdot1+1\cdot2 \end{pmatrix}=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=A
$$

**2. Sum with $0$**

$$
A+0=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}+\begin{pmatrix} 0 & 0 \cr 0 & 0 \end{pmatrix}=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=A
$$

**3. Square $A^2$**

$$
A^2=AA=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=\begin{pmatrix} 2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \cr 0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \end{pmatrix}=\begin{pmatrix} 4 & 4 \cr 0 & 4 \end{pmatrix}
$$

**4. Cube $A^3$**

$$
A^3=A^2A=\begin{pmatrix} 4 & 4 \cr 0 & 4 \end{pmatrix}\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix}=\begin{pmatrix} 4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \cr 0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \end{pmatrix}=\begin{pmatrix} 8 & 12 \cr 0 & 8 \end{pmatrix}
$$

**5. Roles of $I$ and $0$**

- $I$ is the neutral element for multiplication: $AI=IA=A$. It plays the role of the number $1$.
- $0$ is the neutral element for addition: $A+0=A$. It plays the role of the number $0$.

**6. Pattern in the powers**

$$
A^1=\begin{pmatrix} 2 & 1 \cr 0 & 2 \end{pmatrix},\qquad A^2=\begin{pmatrix} 4 & 4 \cr 0 & 4 \end{pmatrix},\qquad A^3=\begin{pmatrix} 8 & 12 \cr 0 & 8 \end{pmatrix}
$$

- The matrix stays upper triangular (zero in the bottom-left corner).
- The diagonal entries are $2,\ 4,\ 8$, that is, $2^n$.
- The top-right entries are $1,\ 4,\ 12$, that is, $n\cdot2^{n-1}$.

This suggests the general formula (observed from the pattern, not proved here):

$$
A^n=\begin{pmatrix} 2^n & n\cdot2^{n-1} \cr 0 & 2^n \end{pmatrix}
$$

Check: for $n=3$ we get $2^3=8$ and $3\cdot2^2=12$, which matches $A^3$.

**Answers:**

$$
AI=A,\qquad IA=A,\qquad A+0=A,\qquad A^2=\begin{pmatrix} 4 & 4 \cr 0 & 4 \end{pmatrix},\qquad A^3=\begin{pmatrix} 8 & 12 \cr 0 & 8 \end{pmatrix}
$$
