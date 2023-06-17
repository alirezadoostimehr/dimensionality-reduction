# Problem statement
Is $\alpha_j$ a Homomorphism?

# Solution
Recall that the Cartesian product of fields $\Pi_{i=1}^n K_i$ is itself a field under the operations of component-wise addition and multiplication. That is, for vectors $(k_1, k_2, \ldots, k_n)$ and $(m_1, m_2, \ldots, m_n)$ in $\Pi_{i=1}^n K_i$, we define

$$(k_1, k_2, \ldots, k_n) + (m_1, m_2, \ldots, m_n) = (k_1+m_1, k_2+m_2, \ldots, k_n+m_n)$$

and

$$(k_1, k_2, \ldots, k_n) \cdot (m_1, m_2, \ldots, m_n) = (k_1m_1, k_2m_2, \ldots, k_nm_n).$$

Under these operations, $\alpha_j$ is indeed a homomorphism. To see why, let $(k_1, k_2, \ldots, k_n)$ and $(m_1, m_2, \ldots, m_n)$ be two vectors in $\Pi_{i=1}^n K_i$. Then we have

$$
\begin{aligned}
\alpha_j((k_1, k_2, \ldots, k_n) + (m_1, m_2, \ldots, m_n)) &= \alpha_j(k_1+m_1, k_2+m_2, \ldots, k_n+m_n) \\
= k_j + m_j \\
= \alpha_j(k_1, k_2, \ldots, k_n) + \alpha_j(m_1, m_2, \ldots, m_n),
\end{aligned}
$$

which shows that $\alpha_j$ preserves addition. Similarly, we have

$$
\begin{aligned}
\alpha_j((k_1, k_2, \ldots, k_n) \cdot (m_1, m_2, \ldots, m_n)) &= \alpha_j(k_1m_1, k_2m_2, \ldots, k_nm_n) \\
= k_jm_j \\
= \alpha_j(k_1, k_2, \ldots, k_n) \cdot \alpha_j(m_1, m_2, \ldots, m_n),
\end{aligned}
$$

which shows that $\alpha_j$ preserves multiplication.

Therefore, $\alpha_j$ is a homomorphism under the operations of component-wise addition and multiplication on $\Pi_{i=1}^n K_i$.
