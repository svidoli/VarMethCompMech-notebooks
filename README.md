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
| [`ch06_three_bases.ipynb`](ch06_three_bases.ipynb) | 6, Numerical Approximation | Three bases for the same tapered cantilever: monomials (fast, ill-conditioned), cosines $1-\cos(a_k x)$ (well conditioned, slow: no shear at the clamp) and Hermite cubic elements (steady $N^{-2}$, $\kappa \sim N^4$); bending moment and shear force |
| [`appA_condition_number.ipynb`](appA_condition_number.ipynb) | Appendix A, Mathematical Toolbox | Condition number of a linear system: perturbed loads, worst case and round-off; stiffness matrix of a bar and Hilbert matrix |
