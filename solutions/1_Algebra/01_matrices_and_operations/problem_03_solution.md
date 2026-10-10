### Exercise 3. Solution

**Condition.** The product $XY$ is defined only if the number of **columns** of $X$ equals the number of **rows** of $Y$. If $X$ is $m \times n$ and $Y$ is $n \times p$, then $XY$ is defined and has size $m \times p$.

Sizes:

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}
$$

**Check of each product**

| Product | Sizes | Inner numbers | Defined? | Size of result |
|---|---|---|---|---|
| $AB$ | $2\times3$ and $3\times4$ | $3 = 3$ | Yes | $2\times4$ |
| $BA$ | $3\times4$ and $2\times3$ | $4 \neq 2$ | No | none |
| $BC$ | $3\times4$ and $4\times2$ | $4 = 4$ | Yes | $3\times2$ |
| $CB$ | $4\times2$ and $3\times4$ | $2 \neq 3$ | No | none |
| $AC$ | $2\times3$ and $4\times2$ | $3 \neq 4$ | No | none |
| $CA$ | $4\times2$ and $2\times3$ | $2 = 2$ | Yes | $4\times3$ |
| $AD$ | $2\times3$ and $2\times2$ | $3 \neq 2$ | No | none |
| $DA$ | $2\times2$ and $2\times3$ | $2 = 2$ | Yes | $2\times3$ |

**Justification**

- $AB$: columns of $A$ is $3$, rows of $B$ is $3$, so the product is defined and the result is $2\times4$.
- $BA$: columns of $B$ is $4$, rows of $A$ is $2$, they differ, so the product is not defined.
- $BC$: columns of $B$ is $4$, rows of $C$ is $4$, so the product is defined and the result is $3\times2$.
- $CB$: columns of $C$ is $2$, rows of $B$ is $3$, they differ, so the product is not defined.
- $AC$: columns of $A$ is $3$, rows of $C$ is $4$, they differ, so the product is not defined.
- $CA$: columns of $C$ is $2$, rows of $A$ is $2$, so the product is defined and the result is $4\times3$.
- $AD$: columns of $A$ is $3$, rows of $D$ is $2$, they differ, so the product is not defined.
- $DA$: columns of $D$ is $2$, rows of $A$ is $2$, so the product is defined and the result is $2\times3$.

**Answers:** the products $AB$, $BC$, $CA$, $DA$ are defined, with sizes

$$
AB: 2\times4,\qquad BC: 3\times2,\qquad CA: 4\times3,\qquad DA: 2\times3
$$

The products $BA$, $CB$, $AC$, $AD$ are not defined.

**Remark.** Matrix multiplication is not commutative: $AB$ is defined, but $BA$ is not. The same holds for $AD$ and $DA$.
