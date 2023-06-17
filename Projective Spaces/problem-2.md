# Problem statement
Let $(k_1, k_2, ..., k_n)$ be a vector in $\Pi_{i}^n K_i$. Define $\alpha_j$ : $\Pi_{i}^n K_i → Kj$ where $\alpha_j(k_1, k_2, ..., k_n) = k_j$.

Show that $\alpha_j$ is an isomorphism.

*Hypotheses: Let* $K_1, K_2, \ldots, K_n$ *be n different fields.*

# Solution
Let $(k_1, k_2, \ldots, k_n)$ be a vector in $\Pi_{i=1}^n K_i$. We define $\alpha_j: \Pi_{i=1}^n K_i \rightarrow K_j$ by $\alpha_j(k_1, k_2, \ldots, k_n) = k_j$ for each $j = 1, 2, \ldots, n$.

To see that $\alpha_j$ is a linear transformation, we need to show that it satisfies the following two properties:

$\alpha_j(u + v) = \alpha_j(u) + \alpha_j(v)$ for any vectors $u$ and $v$ in $\Pi_{i=1}^n K_i$.

$\alpha_j(cu) = c \alpha_j(u)$ for any vector $u$ in $\Pi_{i=1}^n K_i$ and any scalar $c$ in $K_j$.

For Property 1, let $u = (u_1, u_2, \ldots, u_n)$ and $v = (v_1, v_2, \ldots, v_n)$ be two vectors in $\Pi_{i=1}^n K_i$. Then we have

$$
\alpha_j(u + v) = \alpha_j(u_1 + v_1, u_2 + v_2, \ldots, u_n + v_n) = u_j + v_j = \alpha_j(u) + \alpha_j(v),
$$

so Property 1 holds.

For Property 2, let $u = (u_1, u_2, \ldots, u_n)$ be a vector in $\Pi_{i=1}^n K_i$ and let $c$ be any scalar in $K_j$. Then we have

$$
\alpha_j(cu) = \alpha_j(cu_1, cu_2, \ldots, cu_n) = c u_j = c \alpha_j(u),
$$

so Property 2 holds.

Therefore, we have shown that $\alpha_j$ is a linear transformation for each $j = 1, 2, \ldots, n$.
