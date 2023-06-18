# Problem statement

Project all points on the line $C$ using projective transformation mentioned in previous section.

*Hypotheses:* $C$ *is an arbitrary line which is defined as* $C = \alpha x$ *and* $D'$ *is a dataset which is centered at the origin* $O(0, 0)$. *And V is a finite dimensional space over field K. And we know that* $C$ *is a subspace of* $V$ *containing* $D'$.

# Solution

We know $C$ is the line defined as $C =$ { $\alpha * X | \alpha \in K$ }, where $\alpha$ is a fixed scalar in $K$ and $X$ is a nonzero vector in $V$. Let $P$ be the projection defined on the space $V$ to the line $C$ using the projective transformation $\alpha_j (k_1, k_2, ..., k_n) = k_j$.

To project a point $(v_1, v_2, ..., v_n)$ in $V$ onto the line $C$, we can compute the coordinates of the projected point as 

$$P((v_1, v_2, ..., v_n)) = ((\alpha * \alpha_1((v_1, v_2, ..., v_n))), (\alpha * \alpha_2(v_1, v_2, ..., v_n)), ..., \alpha * \alpha_n(v_1, v_2, ..., v_n))$$

using projective transformation mentioned in previous section.
