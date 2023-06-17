# Problem statement
Find an isomorphism from $B_1$ to $B_2$.

# Solution
To find an isomorphism from $B_1$ to $B_2$, we need to find a linear transformation that maps each basis vector in $B_1$ to a unique basis vector in $B_2$.

Let $B_1={v_1,v_2,\ldots,v_n}$ and $B_2={w_1,w_2,\ldots,w_n}$ be the given bases for $V_1$ and $V_2$, respectively. Since $B_1$ and $B_2$ are assumed to have the same cardinality, we can define a linear transformation $T:B_1\rightarrow B_2$ as follows. For each $i=1,2,\ldots,n$, we define $T(v_i)=w_i$. Since $B_1$ and $B_2$ have the same number of elements, this defines a linear transformation from $B_1$ to $B_2$.

To show that $T$ is an isomorphism, we need to show that $T$ is both injective and surjective. First, we show that $T$ is injective. Suppose $T(v)=T(v')$ for some $v,v'\in B_1$. Then we have $T(v)=w_i$ and $T(v')=w_j$ for some $i,j\in{1,2,\ldots,n}$. Since $T(v)=T(v')$, we have $w_i=w_j$, which implies that $i=j$. Therefore, $v_i=v_j$, and hence $v=v'$. Therefore, $T$ is injective.

Next, we show that $T$ is surjective. Let $w\in B_2$ be an arbitrary basis vector. Then $w=w_i$ for some $i\in{1,2,\ldots,n}$. Since $B_1$ is a basis for $V_1$, there exists a unique linear combination $v=\Sigma_{j=1}^n a_jv_j$ of basis vectors in $B_1$ such that $T(v)=w_i$. Therefore, for any $w\in B_2$, there exists a $v\in B_1$ such that $T(v)=w$, and hence $T$ is surjective.

Since $T$ is both injective and surjective, it is an isomorphism between $B_1$ and $B_2$.
