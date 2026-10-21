# Exercise 12. Formula for a Matrix Power

## Question

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

## Solution

### Steps

$$
A^2=AA=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad
A^3=A^2A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},\qquad
A^4=A^3A=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

In each step the upper right entry increases by $1$, so the conjecture is

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix},\qquad n\ge1.
$$

Proof by induction.

Base case: for $n=1$ the formula gives $A$, which is correct.

Inductive step: assume the formula holds for some $n$. Then

$$
\begin{aligned}
A^{n+1}=A^nA &=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \\
0 & 1 \\
\end{pmatrix} \\
&=
\begin{pmatrix}
1 & n+1 \\
0 & 1 \\
\end{pmatrix}.
\end{aligned}
$$

### Result

For all $n\ge1$:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

### Method

The product above is exactly the formula with $n$ replaced by $n+1$. Together with the base case, the induction principle gives the formula for all $n\ge1$. Checking further particular cases would only support the conjecture. The inductive step shows that the pattern cannot break.

### Verification

The formula reproduces the computed matrices for $n=2,3,4$. Multiplying in the other order also works: $AA^n$ has first row $(1,\ 1+n)$ and second row $(0,\ 1)$, which is the same matrix.
