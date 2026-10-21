# Exercise 11. When Do Matrices Commute?

## Question

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

## Solution

### Steps

Compute both products:

$$
AB=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix},\qquad
BA=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

The equality $AB=BA$ means that all four entries agree:

$$
\begin{cases}
a+c=a, \\
b+d=a+b, \\
c=c, \\
d=c+d.
\end{cases}
$$

The first and last equations give $c=0$. The second equation gives $d=a$. The third equation holds always.

### Result

The matrices $A$ and $B$ commute if and only if $c=0$ and $d=a$. All such matrices have the form

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix},\qquad a,b\in\mathbb{R}.
$$

Equivalently, since $A-I$ has a single nonzero entry $1$ in position $(1,2)$,

$$
B=(a-b)I+bA.
$$

### Method

The condition $AB=BA$ is a system of linear equations in the unknown entries of $B$. Solving it describes the whole family of matrices commuting with $A$. This family is two-dimensional, with free parameters $a$ and $b$.

### Verification

For $B$ of the found form:

$$
\begin{aligned}
AB &=
\begin{pmatrix}
a & a+b \\
0 & a \\
\end{pmatrix} \\
&= BA.
\end{aligned}
$$

The identity $B=(a-b)I+bA$ is confirmed by expanding:

$$
\begin{aligned}
(a-b)I+bA &=
\begin{pmatrix}
a-b+b & b \\
0 & a-b+b \\
\end{pmatrix} \\
&=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}.
\end{aligned}
$$

Moreover, $I$ and $A$ both commute with $A$, so any combination $(a-b)I+bA$ commutes with $A$, which confirms the result independently.
