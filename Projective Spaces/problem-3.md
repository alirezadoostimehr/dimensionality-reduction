# Problem statement
Find $ker(\alpha_j)$.

# Solution
Recall that $\alpha_j: \Pi_{i=1}^n K_i \rightarrow K_j$ is the linear transformation defined by $\alpha_j(k_1, k_2, \ldots, k_n) = k_j$ for each $j = 1, 2, \ldots, n$. To find the kernel of $\alpha_j$, we need to find the set of all vectors in $\Pi_{i=1}^n K_i$ that are mapped to zero by $\alpha_j$.

Suppose $(k_1, k_2, \ldots, k_n)$ is a vector in $\Pi_{i=1}^n K_i$ that is mapped to zero by $\alpha_j$. Then we have $\alpha_j(k_1, k_2, \ldots, k_n) = k_j = 0$. Since $K_j$ is a field, this implies that $k_j = 0$ for all $j \neq i$, while $k_i$ can be any element of $K_i$. Therefore, the kernel of $\alpha_j$ consists of all vectors of the form

$$(k_1, k_2, \ldots, k_{j-1}, 0, k_{j+1}, \ldots, k_n)$$

where $k_i$ can be any element of $K_i$. In other words, the kernel of $\alpha_j$ is the set of all vectors in $\Pi_{i=1}^n K_i$ that have a zero in the $j$-th component and arbitrary elements in all other components.
