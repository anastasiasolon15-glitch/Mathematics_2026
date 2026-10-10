### Exercise 12. Solution

**1. Powers of $A$**

$$
A^2=AA=\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot1+1\cdot0 & 1\cdot1+1\cdot1 \cr 0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \end{pmatrix}=\begin{pmatrix} 1 & 2 \cr 0 & 1 \end{pmatrix}
$$

$$
A^3=A^2A=\begin{pmatrix} 1 & 2 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot1+2\cdot0 & 1\cdot1+2\cdot1 \cr 0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \end{pmatrix}=\begin{pmatrix} 1 & 3 \cr 0 & 1 \end{pmatrix}
$$

$$
A^4=A^3A=\begin{pmatrix} 1 & 3 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot1+3\cdot0 & 1\cdot1+3\cdot1 \cr 0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \end{pmatrix}=\begin{pmatrix} 1 & 4 \cr 0 & 1 \end{pmatrix}
$$

**2. Pattern and conjecture**

$$
A^1=\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix},\quad A^2=\begin{pmatrix} 1 & 2 \cr 0 & 1 \end{pmatrix},\quad A^3=\begin{pmatrix} 1 & 3 \cr 0 & 1 \end{pmatrix},\quad A^4=\begin{pmatrix} 1 & 4 \cr 0 & 1 \end{pmatrix}
$$

The diagonal entries stay $1$, the bottom-left entry stays $0$, and the top-right entry equals the exponent. Conjecture:

$$
A^n=\begin{pmatrix} 1 & n \cr 0 & 1 \end{pmatrix},\qquad n=1,2,3,\dots
$$

**3. Proof by induction**

*Base case.* For $n=1$ the formula gives $\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=A$, which is true.

*Inductive step.* Assume the formula holds for some $n$:

$$
A^n=\begin{pmatrix} 1 & n \cr 0 & 1 \end{pmatrix}
$$

Multiply by $A$:

$$
A^{n+1}=A^nA=\begin{pmatrix} 1 & n \cr 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} 1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \cr 0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \end{pmatrix}=\begin{pmatrix} 1 & n+1 \cr 0 & 1 \end{pmatrix}
$$

This is exactly the formula for $n+1$. By induction, the formula holds for every natural $n$.

**Why it works.** Multiplying by $A$ on the right adds the first column to the second column. The first column of $A^n$ is $(1,0)^T$, so each multiplication adds $1$ to the top-right entry and changes nothing else.

**Answer:**

$$
A^n=\begin{pmatrix} 1 & n \cr 0 & 1 \end{pmatrix}
$$
