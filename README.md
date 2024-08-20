# Topological Data Analysis with Persistent Hodge Laplacian for Images

![HodgeDecomposition](README.assets/HodgeDecomposition.png)

# De Rham-Hodge Theory

## Hodge Decomposition on Closed Manifolds

On a closed manifold $M$, the space of differential $k$-form $\Omega^k(M)$ can be decomposed into 
$$
\Omega^k(M)= \text{im}\;\delta^{k+1} \oplus \text{im}\;d^{k-1} \oplus \mathcal{H}^k_{\text{cc}},
$$
where $\mathcal{H}^k_{\text{cc}}\equiv\text{ker}\;d^k\cap\text{ker}\;\delta^k$. 

On a closed manifold,
$$
\mathcal{H}^k_{\text{cc}}=\mathcal{H}^k_\Delta \\
\mathcal{H}^k_\Delta \equiv \text{ker}\;\Delta^k = \{\omega^k\in\Omega^k(M)\mid\Delta^k\omega^k=0\}
$$
Therefore, the 3-component Hodge decomposition on a closed manifold becomes
$$
\Omega^k(M)= \text{im}\;\delta^{k+1} \oplus \text{im}\;d^{k-1} \oplus \mathcal{H}^k_\Delta.
$$
