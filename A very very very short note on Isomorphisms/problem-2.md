# Problem statement
Find an isomorphism $\alpha : V \rightarrow K^n$ where $\ker(\alpha) = \ ${0}

*Hypotheses: V is a finite dimensional space over the field K.*

# Proof: 

We can construct an isomorphism $\alpha: V \rightarrow K^n$ as follows:

Let ${v_1,v_2,\ldots,v_n}$ be a basis for $V$. Since $V$ is finite-dimensional, we can assume that $n$ is finite. Define $\alpha: V \rightarrow K^n$ by

$$\alpha(a_1v_1 + a_2v_2 + \ldots + a_nv_n) = \begin{pmatrix}a_1 \ a_2 \ \cdots \ a_n\end{pmatrix}$$

for any $a_1,a_2,\ldots,a_n \in K$.

It can be shown that $\alpha$ is a linear transformation, and that it is injective. To see why $\alpha$ is injective, suppose that $\alpha(v) = \mathbf{0}$, where $\mathbf{0}$ is the zero vector in $K^n$. Then

$$\alpha(v) = \begin{pmatrix}0 \ 0 \ \cdots \ 0\end{pmatrix}$$

implies that $a_1v_1 + a_2v_2 + \ldots + a_nv_n = 0$, where $a_1,a_2,\ldots,a_n \in K$. But since ${v_1,v_2,\ldots,v_n}$ is a basis for $V$, this implies that $a_1 = a_2 = \ldots = a_n = 0$, so $v = 0$. Thus, $\ker(\alpha) = ${0}.

To see that $\alpha$ is surjective, let $\mathbf{b} = (b_1 \ b_2 \ \cdots \ b_n )$ be any vector in $K^n$. Define $v = b_1v_1 + b_2v_2 + \ldots + b_nv_n$. Then

$$\alpha(v) = \begin{pmatrix}b_1 \ b_2 \ \cdots \ b_n\end{pmatrix} = \mathbf{b}$$

which shows that $\alpha$ is surjective.

Thus, we have constructed an isomorphism $\alpha: V \rightarrow K^n$ such that $\ker(\alpha) = ${0}.
