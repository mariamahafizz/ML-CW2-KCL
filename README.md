# ML Coursework 2 – TypiClust (TPC_RP) on CIFAR-10

**Student:** Mariam Hafiz (K23115695)  
**Module:** Machine Learning, King's College London  
**Paper:** Hacohen et al. (2022) "Active Learning on a Budget: Opposite Strategies Suit High and Low Budgets"

## Overview
Implementation of the TPC_RP active learning algorithm on CIFAR-10, including a proposed modification (Gaussian-weighted adaptive typicality).

## Contents
- `typiclust-cifar10-fixed.ipynb` – Full implementation notebook (SimCLR training, TypiClust, baselines, modification, evaluation)

## How to Run
1. Open the notebook in Kaggle with GPU T4 enabled
2. Upload `simclr_latest.pt` as a dataset to skip training
3. Run all cells

## Key Results
| Strategy | LP B=10 | LP B=50 | FS B=10 |
|----------|---------|---------|---------|
| TPC_RP | **80.2%** | **83.4%** | **25.6%** |
| Random | 70.8% | 81.4% | 22.6% |
| Modified TPC_RP | 79.5% | 83.0% | -- |
