# Problem statement
Show that $\Pi_{i=1}^n K_i$ is also a field where $\Pi_{i} K_i$ is the Cartesian product of $K_i$ s.

*Hypotheses: Let* $K_1, K_2, \ldots, K_n$ *be n different fields.*

# Solution
Let $K_1, K_2, \ldots, K_n$ be $n$ different fields. We want to show that the Cartesian product $\Pi_{i=1}^{n} K_i$ is also a field.

To show that $K$ is a field, we need to show that it satisfies the following properties:

1. $K$ is a commutative ring with unity.

2. Every nonzero element of $K$ has a multiplicative inverse.

Property 1 follows immediately from the fact that each $K_i$ is a field, since the Cartesian product of rings is also a ring. That is, $K$ is a commutative ring with unity, where the addition and multiplication operations are defined component-wise.

To prove Property 2, let $(a_1, a_2, \ldots, a_n)$ be any nonzero element of $K$. Then there exists some $i$ such that $a_i \neq 0$, since otherwise $(a_1, a_2, \ldots, a_n) = (0, 0, \ldots, 0)$, which is the zero element of $K$. Let $b_i$ be the multiplicative inverse of $a_i$ in $K_i$. That is, $b_i$ satisfies $a_i b_i = 1_{K_i}$, where $1_{K_i}$ is the multiplicative identity element in $K_i$.

Now define an element $(b_1, b_2, \ldots, b_n)$ of $K$ as follows:

$$
b_j =
\begin{cases}
b_i & \text{if } j = i \\
0 & \text{if } j \neq i
\end{cases}
$$

Then we have

$$(a_1, a_2, \ldots, a_n) \cdot (b_1, b_2, \ldots, b_n) = (a_1b_1, a_2b_2, \ldots, a_nb_n) = (0,0,\ldots,0,1_{K_i},0,\ldots,0),$$

where $1_{K_i}$ is in the $i$-th component. Therefore, $(b_1, b_2, \ldots, b_n)$ is a multiplicative inverse of $(a_1, a_2, \ldots, a_n)$ in $K$.

Hence, we have shown that every nonzero element of $K$ has a multiplicative inverse, and therefore $K$ is a field.
