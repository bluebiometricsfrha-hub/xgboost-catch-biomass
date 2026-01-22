# XGBoost Biomass Model

This repository provides the code used to develop and evaluate an XGBoost-based model for biomass estimation, including data preprocessing, model training, and validation workflows.

This code accompanies the associated peer-reviewed publication. If you use this code, please cite the corresponding paper.
Cite: `Article is under preparation.`

---

# Physics-Informed XGBoost Analysis for Mesopelagic Fisheries

## Description

This repository contains two Jupyter notebooks implementing physics-informed XGBoost regression models to predict mesopelagic fisheries indicators using oceanographic and biogeochemical variables. The analysis is conducted separately for two ecological groups and two regions of the Arabian Sea.

The notebooks include feature engineering, model training, evaluation, and sensitivity analysis.

---

## Notebooks

* `2_myct_clean_analysis_XGBoost_targetwise_areawise_with_Sensitivity.ipynb`
  XGBoost modeling and sensitivity analysis for **myctophids (MYCT)**

* `2_nekt_clean_analysis_XGBoost_targetwise_areawise_with_Sensitivity.ipynb`
  XGBoost modeling and sensitivity analysis for **nekton (NEKT)**

Each notebook performs the analysis independently for:

* NEAS: Northeastern Arabian Sea
* SEAS: Southeastern Arabian Sea

---

## Method Summary

* Physics-informed feature engineering from vertical structure, OMZ, thermocline, and productivity variables
* XGBoost regression with cross-validated hyperparameter tuning
* Performance metrics: RMSE, R², Nash–Sutcliffe Efficiency
* Sensitivity analysis using:

  * Permutation importance (global)
  * ICE and partial dependence plots (local)

---

## Outputs

* Trained models and preprocessing objects (`.pkl`)
* Feature importance tables
* Sensitivity analysis results (CSV)
* ICE and PDP plots (PNG)

All outputs are saved under:

```
saved_models/
```

---

## Requirements

* Python ≥ 3.9
* pandas
* numpy
* scikit-learn
* xgboost
* matplotlib
* joblib

---

## Usage

Open the required notebook and run all cells in order.
Input CSV files must be present in the working directory.
No command-line execution is required.

---

