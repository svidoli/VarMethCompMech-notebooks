# Variational Methods in Computational Mechanics — companion notebooks

Jupyter notebooks accompanying the book *Variational Methods in Computational Mechanics* by Stefano Vidoli
(Sapienza University of Rome).
The book prints a minimal version of each code; the notebooks here are the full versions, with plots and
parameters to change.

## Running the notebooks

- **In the browser, nothing to install:** scan the QR code printed in the book, or open a notebook on GitHub and
  replace `github.com` with `colab.research.google.com/github` in the address.
- **Locally:** `pip install -r requirements.txt`, then `jupyter lab`.

Each notebook starts with a cell of parameters: change them and run all the cells again.

## Notebooks

| Notebook | Chapter | Subject |
|---|---|---|
| [`ch04_angle_basis.ipynb`](ch04_angle_basis.ipynb) | 4, Function Spaces | Angles between functions: how little a new monomial adds to the previous ones (also sines and clamped-bar polynomials, in the $L^2$, $H^1$ and energy inner products) |
| [`ch04_riesz_bar.ipynb`](ch04_riesz_bar.ipynb) | 4, Function Spaces | Solving a bar with the Riesz theorem: Gram–Schmidt on the monomials in the energy inner product and the truncated series $\sum_i \ell(e_i)\,e_i$; fast convergence for a smooth stiffness, slow for a stiffness that jumps |
| [`ch06_cantilever_modes.ipynb`](ch06_cantilever_modes.ipynb) | 6, Numerical Approximation | The modes of the uniform cantilever as a Galerkin basis: a uniform load (diagonal stiffness matrix, each derivative costs one order of convergence), a smooth variable stiffness (full but almost diagonal matrix) and a concentrated force (slow convergence of the shear, Gibbs oscillations) |
| [`ch06_three_bases.ipynb`](ch06_three_bases.ipynb) | 6, Numerical Approximation | Three bases for a cantilever with a soft segment: monomials (slow and ill-conditioned when the stiffness jumps), vibration modes of the uniform cantilever (well conditioned, $N^{-1/2}$) and Hermite cubic elements, $h^2$ with nodes at the jumps and $N^{-1/2}$ without; curvature and bending moment |
| [`ch08_cylinder_channel.ipynb`](ch08_cylinder_channel.ipynb) | 8, Case Studies | Potential flow past a cylinder in a channel with linear triangles: velocity potential and stream function, two primal problems with exchanged essential and natural conditions; streamlines, pressure on the cylinder, two-sided bounds on the kinetic energy |
| [`appA_condition_number.ipynb`](appA_condition_number.ipynb) | Appendix A, Mathematical Toolbox | Condition number of a linear system: perturbed loads, worst case and round-off; stiffness matrix of a bar and Hilbert matrix |
