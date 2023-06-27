# Schrodinger-equation-DNN

In this project, I am going to display the power of Deep Neural Networks (in this case an autoencoder) to solve the 1D time-independent Schrödinger equation for potentials of the type $\boldsymbol{V}(x) = \boldsymbol{\Sigma}_i \boldsymbol{\alpha}_i x^i$. The network will essentially learn a non-linear map between the potential of a particle and the associated wave function of a particle.

If a particle is subject to a known potential $\mathbb{V}(\boldsymbol{x})$, we need to find the find it's wave function $\boldsymbol{\psi}(\boldsymbol{x})$ that satisfies the following relation:
$$-\frac{\boldsymbol{\Sigma}_m(\boldsymbol{x})}{2}\boldsymbol{\Delta\psi}(\boldsymbol{x})+\mathbb{V}(\boldsymbol{x})\boldsymbol{\psi}(\boldsymbol{x})=\mathbb{E}\boldsymbol{\psi}(\boldsymbol{x})$$



## References
Computational Physics: Problem-Solving with Computers, Rubin H. Landau et al. 
https://books.google.fr/books/about/Computational_Physics.html?id=RBg-vgAACAAJ&redir_esc=y
>>>>>>> 6a1e441fc467e2f2ed1d127e1a1f0f7296f9ca14
