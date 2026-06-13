# RCT_Bench — A Public Benchmark of Real-World RCT Datasets for Covariate Adjustment Research

This repository provides a curated, analysis-ready benchmark of **real-world randomized controlled trial (RCT) datasets**, together with the R pipelines used to clean and analyze them. It accompanies the study **"How should covariates be handled in randomized trials? Empirical evidence from 50 trials and recommendations for practice"** (Yulin Shao, Liangbo Lyu, Menggang Yu, Bingkai Wang — Department of Biostatistics, University of Michigan).

The goal of this repo is to give methodologists, trialists, and statisticians a **ready-to-use, standardized benchmark** for evaluating covariate-adjustment methods, variable-selection strategies, and other estimation procedures on real (not simulated) trial data — without having to track down, clean, and harmonize dozens of individual trial datasets.

## What's Included

- **Cleaned individually-randomized (non-clustered) RCT datasets** — standardized, analysis-ready data from publicly available trials, with harmonized variable naming so datasets can be processed interchangeably
- **`meta_data.xlsx`** — trial-level metadata (trial name, publication, journal, sample size, primary outcome and type, study phase, randomization scheme, research area, citation, etc.) for each trial in the benchmark
- **`meta_data_demo.xlsx`** — per-trial participant demographic breakdowns (sex and race/ethnicity counts, e.g., Male/Female/Other and Asian/Black/White/Hispanic/etc., by trial)
- **`meta_data_comparison.xlsx`** — the full method-comparison results table: for every trial/treatment-outcome comparison and covariate-selection strategy (All / Top-3 / Baseline+), the point estimates, standard errors, p-values, and precision-gain metrics for each estimator (Unadjusted, ANCOVA, ANHECOVA, IPW, g-logistic, DML, TMLE, AIPW, SuperLearner-based, PSWeight-based, etc.)
- **`RCT_data_cleaning.Rmd`** — the unified data-cleaning pipeline that transforms raw trial data into the standardized format provided here (included for transparency and so users can apply the same conventions to their own datasets)
- **`RCT_analysis.Rmd`** — an end-to-end analysis pipeline demonstrating how to apply and compare covariate-adjustment estimators (e.g., ANCOVA, ANHECOVA, IPW, g-computation, machine-learning-based estimators such as DML and TMLE) across multiple covariate-selection strategies on these datasets

> Note: This public release includes only the **non-clustered (individually randomized)** trial datasets. Clustered-RCT data and other supplementary materials from the original study are not part of this benchmark.

## Variable Naming Convention

All cleaned datasets follow a common schema so they can be looped over programmatically:

- `YP_*` — primary outcome(s)
- `YS_*` — secondary outcome(s)
- `X_*` — baseline covariates
- `Treatment` — treatment assignment

## Repository Structure

```text
RCT_Data/
├── cleaned_data/
│   ├── Non_Clustered_RCT/        # Standardized, analysis-ready datasets (one per trial)
│   ├── meta_data.xlsx            # Trial-level metadata (publication, sample size, outcomes, etc.)
│   ├── meta_data_demo.xlsx       # Per-trial participant demographics (sex, race/ethnicity)
│   └── meta_data_comparison.xlsx # Full estimator-comparison results (estimates, SEs, p-values, precision gains)
├── RCT_data_cleaning.Rmd         # Pipeline used to produce the cleaned datasets
└── RCT_analysis.Rmd              # Example pipeline: apply & compare adjustment methods
```