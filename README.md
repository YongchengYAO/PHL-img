# Topological Data Analysis with Persistent Hodge Laplacian for Images

![HodgeDecomposition](README.assets/HodgeDecomposition.png)

# De Rham-Hodge Theory

## Hodge Laplacian

Hodge Laplacian is defined as a mapping
$$
\Delta^k \equiv d^{k-1}\delta^k + \delta^{k+1} d^k \;:\; \Omega^k(M) \to \Omega^k(M)
$$
We call a differential $k$-form is a harmonic form if $\omega^k\in\text{ker}\;\Delta^k$. We denote the complete space of harmonic $k$-forms by
$$
\mathcal{H}^k_\Delta \equiv \text{ker}\; \Delta^k.
$$
Due to 
$$
\langle d\omega, \omega \rangle_{L^2}=\langle \omega, \delta\omega \rangle_{L^2}
$$

we have

$$
\langle \Delta\omega, \omega\rangle_{L^2} = \langle (d\delta+\delta d)\omega, \omega\rangle_{L^2} = \langle d\delta\omega, \omega\rangle_{L^2} + \langle \delta d\omega, \omega\rangle_{L^2} = \langle \delta\omega, \delta\omega \rangle_{L^2} + \langle d\omega, d\omega \rangle_{L^2},
$$
We know that if a non-trivial differential $k$-form $\omega^k \in \text{ker}\;d^k \cap \text{ker}\;\delta^k$ (i.e., $\omega^k$ is closed and coclosed), then $\langle \Delta\omega^k, \omega^k\rangle_{L^2}=0$ due to $\delta\omega^k=0$ and $d\omega^k=0$. Since $\omega^k\neq \bf{0}$, we have proved that $\Delta\omega^k=\bf{0}$, i.e. $\omega^k\in\mathcal{H}^k_\Delta$. We denote the special space of harmonic $k$-form by
$$
\mathcal{H}^k_{\text{cc}} \equiv \text{ker}\;d^k \cap \text{ker}\;\delta^k,
$$
where $\text{cc}$ stands for "closed and coclosed". Note that all closed and co-closed forms are harmonic, but the converse is not necessarily true, that is 
$$
\mathcal{H}^k_{\text{cc}} \subseteq \mathcal{H}^k_\Delta.
$$

On a closed Riemannian manifold, the complete space of harmonic forms $\mathcal{H}^k_\Delta$ reduces to the special space of harmonic forms $\mathcal{H}^k_{\text{cc}}$ due to the adjointness of $d$ and $\delta$.

## Hodge Decomposition on Closed Manifolds

Due to the important property of adjoint operators, that the kernel of one operator is the orthogonal complement of the image of its adjoint operator, and the adjointness of $d$ and $\delta$ on a closed Riemannian manifold, the space of differential $k$-forms can be decomposed into 

$$
\Omega^k(M)=\text{ker}\;d^{k} \oplus \text{im}\;\delta^{k+1},
$$
or

$$
\Omega^k(M)=\text{im}\;d^{k-1} \oplus \text{ker}\;\delta^{k}.
$$

With $\text{im}\;\delta^{k+1} \subset \text{ker}\;\delta^k$ (due to $\delta\delta=0$) and \cref{eq:2componentsDecomp-v1}, we have
$$
\Omega^k(M) \cap \text{ker}\;\delta^k = \text{ker}\;d^{k} \cap \text{ker}\;\delta^k \oplus \text{im}\;\delta^{k+1} \cap \text{ker}\;\delta^k, \\
\text{ker}\;\delta^k = \text{ker}\;d^{k} \cap \text{ker}\;\delta^k \oplus \text{im}\;\delta^{k+1}, \\
\text{ker}\;\delta^k = \mathcal{H}^k_{\text{cc}} \oplus \text{im}\;\delta^{k+1},
$$

and 
$$
\Omega^k(M)= \text{im}\;\delta^{k+1} \oplus \text{im}\;d^{k-1} \oplus \mathcal{H}^k_{\text{cc}} .
$$

With $\mathcal{H}^k_{\text{cc}}=\mathcal{H}^k_\Delta$ on closed manifolds, the Hodge decomposition becomes
$$
\Omega^k(M)= \text{im}\;\delta^{k+1} \oplus \text{im}\;d^{k-1} \oplus \mathcal{H}^k_\Delta .
$$

Note that a differential $k$-form $\omega^k$ is exact if $\omega^k\in\text{im}\;d^{k-1}$, and is coexact if $\omega^k\in\text{im}\;\delta^{k+1}$. The Hodge decomposition indicates that any differential $k$-form can be decomposed into the sum of an exact form, an coexact form, and a harmonic form:
$$
\omega = \delta\alpha + d\beta + \gamma,\quad \alpha\in\text{im}\;\delta,\;\beta\in\text{im}\;d,\;\gamma\in\mathcal{H}^k_\Delta
$$

