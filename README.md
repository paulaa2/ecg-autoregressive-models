# ECG Autoregressive Generative Models

Autoregressive generative models for synthetic ECG signal generation, trained on the MIT-BIH Arrhythmia Database.

## Overview

Lab assignment for the APRNS course exploring autoregressive architectures for time-series generation. The pipeline loads normal ECG signals, discretizes and windows them, trains generative models, and evaluates synthetic samples against real data using statistical metrics.

## Approach

1. Load ECG signals from MIT-BIH via `apafib`
2. Preprocess: discretization, windowing, train/validation split
3. Train autoregressive models using `pytorch_generative`
4. Generate synthetic ECG samples
5. Compare generated vs. real signals (distribution metrics, visual inspection)

## Tech Stack

- Python 3
- PyTorch, `pytorch_generative`
- `apafib` (MIT-BIH loader)
- NumPy, SciPy, Matplotlib, Seaborn, scikit-learn

## Key Notebooks

| Notebook | Description |
|----------|-------------|
| `01-ModelosAutoregresivos-colab_original.ipynb` | Course reference material |
| `ejercicio_entregable.ipynb` | Main submission notebook |
| `final.ipynb` | Final trained model and evaluation |

## How to Run

Open `ejercicio_entregable.ipynb` or `final.ipynb` in Jupyter and run cells sequentially. GPU recommended for training.

## Author

Paula Esteve Sabater

## Context

Course project — APRNS (Pattern Recognition and Neural Systems), UPC.
