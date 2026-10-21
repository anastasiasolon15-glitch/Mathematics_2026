# Exercise 13. A Recurrence Written in Matrix Form

## Question

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

### Steps

Let $f_0=0$, $f_1=1$, $f_2=1$, $f_3=2$, $f_4=3$, $f_5=5$, $f_6=8$ denote the Fibonacci numbers.

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad
F^3=F^2F=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

$$
F^4=F^3F=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},\qquad
F^5=F^4F=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}
$$

The entries of the powers are Fibonacci numbers:

$$
F^n=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix}.
$$

For $n=5$ this gives $f_6=8$, $f_5=5$, $f_4=3$, which matches $F^5$.

The action of $F$ on a vector:

$$
\begin{aligned}
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix} &=
\begin{pmatrix}
1\cdot a+1\cdot b \\
1\cdot a+0\cdot b \\
\end{pmatrix} \\
&=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
\end{aligned}
$$

### Result

The powers of $F$ contain consecutive Fibonacci numbers, and multiplication by $F$ maps the pair $(a,b)$ to $(a+b,\ a)$.

### Method

If $(a,b)=(f_{n+1},f_n)$ are two consecutive terms, then

$$
\begin{aligned}
F
\begin{pmatrix}
f_{n+1} \\
f_n \\
\end{pmatrix} &=
\begin{pmatrix}
f_{n+1}+f_n \\
f_{n+1} \\
\end{pmatrix} \\
&=
\begin{pmatrix}
f_{n+2} \\
f_{n+1} \\
\end{pmatrix}.
\end{aligned}
$$

The first row of $F$ creates the sum of the two terms, and the second row keeps the larger term $f_{n+1}$ for the next step. Hence $n$ applications of $F$ to $(f_1,f_0)=(1,0)$ give $(f_{n+1},f_n)$, which is the first column of $F^n$.

### Verification

The first column of $F^5$ is $(8,5)=(f_6,f_5)$. The determinant check also works: $\det F=-1$, and $\det F^5=8\cdot3-5\cdot5=-1=(-1)^5$.
