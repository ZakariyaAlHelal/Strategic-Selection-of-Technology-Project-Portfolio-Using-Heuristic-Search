# Strategic Selection of Technology Project Portfolio Using Heuristic Search

This repository accompanies the paper: "Strategic Selection of a Technology Project Portfolio as a Multi-Dimensional Knapsack Problem with Structured Balance Penalties" 
and provides a reproducible implementation of the proposed optimization framework.

## Overview

The project implements a heuristic-based portfolio optimization approach using Simulated Annealing (SA) to select a balanced and resource-feasible set of projects.

The framework supports multiple data sources and experimental configurations, enabling flexible testing and reproducibility.

## Purpose

This project provides a computational decision-support framework for strategic project portfolio selection under constraints, enabling analysis of trade-offs between short-term value and long-term capability development.

---

## Model Summary
The portfolio selection model integrates:

- Primary strategic value score (p)
- Complementarity score (c)
- Future capability score (f)
- Budget constraint
- Human resource constraint
- Time horizon balance (Short / Medium / Long)
- Strategic intent balance (Exploratory / Exponential / Sustaining)

A heuristic search procedure is applied to identify high-quality feasible portfolios that satisfy resource and balance requirements.

---

## How to Run
1. Open the notebook: `strategic_technology_portfolio_selection.ipynb`
2. Run all cells sequentially.
3. The model loads input data from:

   `data/portfolio_dataset.xlsx`

4. Results and selected portfolios are displayed at the end of the notebook.

---

## Data Description
The dataset includes:

- idx – Project identifier
- g – Screening eligibility indicator (0/1)
- p – Primary strategic score (1–10)
- c – Complementarity score (1–10)
- f – Future capability score (1–10)
- b – Budget requirement
- h – Human resource requirement
- time_cat – Time horizon category
- intent_cat – Strategic intent category

---
## Data Input Options

The model now supports three input modes:

- **GitHub dataset** (default): Loads the provided dataset from the repository  
- **User upload**: Allows uploading a custom `.xlsx` or `.csv` file with the same template  
- **Synthetic data generation**: Generates datasets (e.g., 60 projects) using controlled distributions consistent with the paper  

This flexibility allows both replication of the original study and extension to new scenarios.

## Key Features

- Multi-dimensional portfolio optimization (value + balance)
- Resource constraints (budget and staff-hours)
- Balance penalties across:
  - Time horizon (Short / Medium / Long)
  - Strategic intent (Exploratory / Exponential / Sustaining)
- Synthetic data generation aligned with experimental assumptions
- Export of optimized portfolios and datasets
- Ready integration with simulation tools (e.g., Arena)
