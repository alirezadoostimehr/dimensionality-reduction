# Problem statement
Find kernel(T).

*We defined T in previous problem. For checking it click [here](https://github.com/alirezadoostimehr/dimensionality-reduction/blob/main/Recenter%20Data/problem-3.md).*

# Solution

To begin, let's establish the definition of the kernel of a homomorphism.
$ker(T) =$ \{ $x \in \text{Domain}(T) \mid T(x) = \text{identity element in Codomain}(T)$ \}

In this scenario, where the identity element is the zero vector and the zero vector in the codomain is represented as $O(0, 0)$, our objective is to identify all vectors $x$ in $V$ that satisfy the condition $T(x) = O(0, 0)$.

So the equation is
$$x - \bar{X}n = O(0, 0)$$
Simplifying the equation further, we find:
$$x = \bar{X}n$$
Consequently, the kernel of $T$, denoted as $ker(T)$, comprises solely the vector $\bar{X}n$.

