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
| [`ch04_angle_basis.ipynb`](ch04_angle_basis.ipynb) | 4, Function Spaces | Angles between functions; Gram matrices of monomials, sines and clamped-bar polynomials; conditioning; best approximation with nearly parallel and with orthonormal bases |
| [`appA_condition_number.ipynb`](appA_condition_number.ipynb) | Appendix A, Mathematical Toolbox | Condition number of a linear system: perturbed loads, worst case and round-off; stiffness matrix of a bar and Hilbert matrix |
