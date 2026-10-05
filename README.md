# AI651 PA1: Deep Learning for Spatio-Temporal Graphs

Syed Obaidullah Hassan Chishti (25280049)

Code for Programming Assignment 1. The report (PDF and LaTeX source) is submitted separately on LMS.

## Repository layout

```
Question 1/                          Task 1: forecasting across heterogeneous sensors
  Assignment1.ipynb                  implementation notebook, executed with PA1_PRESET=full
  harness/                           supplied data, model, control and reporting code
  results/design/                    Outputs 1.1-4.3 (CSV, LaTeX tables, PDF figures)
  requirements.txt

Question 2 - Leaderboard/            Task 2: Autoformer leaderboard
  25280049_Task2_Autoformer.ipynb    final notebook (validation, ablations, refit, forecast)
  task2_predictions_single.csv       168-step forecast for time_idx 43657-43824
  Data/                              student_train.csv, student_test.csv, optional_external_data.csv
  experiments/                       earlier development notebooks (baseline, 3-seed ensemble, target-only)
```

## Setup

```bash
conda create -n dl4stg_env python=3.11
conda activate dl4stg_env
pip install -r "Question 1/requirements.txt"
```

Task 2 uses the same packages (numpy, pandas, matplotlib, torch).

## Task 1

Open `Question 1/Assignment1.ipynb`, set `PA1_PRESET = "full"`, and run all cells. Tables and figures go to `Question 1/results/design/`. All numbers in the report come from the full preset.

## Task 2

Run `Question 2 - Leaderboard/25280049_Task2_Autoformer.ipynb` from top to bottom. It runs on a CPU, but a GPU is faster.

