# Global-Economic-Indicators-for-Digital-Economy-Benefit-Prediction
This dataset contains country-level global economic indicator records prepared for analyzing the relationship between digital economy development and corporate economic benefits. 
# Hybrid FTS–LSTM Framework for Economic Benefit Prediction

## Overview

This repository contains the implementation of a Hybrid Fuzzy Time Series (FTS) and Long Short-Term Memory (LSTM) framework developed for forecasting economic indicators. The framework combines fuzzy temporal modeling with deep learning to improve prediction accuracy on time-series economic data.

---

## Repository Structure

```
Project/
│
├── Code_Economic.ipynb
├── README.md
├── requirements.txt
│
├── Processed_Output/
│   ├── step1_preprocessed_data.csv
│   ├── step2_feature_selection.csv
│   ├── step3_fuzzy_partition.csv
│   ├── step4_flrg_output.csv
│   ├── step5_fts_forecast_defuzzified_output.csv
│   ├── step6_hybrid_fts_lstm_predictions.csv
│   ├── step6_hybrid_fts_lstm_metrics.csv
│   ├── step6_lstm_training_history.csv
│   └── step6_hybrid_fts_lstm_model.h5
│
└── Dataset/
    └── economic_dataset.csv
```

---

# System Requirements

## Hardware

- Processor: Intel Core i7 or AMD Ryzen 7 (or higher)
- RAM: Minimum 16 GB
- Storage: 10 GB free space
- GPU (Recommended): NVIDIA RTX 3060 or above

---

## Software

- Operating System
  - Windows 10/11
  - Ubuntu 20.04+
  - macOS

- Python
  - Python 3.10 or later

---

# Python Libraries

Install the required packages using:

```bash
pip install -r requirements.txt
```

or

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn scipy openpyxl
```

---

# Dataset

Place the dataset inside the **Dataset** folder.

Example:

```
Dataset/
    economic_dataset.csv
```

---

# Running the Framework

Execute the notebook sequentially.

### Step 1

Data preprocessing

Outputs:

- Cleaned dataset

---

### Step 2

Feature selection

Outputs:

- Selected economic indicators

---

### Step 3

Fuzzy partition generation

Outputs:

- Fuzzy intervals

---

### Step 4

FLRG generation

Outputs:

- Fuzzy logical relationship groups

---

### Step 5

FTS forecasting

Outputs:

```
step5_fts_forecast_defuzzified_output.csv
```

---

### Step 6

Hybrid FTS–LSTM prediction

Outputs:

```
step6_hybrid_fts_lstm_predictions.csv
step6_hybrid_fts_lstm_metrics.csv
step6_lstm_training_history.csv
step6_hybrid_fts_lstm_model.h5
```

---

# Hyperparameters

| Parameter | Value |
|------------|-------|
| Window Size | 5 |
| LSTM Layer 1 | 64 Units |
| LSTM Layer 2 | 32 Units |
| Dropout | 0.20 |
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Epochs | 150 |
| Batch Size | 32 |
| Early Stopping | Patience = 15 |
| Cross Validation | TimeSeriesSplit (5 folds) |
| Random Seeds | 42, 123, 2024 |

---

# Reproducibility

The experiments use:

- Fixed random seeds
- TimeSeriesSplit rolling-window cross-validation
- Box–Cox transformation
- Min-Max normalization
- Portable file paths
- TensorFlow reproducibility settings

---

# Expected Outputs

The repository generates:

- Prediction CSV
- Evaluation metrics
- Training history
- Trained LSTM model

---

# Citation

If you use this implementation in your research, please cite the corresponding manuscript.

---

# Contact

For questions regarding the implementation, please contact the corresponding author.
