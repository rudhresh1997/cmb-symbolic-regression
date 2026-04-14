[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19561564.svg)](https://doi.org/10.5281/zenodo.19561564)

# CMB Symbolic Regression

This repository contains the code, synthetic datasets, trained symbolic regression models, baseline Random Forest results, and figures used in the paper:

"Symbolic Regression for Interpretable Cosmological Parameter Inference from the CMB"

## Contents
- `cmb_pysr_final.ipynb`: main analysis notebook
- `cmb_sampled_parameters.csv`: sampled cosmological parameters
- `cmb_spectra_data.npz`: synthetic CMB spectra
- `pysr_*.pkl`: trained symbolic regression models
- `rf_baseline_results.csv`: Random Forest baseline results
- `final_symbolic_regression_summary.csv`: summary results
- `figures/`: figures used in the paper

## Reproducibility
Run `cmb_pysr_final.ipynb` to regenerate the analysis products.

## Main dependencies
- Python
- CAMB
- PySR
- NumPy
- pandas
- scikit-learn