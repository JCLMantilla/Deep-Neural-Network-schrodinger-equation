
## ATTENTION! THIS PROJECT IS UNDER MAINTENANCE! These are the changes I am working on:
  - Add documentation
  - Organize physics-related code in different scripts
  - Change the autoencoder into TensorFlow Functional API
  - Change the simulation data generation into a Python generator and use it to feed the data into the autoencoder model for training

# Schrodinger-equation-DNN
In this project, I am going to display the power of Deep Neural Networks (in this case an autoencoder) to solve the 1D time-independent Schrödinger equation.

If a particle is subject to a known potential $\boldsymbol{V}(x)$, we need to find the find it's wave function $\boldsymbol{\psi}(\boldsymbol{x})$ that satisfies the following relation:

$$ \frac{-\hbar^2}{2m} \frac{\partial ^2 }{\partial x^2}\psi (x) +\boldsymbol{V}(x)\psi(x) = \boldsymbol{E} \psi(x)$$


We are going to create syntetic pontentials of the type $\boldsymbol{V}(x) = \boldsymbol{\Sigma}_i \boldsymbol{\alpha}_i x^i$ and we will use their analytical solution to train an autoecoder that will essentially learn a non-linear map between the potential  $\boldsymbol{V}(x)$ of a particle and the associated wave function $\boldsymbol{\psi}(x)$ of a particle.

We will use the trained network to solve the Schödinger equation for the 1-Dimensional quantum harmonic oscillator and we will compare it using the analytical solution:

$$\psi_n(x) = \left(\frac{1}{\sqrt{2^n n!}}\right) \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

## References
Computational Physics: Problem-Solving with Computers, Rubin H. Landau et al. 
https://books.google.fr/books/about/Computational_Physics.html?id=RBg-vgAACAAJ&redir_esc=y
