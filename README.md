# Robust Neural Networks

This repository contains a collection or robust neural network architectures developed at the Australian Centre For Robotics (ACFR). All networks are implemented in Python/JAX.

Implemented network architectures include:

- Lipschitz-bounded Sandwich MLPs from [Wang & Manchester (ICML 2023)](https://proceedings.mlr.press/v202/wang23v.html). Tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/acfr/RobustNeuralNetworks/blob/main/examples/sandwich_mnist.ipynb)

- Recurrent Equilibrium Network (REN) from [Revay, Wang, & Manchester (TAC 2023)](https://ieeexplore.ieee.org/document/10179161).

- **[WIP]** Monotone, Bi-Lipschitz (BiLipNet), and Polyak-Lojasiewicz networks (PLNet) from [Wang, Dvijotham, & Manchester (ICML 2024)](https://proceedings.mlr.press/v235/wang24p.html).

- Robust Recurrent Deep Network (R2DN) from [Barbara, Wang, & Manchester (arXiv 2025)](https://arxiv.org/abs/2504.01250).

This repository is a work-in-progress. More network architectures, tutorials, and documentation will be added as we go along. 

## Installation for Development

To install the required dependencies, open a terminal in the root directory of this repository and enter the following commands.

```bash
    ./install.sh
```

This will create a Python virtual environment at `./venv` and install all dependencies. If you would rather create a virtual environment with conda, poetry, or something else, feel free to modify the `install.sh` script.

### A Note on Dependencies

All code was tested and developed in Ubuntu 22.04 with CUDA 12.4 and Python 3.10.12. 

Requirements were generated with [`pipreqs`](https://github.com/bndr/pipreqs). The ```install.sh``` will check for whether CUDA is available for your machine, and install the corresponding jax package. 

## Running an Example

Once you have installed the package as above, simply activate the virtual environment and run any of the scripts in the `examples/` folder. For example, from the root directory of the project, run:

```bash
source venv/bin/activate
python examples/sandwich_mnist.py
```

## Contact

Please contact Nicholas Barbara (nicholas.barbara@sydney.edu.au) with any questions.
