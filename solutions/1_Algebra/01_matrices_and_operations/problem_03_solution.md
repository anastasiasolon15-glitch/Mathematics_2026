# Matrices and Basic Operations — Exercise 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

Rule: the product $XY$ with $X$ of size $m\times n$ and $Y$ of size $p\times q$ is defined if and only if $n=p$ (inner dimensions agree). The result has size $m\times q$.

| Product | Sizes | Inner dimensions | Defined? | Result size |
|---|---|---|---|---|
| $AB$ | $2\times3$ and $3\times4$ | $3=3$ | Yes | $2\times4$ |
| $BA$ | $3\times4$ and $2\times3$ | $4\ne2$ | No | — |
| $BC$ | $3\times4$ and $4\times2$ | $4=4$ | Yes | $3\times2$ |
| $CB$ | $4\times2$ and $3\times4$ | $2\ne3$ | No | — |
| $AC$ | $2\times3$ and $4\times2$ | $3\ne4$ | No | — |
| $CA$ | $4\times2$ and $2\times3$ | $2=2$ | Yes | $4\times3$ |
| $AD$ | $2\times3$ and $2\times2$ | $3\ne2$ | No | — |
| $DA$ | $2\times2$ and $2\times3$ | $2=2$ | Yes | $2\times3$ |

## Explanation

Each entry of $XY$ is a row of $X$ multiplied by a column of $Y$, so the row length (the number of columns of $X$) must equal the column length (the number of rows of $Y$). Four of the eight products are defined: $AB$, $BC$, $CA$, $DA$. In several cases one order works and the reverse does not (for example $AB$ is defined but $BA$ is not), which already shows that matrix multiplication is not commutative.
