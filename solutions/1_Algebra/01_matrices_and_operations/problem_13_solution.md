### Exercise 13. Solution

Denote the Fibonacci numbers by $F_0=0,\ F_1=1,\ F_2=1,\ F_3=2,\ F_4=3,\ F_5=5,\ F_6=8,\dots$ with the rule $F_{k+1}=F_k+F_{k-1}$. (The matrix is called $\mathbf{F}$ below only when needed; the numbers carry indices.)

**1. Powers of the matrix**

$$
F^2=FF=\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} 1\cdot1+1\cdot1 & 1\cdot1+1\cdot0 \cr 1\cdot1+0\cdot1 & 1\cdot1+0\cdot0 \end{pmatrix}=\begin{pmatrix} 2 & 1 \cr 1 & 1 \end{pmatrix}
$$

$$
F^3=F^2F=\begin{pmatrix} 2 & 1 \cr 1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} 2\cdot1+1\cdot1 & 2\cdot1+1\cdot0 \cr 1\cdot1+1\cdot1 & 1\cdot1+1\cdot0 \end{pmatrix}=\begin{pmatrix} 3 & 2 \cr 2 & 1 \end{pmatrix}
$$

$$
F^4=F^3F=\begin{pmatrix} 3 & 2 \cr 2 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} 3\cdot1+2\cdot1 & 3\cdot1+2\cdot0 \cr 2\cdot1+1\cdot1 & 2\cdot1+1\cdot0 \end{pmatrix}=\begin{pmatrix} 5 & 3 \cr 3 & 2 \end{pmatrix}
$$

$$
F^5=F^4F=\begin{pmatrix} 5 & 3 \cr 3 & 2 \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} 5\cdot1+3\cdot1 & 5\cdot1+3\cdot0 \cr 3\cdot1+2\cdot1 & 3\cdot1+2\cdot0 \end{pmatrix}=\begin{pmatrix} 8 & 5 \cr 5 & 3 \end{pmatrix}
$$

**2. Relationship with the sequence $0,1,1,2,3,5,8,\ldots$**

$$
F^1=\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}=\begin{pmatrix} F_2 & F_1 \cr F_1 & F_0 \end{pmatrix},\qquad F^2=\begin{pmatrix} 2 & 1 \cr 1 & 1 \end{pmatrix}=\begin{pmatrix} F_3 & F_2 \cr F_2 & F_1 \end{pmatrix}
$$

$$
F^3=\begin{pmatrix} F_4 & F_3 \cr F_3 & F_2 \end{pmatrix},\qquad F^4=\begin{pmatrix} F_5 & F_4 \cr F_4 & F_3 \end{pmatrix},\qquad F^5=\begin{pmatrix} F_6 & F_5 \cr F_5 & F_4 \end{pmatrix}
$$

All entries of the powers are consecutive Fibonacci numbers. The observed pattern (not proved here) is

$$
F^n=\begin{pmatrix} F_{n+1} & F_n \cr F_n & F_{n-1} \end{pmatrix}
$$

**3. One recurrence step**

$$
F\begin{pmatrix} a \cr b \end{pmatrix}=\begin{pmatrix} 1 & 1 \cr 1 & 0 \end{pmatrix}\begin{pmatrix} a \cr b \end{pmatrix}=\begin{pmatrix} a+b \cr a \end{pmatrix}
$$

If the vector contains two consecutive terms, $a=F_{k+1}$ and $b=F_k$, then

$$
F\begin{pmatrix} F_{k+1} \cr F_k \end{pmatrix}=\begin{pmatrix} F_{k+1}+F_k \cr F_{k+1} \end{pmatrix}=\begin{pmatrix} F_{k+2} \cr F_{k+1} \end{pmatrix}
$$

- The first row $(1,\ 1)$ creates the sum $a+b$, which is the new term.
- The second row $(1,\ 0)$ copies $a$, so the newer of the two terms is kept for the next step.

So one multiplication by $F$ moves the pair $(F_{k+1},F_k)$ one step forward to $(F_{k+2},F_{k+1})$. Starting from $\begin{pmatrix} F_1 \cr F_0 \end{pmatrix}=\begin{pmatrix} 1 \cr 0 \end{pmatrix}$ and applying $F$ exactly $n$ times, we get

$$
F^n\begin{pmatrix} 1 \cr 0 \end{pmatrix}=\begin{pmatrix} F_{n+1} \cr F_n \end{pmatrix}
$$

which is the first column of $F^n$, as seen above.

**Answers:**

$$
F^2=\begin{pmatrix} 2 & 1 \cr 1 & 1 \end{pmatrix},\quad F^3=\begin{pmatrix} 3 & 2 \cr 2 & 1 \end{pmatrix},\quad F^4=\begin{pmatrix} 5 & 3 \cr 3 & 2 \end{pmatrix},\quad F^5=\begin{pmatrix} 8 & 5 \cr 5 & 3 \end{pmatrix}
$$

$$
F\begin{pmatrix} a \cr b \end{pmatrix}=\begin{pmatrix} a+b \cr a \end{pmatrix}
$$
