# Matrices and Basic Operations — Exercise 4. Matrix Multiplication and Noncommutativity

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
2+6 & 0+2 \\
0+3 & 0+1 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}.
$$

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
2+0 & 4+0 \\
3+0 & 6+1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

Since 

$$
\begin{pmatrix}
8 & 2 \\
3 & 1 
\end{pmatrix}
\neq
\begin{pmatrix}
2 & 4 \\
3 & 7 
\end{pmatrix},
$$

we have $AB \neq BA$.

## Explanation

### What Noncommutativity Means
Both products are defined and have the same size ($2 \times 2$), yet they yield different matrices. 

Noncommutativity means that the order of the factors matters: in general, $AB \neq BA$. This contrasts sharply with ordinary numbers, where multiplication is commutative ($ab = ba$). 

### Conclusion
Finding even a single counterexample where $AB \neq BA$ is sufficient to prove that matrix multiplication is not commutative in general.
