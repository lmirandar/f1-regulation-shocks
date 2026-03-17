
# Regulation Shocks and Competitive Order in Formula 1

*A causal inference study treating F1 regulation changes as policy interventions in a competitive market.*

---

## Research Question

**Did major Formula 1 regulation changes increase competitive instability in the Constructors' Championship in the first 1–3 seasons after implementation?**

**Stretch:** Are larger regulation shocks associated with larger competitive reshuffles?

## Why This Matters

Every few years, the FIA rewrites the technical rulebook with the stated goal of leveling the playing field. But do these regulatory resets actually disrupt the competitive hierarchy or do the same teams find their way back to the top?

This is the same question any industry faces when regulators intervene: telecom spectrum auctions, pharmaceutical patent cliffs, financial regulation overhauls. The analytical framework here, measuring how regulatory shocks reshape market concentration and how quickly incumbents reconverge, transfers directly to policy evaluation in any competitive market.

## Methodology

- **Panel dataset** of constructor-level performance from 1958–2025 via the Jolpica (Ergast-compatible) API
- **6 major regulation resets** analyzed: 1998, 2005, 2009, 2014, 2017, 2022
- **Concentration metrics:** HHI (Herfindahl-Hirschman Index), points share, rank volatility (Kendall's τ), top-3 turnover, champion turnover
- **Statistical methods:** Interrupted time series, event-study windows, structural break tests (Chow/Bai-Perron), placebo controls on non-regulation years
- **Reconvergence analysis:** How many seasons until competitive concentration returns to pre-shock levels

## Key Findings

> *Coming soon — analysis in progress.*

## Tech Stack

| Layer | Tool |
|-------|------|
| Data Ingestion | Python, FastF1 (Jolpica integration) |
| Storage | Parquet |
| Analysis | Pandas, NumPy, SciPy, statsmodels |
| Visualization | Matplotlib, Plotly |
| Report | Quarto / Jupyter |

## Repo Structure

```
f1-regulation-shocks/
├── data/
│   ├── raw/              # API exports
│   └── processed/        # Cleaned, metric-ready datasets
├── src/                  # ETL pipeline and metric functions
├── notebooks/            # Numbered analysis notebooks
├── report/               # Final write-up and visualizations
├── tests/                # Data sanity checks
├── dashboard/            # Interactive app (stretch goal)
├── requirements.txt
└── README.md
```

## Status

🟡 **In Progress** Phase 1: Data Collection & EDA

---

*Built by Sofía · MS Information Systems (Business Analytics), Florida International University*
