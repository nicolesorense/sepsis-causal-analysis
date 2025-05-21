# Causal Discovery and Inference on ICU Transfers and Sepsis

This repository contains code for a causal inference analysis to evaluate the effect of inter-unit ICU transfers on sepsis occurrence using the MIMIC-IV dataset.

## Project Overview
This project uses causal discovery (PC and FCI algorithms) and causal inference techniques (propensity score matching, IPTW, and doubly robust estimation) to analyze the relationship between ICU transfers and sepsis onset, accounting for confounders like Glasgow Coma Scale (GCS), creatinine levels, and comorbidities.

## Prerequisites
- Python 3.8+
- Required packages (install via `pip install -r requirements.txt`):
  - pandas
  - numpy
  - matplotlib
  - causallearn
  - scikit-learn
  - google-cloud-bigquery
  - statsmodels
  - scipy
  - tqdm
  - seaborn

## Data
The analysis uses the [MIMIC-IV dataset](https://physionet.org/content/mimiciv/2.2/). Access requires credentials from PhysioNet. Place the dataset files in a `data/` folder or configure access to Google Cloud BigQuery.

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/nicolesorense/sepsis-causal-analysis.git
   cd sepsis-causal-analysis
   ```
