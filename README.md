# Simulation Software Environment

This repository provides the exact Python software environment used for the
revised stock-direction forecasting simulations. It is supplied as a
reproducibility supplement to the associated manuscript.

## Random seeds

The final neural-network configurations were run with **five random seeds: 0,
1, 2, 3, and 4**. Therefore, the notation “seeds 0–4” refers to five distinct
seed values. A table reporting an individual run should identify its seed; an
aggregate result should be labeled as the mean and sample standard deviation
across all five seeds.

## Software environment

The simulations were run with:

- Python 3.12.14
- TensorFlow CPU 2.21.0
- NumPy 2.5.3
- pandas 3.0.5
- SciPy 1.18.1
- scikit-learn 1.9.1
- Matplotlib 3.11.2

All direct and transitive Python packages are pinned in `requirements.txt`.

## Installation

Create and activate a virtual environment, then install the exact dependencies:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

On macOS or Linux, activate the environment with:

```bash
source .venv/bin/activate
```

## Scope

This repository contains the environment specification and its documentation
only. It intentionally excludes datasets, Reuters-derived news records, trained
model files, and experiment outputs. Those materials should be distributed
separately only when their licenses and the manuscript's data-availability
statement permit redistribution.

## Suggested table note

> Neural-network results were obtained using seeds 0, 1, 2, 3, and 4 and are
> reported as mean ± sample standard deviation unless a specific seed is
> identified. Simulations used Python 3.12.14 and TensorFlow CPU 2.21.0; the
> complete package environment is available in `requirements.txt`.
