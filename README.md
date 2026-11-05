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
| [`ch06_soft_segment.ipynb`](ch06_soft_segment.ipynb) | 6, Numerical Approximation | A cantilever with a soft segment (a jump of the stiffness): vibration modes of the uniform cantilever (well conditioned, $N^{-1/2}$) and Hermite cubic elements ($h^2$ with nodes at the jumps, $N^{-1/2}$ without); curvature and bending moment, exact at the Gauss points; modes of the actual beam computed with finite elements |
| [`ch07_mixed_euler_beam.ipynb`](ch07_mixed_euler_beam.ipynb) | 7, Mixed Variational Principles | The Euler cantilever with Hermite elements and with the second mixed form (linear deflection and bending moment): exact nodal displacements and moments off by $h^2/12$, or exact nodal moments and displacements off by $h^2x^2/24$ |
| [`ch07_timoshenko_locking.ipynb`](ch07_timoshenko_locking.ipynb) | 7, Mixed Variational Principles | Shear locking in a Timoshenko cantilever: linear elements with full integration (too stiff, by the factor $1 + h^2/12\eta$; oscillating shear force), the one-point rule for the shear (the mixed method with constant shear forces) and a quadratic deflection; the dimension of the fields with zero shear energy |
| [`ch08_cylinder_channel.ipynb`](ch08_cylinder_channel.ipynb) | 8, Case Studies | Potential flow past a cylinder in a channel with linear triangles: velocity potential and stream function, two primal problems with exchanged essential and natural conditions; streamlines, pressure on the cylinder, two-sided bounds on the kinetic energy |
| [`ch08_antiplane_crack.ipynb`](ch08_antiplane_crack.ipynb) | 8, Case Studies | Antiplane shear at the tip of a crack in a perfectly plastic material: linear triangles on a polar mesh, alternate minimization (elastic solve with a constant matrix, projection of the stress on the yield disk); the plastic zone against the closed-form solution of Hult and McClintock, the displacement in the plastic fan, convergence of the energy |
| [`appA_condition_number.ipynb`](appA_condition_number.ipynb) | Appendix A, Mathematical Toolbox | Condition number of a linear system: perturbed loads, worst case and round-off; stiffness matrix of a bar and Hilbert matrix |
