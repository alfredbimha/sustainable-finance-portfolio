# Sustainable Finance Research Portfolio

A 20-project research portfolio in sustainable finance, financial econometrics, and ESG analytics — built with Python, R, and Stata using real-world financial data.

Each project follows a complete research workflow: formulating a research question, collecting and processing data, applying rigorous econometric or analytical methods, and interpreting results with methodological caveats.

---

## Portfolio Overview

| # | Project | Category | Methods | Languages |
|---|---------|----------|---------|-----------|
| 1 | [Volatility Dynamics of Green vs Brown Assets](https://alfredbimha.github.io/project1_volatility_green_brown/) | Financial Econometrics | GARCH(1,1), GJR-GARCH, rolling forecasts | Python, R |
| 2 | [ESG Scores and Financial Performance](https://alfredbimha.github.io/project2_esg_panel_regression/) | Financial Econometrics | Panel FE/RE, Hausman test, clustered SEs | Python, Stata, R |
| 3 | [Green Factor Premium Analysis](https://alfredbimha.github.io/project3_fama_french_green/) | Financial Econometrics | Fama-French 3 & 5-factor, GRS test | Python, R |
| 4 | [Cointegration of Clean & Fossil Energy](https://alfredbimha.github.io/project4_cointegration_energy/) | Financial Econometrics | Engle-Granger, Johansen, VECM, IRF | Python |
| 5 | [Market Reaction to ESG Rating Changes](https://alfredbimha.github.io/project5_event_study_esg/) | Financial Econometrics | Market model, CAR, cross-sectional t-test | Python, Stata |
| 6 | [ESG Rating Disagreement Dashboard](https://alfredbimha.github.io/project6_esg_disagreement/) | Sustainability Analytics | Kendall's τ, pillar decomposition, heatmaps | Python, R |
| 7 | [Climate Risk Disclosure NLP Analysis](https://alfredbimha.github.io/project7_climate_nlp/) | Sustainability Analytics | Keyword dictionaries, TF-IDF, LDA | Python |
| 8 | [Geospatial Climate Risk Mapping](https://alfredbimha.github.io/project8_geospatial_climate/) | Sustainability Analytics | Spatial joins, folium mapping, risk scoring | Python, R |
| 9 | [Corporate Water Stress Financial Analysis](https://alfredbimha.github.io/project9_water_stress/) | Sustainability Analytics | Risk scoring, sector benchmarking, scenarios | Python, R |
| 10 | [Corporate Biodiversity Footprint Assessment](https://alfredbimha.github.io/project10_biodiversity_footprint/) | Sustainability Analytics | TNFD LEAP, ENCORE, MSA metrics | Python, R |
| 11 | [Green Bond Premium (Greenium) Analysis](https://alfredbimha.github.io/project11_green_bond_premium/) | Financial Analytics | Matched pairs, paired t-test, panel regression | Python, R |
| 12 | [Green Lending Regulation Impact](https://alfredbimha.github.io/project12_bank_lending_did/) | Financial Analytics | Difference-in-differences, triple difference | Python, Stata |
| 13 | [Sovereign ESG and Bond Spreads](https://alfredbimha.github.io/project13_sovereign_esg/) | Financial Analytics | Panel FE, Driscoll-Kraay SEs, pillar decomposition | Python, R |
| 14 | [Global Climate Finance Flow Analysis](https://alfredbimha.github.io/project14_climate_finance_flows/) | Financial Analytics | Flow decomposition, gap analysis, mobilisation ratios | Python, R |
| 15 | [Impact Investing Portfolio Optimisation](https://alfredbimha.github.io/project15_impact_investing/) | Financial Analytics | Markowitz MVO, impact constraints, Sharpe comparison | Python, R |
| 16 | [ESG Controversy Event Prediction](https://alfredbimha.github.io/project16_esg_controversy/) | Sustainable Finance Analytics | XGBoost, Random Forest, SHAP importance | Python |
| 17 | [Central Bank Climate Communication](https://alfredbimha.github.io/project17_central_bank_nlp/) | Sustainable Finance Analytics | Structural topic model (STM), sentiment analysis | Python, R |
| 18 | [Stranded Assets Valuation](https://alfredbimha.github.io/project18_stranded_assets/) | Sustainable Finance Analytics | Monte Carlo simulation, NGFS scenarios, VaR | Python, R |
| 19 | [Carbon Risk Factor Replication](https://alfredbimha.github.io/project19_carbon_risk_replication/) | Sustainable Finance Analytics | Fama-MacBeth two-pass, Newey-West correction | Python, Stata, R |
| 20 | [Reproducible Research Template](https://alfredbimha.github.io/project20_reproducible_research/) | Research Methods | Makefile automation, FAIR data, version control | Python, R, Stata |

---

## Category Breakdown

### I. Financial Econometrics (Projects 1–5)

Core time series and panel data methods applied to sustainable finance questions. These projects demonstrate proficiency in the standard econometric toolkit used in empirical finance research: volatility modelling (GARCH), panel regressions with fixed effects, asset pricing factor models, cointegration and error correction, and event study methodology.

### II. Sustainability Analytics (Projects 6–10)

Data science and analytics applied to environmental and social sustainability questions. These projects go beyond traditional finance to incorporate NLP text mining of corporate disclosures, geospatial climate risk analysis, water stress quantification, and biodiversity impact measurement using emerging frameworks like TNFD and ENCORE.

### III. Financial Analytics (Projects 11–15)

Quantitative analysis of sustainable finance instruments and markets. Projects cover green bond pricing (the "greenium"), causal inference for policy evaluation using difference-in-differences, sovereign ESG-spread modelling with World Bank data, climate finance flow tracking, and multi-objective portfolio optimisation for impact investing.

### IV. Sustainable Finance Analytics (Projects 16–20)

Advanced methods including machine learning, Monte Carlo simulation, and academic replication. Projects apply XGBoost with SHAP interpretability to ESG controversy prediction, structural topic modelling to central bank communications, stochastic simulation to stranded asset valuation under NGFS climate scenarios, and Fama-MacBeth regressions to replicate the carbon risk premium literature.

---

## Data Sources

| Source | Access Method | Projects |
|--------|--------------|----------|
| Yahoo Finance | `yfinance` Python library | 1, 4, 15 |
| SEC EDGAR | REST API with User-Agent header | 7 |
| World Bank | `wbgapi` Python library | 13 |
| CPI / OECD / GCF | Published datasets | 14 |
| Kenneth French Library | `pandas-datareader` | 3 |
| Simulated (calibrated) | Custom generation scripts | 2, 5, 6, 8–12, 16–19 |

Projects using simulated data are calibrated to match the distributional properties of published academic datasets (e.g., Refinitiv ESG, CRSP, Compustat). A data sourcing guide exists for converting remaining projects to real data.

---

## Key Findings

Selected results that can be cited and discussed:

- **Energy vs clean energy cointegration**: ICLN and XLE are cointegrated at p = 0.03, confirming a shared long-run price equilibrium (Project 4)
- **Climate disclosure intensity**: Energy sector averages ~39 climate keywords per SEC 10-K filing vs. near zero for tech companies (Project 7)
- **Governance dominates sovereign spreads**: Governance improvements predict lower sovereign bond spreads at t = −2.28, while environmental metrics are not yet priced (Project 13)
- **Impact investing performance**: Impact fund portfolios achieve a Sharpe ratio of ~0.42 vs ~0.36 for conventional benchmarks (Project 15)
- **Carbon risk premium**: Estimated at 1.5–3.0% annually, consistent with Bolton & Kacperczyk (2021) (Project 19)
- **Stranded asset risk**: Net Zero 2050 scenario implies 45–65% impairment of fossil fuel asset book value (Project 18)

---

## Technical Environment

**Languages:** Python (primary), R, Stata

**Key Python packages:** pandas, numpy, scipy, statsmodels, linearmodels, arch, yfinance, scikit-learn, xgboost, shap, geopandas, folium, nltk, matplotlib, seaborn, plotly

**Key R packages:** plm, stm, quanteda, ggplot2, fixest, PortfolioAnalytics, sf, tmap

**Stata commands:** xtreg, xtset, hausman, coint, eventstudy, did_multiplegt

---

## Methodology Note

This portfolio uses an **AI-assisted research workflow**. All research questions, methodological choices, and result interpretations are directed by the researcher. Code implementation is assisted by Claude AI — reflecting a modern, collaborative approach to data-intensive research. This workflow is fully transparent and documented throughout the portfolio.

---

## Repository Structure

Each of the 20 project repositories contains:

```
project_name/
├── index.html          # Visual research guide (viewable via GitHub Pages)
├── main_analysis.py    # Primary analysis script (heavily commented)
├── README.md           # Project-specific documentation
├── requirements.txt    # Python dependencies
├── data/               # Raw and processed data files
└── output/             # Generated figures, tables, and results
```

---

## Contact

[Your Name] · [Your Email] · [Your LinkedIn]
