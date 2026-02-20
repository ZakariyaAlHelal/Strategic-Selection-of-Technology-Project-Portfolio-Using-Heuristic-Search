# Strategic Selection of Technology Project Portfolio Using Heuristic Search

## Purpose
This project develops a computational decision-making framework for the strategic selection of technology project portfolios under resource constraints.

The model supports structured portfolio balancing across time horizons and strategic intent dimensions, enabling firms to evaluate trade-offs between short-term value and long-term capability development.

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

## Conceptual Foundation
The model operationalizes strategic portfolio management through structured quantitative evaluation and constrained optimization.
