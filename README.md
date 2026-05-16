# CMB Symbolic Regression

This repository contains the code, synthetic datasets, trained symbolic-regression models, baseline-model results, robustness diagnostics, uncertainty analyses, and figures used in the paper:

**Interpretable symbolic regression for cosmological parameter recovery from CMB power spectra**

## Overview

This project investigates symbolic regression as an interpretable framework for recovering cosmological parameters from synthetic cosmic microwave background (CMB) power spectra. Synthetic \(TT\), \(TE\), and \(EE\) spectra are generated using CAMB across a five-parameter \(\Lambda\)CDM-inspired parameter space. Symbolic regression models are trained to recover:

- \(n_s\)
- \(\ln(10^{10}A_s)\)
- \(\omega_b\)
- \(\omega_{\rm cdm}\)
- \(\tau\)

The repository also includes robustness tests, bootstrap uncertainty estimates, calibration diagnostics, feature/operator ablations, baseline comparisons, and physics-informed feature engineering for \(\omega_b\).

## Main files

- `cmb_pysr_final.ipynb`  
  Original main analysis notebook.

- `cmb_pysr_final-AC.ipynb`  
  Updated Astronomy and Computing submission notebook. This includes the final analyses used in the manuscript, including bootstrap uncertainty, calibration diagnostics, noise robustness, cross-validation, feature ablations, operator ablations, perturbation-based interpretability tests, complexity-frontier diagnostics, and final manuscript figures.

- `cmb_sampled_parameters.csv`  
  Sampled cosmological parameters.

- `cmb_spectra_data.npz`  
  Synthetic CAMB-generated CMB spectra.

- `final_symbolic_regression_summary.csv`  
  Summary of symbolic-regression model performance.

- `rf_baseline_results.csv`  
  Random Forest baseline results.

## Directories

- `figures/`  
  Original figures generated during the analysis.

- `figures_AC/`  
  Final figures used for the Astronomy and Computing manuscript.

- `models/`  
  Trained symbolic-regression models, bootstrap models, robustness models, and ablation models.

- `outputs/`  
  Analysis outputs generated during notebook execution.

- `results/`  
  CSV/NPZ summaries for bootstrap uncertainty, calibration, robustness, ablations, baselines, perturbation tests, and complexity-frontier diagnostics.

## Reproducibility

To reproduce the final manuscript results, run:

```bash
jupyter notebook cmb_pysr_final-AC.ipynb