### Exercise 8. Solution

Each operation changes only one row (or swaps two rows), and the other rows stay the same.

**Start**

$$
A=\begin{pmatrix} 1 & 2 & -1 \cr 2 & 4 & 1 \cr -1 & 1 & 3 \end{pmatrix}
$$

**Step 1. $R_2\leftarrow R_2-2R_1$**

New $R_2=(2-2\cdot1,\ 4-2\cdot2,\ 1-2\cdot(-1))=(0,\ 0,\ 3)$.

$$
A_1=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr -1 & 1 & 3 \end{pmatrix}
$$

**Step 2. $R_3\leftarrow R_3+R_1$**

New $R_3=(-1+1,\ 1+2,\ 3+(-1))=(0,\ 3,\ 2)$.

$$
A_2=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr 0 & 3 & 2 \end{pmatrix}
$$

**Step 3. Interchange $R_2$ and $R_3$**

$$
A_3=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 3 & 2 \cr 0 & 0 & 3 \end{pmatrix}
$$

The final matrix is upper triangular (zeros below the diagonal).

**Reversing the operations**

| Operation | Reverse operation |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | $R_2\leftarrow R_2+2R_1$ |
| $R_3\leftarrow R_3+R_1$ | $R_3\leftarrow R_3-R_1$ |
| interchange $R_2$ and $R_3$ | interchange $R_2$ and $R_3$ again |

To undo the whole sequence, apply the reverse operations in the **opposite order**: first swap $R_2$ and $R_3$, then $R_3\leftarrow R_3-R_1$, then $R_2\leftarrow R_2+2R_1$.

**Check.** Starting from $A_3$:

$$
\begin{pmatrix} 1 & 2 & -1 \cr 0 & 3 & 2 \cr 0 & 0 & 3 \end{pmatrix}\to\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr 0 & 3 & 2 \end{pmatrix}\to\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr -1 & 1 & 3 \end{pmatrix}\to\begin{pmatrix} 1 & 2 & -1 \cr 2 & 4 & 1 \cr -1 & 1 & 3 \end{pmatrix}=A
$$

We return to the original matrix $A$, so every operation is reversible.

**Answers:**

$$
A_1=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr -1 & 1 & 3 \end{pmatrix},\quad A_2=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 0 & 3 \cr 0 & 3 & 2 \end{pmatrix},\quad A_3=\begin{pmatrix} 1 & 2 & -1 \cr 0 & 3 & 2 \cr 0 & 0 & 3 \end{pmatrix}
$$
