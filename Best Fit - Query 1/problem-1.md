# Problem statement

Show that the line $C$ is a subspace of $V$ containing $D'$.

*Hypotheses:* $C$ *is an arbitrary line which is defined as* $C = \alpha x$ *and* $D'$ *is a dataset which is centered at the origin* $O(0, 0)$. *And V is a finite dimensional space over field K*

# Solution

To show that the line $C$ is a subspace of $V$ containing $D'$, we need to verify the two conditions for subspaces:

1. Closure under vector addition: Let $x, y \in C$ and $k, l \in K$ be scalars. Then, $x = \alpha k x'$ and $y = \alpha l y'$ for some fixed vector $x', y' \in V$. We have:

   $x + y = \alpha k x' + \alpha l y' = \alpha (k x' + l y')$
   
   Since $k x' + l y' \in V$, we have shown that $x + y \in C$.
   
2. Closure under scalar multiplication: Let $x \in C$ and $k \in K$ be a scalar. Then, $x = \alpha k x'$ for some fixed vector $x' \in V$. We have:

   $k x = k (\alpha k x') = \alpha (k^2 x')$
   
   Since $k^2 \in K$ and $x' \in V$, we have shown that $k x \in C$.

Therefore, we have shown that $C$ is a subspace of $V$ containing $D'$, since any vector in $D'$ can be expressed as a scalar multiple of $x$, which is in $C$.
