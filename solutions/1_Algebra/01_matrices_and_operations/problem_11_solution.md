### Exercise 11. Solution

**1. Compute $AB$**

$$
AB=\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}\begin{pmatrix} a & b \cr c & d \end{pmatrix}=\begin{pmatrix} a+c & b+d \cr c & d \end{pmatrix}
$$

**2. Compute $BA$**

$$
BA=\begin{pmatrix} a & b \cr c & d \end{pmatrix}\begin{pmatrix} 1 & 1 \cr 0 & 1 \end{pmatrix}=\begin{pmatrix} a & a+b \cr c & c+d \end{pmatrix}
$$

**3. Condition $AB=BA$**

Two matrices are equal when all their entries are equal, so we compare entry by entry:

- top-left: $a+c=a$, so $c=0$;
- top-right: $b+d=a+b$, so $d=a$;
- bottom-left: $c=c$, always true;
- bottom-right: $d=c+d$, so $c=0$.

The conditions are therefore

$$
c=0,\qquad d=a,
$$

and $a$ and $b$ can be any numbers.

**4. General form of $B$**

$$
B=\begin{pmatrix} a & b \cr 0 & a \end{pmatrix}=a\begin{pmatrix} 1 & 0 \cr 0 & 1 \end{pmatrix}+b\begin{pmatrix} 0 & 1 \cr 0 & 0 \end{pmatrix}=aI+bN,\qquad N=A-I
$$

So the matrices that commute with $A$ are exactly the matrices of the form $aI+bA'$, where $A'$ is any combination of $I$ and $A$ (since $N=A-I$, we get $B=(a-b)I+bA$).

**5. Check**

Take $a=2$, $b=3$, so $B=\begin{pmatrix} 2 & 3 \cr 0 & 2 \end{pmatrix}$. Then

$$
AB=\begin{pmatrix} 2 & 5 \cr 0 & 2 \end{pmatrix},\qquad BA=\begin{pmatrix} 2 & 5 \cr 0 & 2 \end{pmatrix}
$$

Both products are equal, as expected.

**Answers:**

$$
AB=BA\iff c=0\ \text{and}\ d=a,\qquad B=\begin{pmatrix} a & b \cr 0 & a \end{pmatrix}\ (a,b\in\mathbb{R})
$$
