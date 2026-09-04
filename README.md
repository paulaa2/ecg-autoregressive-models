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

```
APRNS-Lab-8/
├── notebooks/                                  # Definite & clean notebooks
│   ├── ecg_autoregressive_models.ipynb         # [DEFINITIVE] Complete 200-epoch training, 6-config grid search & anomaly detection
│   ├── ecg_baseline_100epochs.ipynb            # Baseline 100-epoch training run
│   └── lab_reference_template.ipynb            # Original course reference material
├── archive/                                    # Obsolete / non-definitive drafts
│   ├── troubleshooting_draft.ipynb             # Incomplete draft with troubleshooting notes
│   ├── experiment_draft.ipynb                  # Secondary experiment notebook
│   ├── scratch_aaaaaaa.ipynb                   # Scratch run
│   └── scratch_aaaaaaachus.ipynb               # Scratch run
├── README.md                                   # Project documentation
└── .gitignore                                  # Git configuration
```

## How to Run

Open `notebooks/ecg_autoregressive_models.ipynb` in Jupyter/Colab and run cells sequentially. GPU recommended for training.

## Author

Paula Esteve Sabater

## Context

Course project — APRNS (Pattern Recognition and Neural Systems), UPC.
