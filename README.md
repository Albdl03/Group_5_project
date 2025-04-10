# 🌿 ESG Risk Prediction in the Fashion Industry

This project investigates how textual ESG disclosures in the fashion industry relate to actual ESG risk ratings. Using Natural Language Processing (NLP), GRI alignment, and greenwashing detection, we built a predictive model and developed interactive visualizations to evaluate corporate sustainability communication.

## Project Structure

-  'ESG_Group_Project.ipynb` — Python notebook for preprocessing, feature engineering, and predictive modeling.
-  'Dashboard.twbx` — Tableau dashboard for interactive ESG topic and risk visualization.
-  'ESG (Edited) Report.docx` — Full research paper including literature review, methodology, results, and implications.


## Objectives

- Identify whether companies' ESG disclosures align with actual ESG risk ratings.
- Quantify greenwashing tendencies using narrative vs. numeric text balance.
- Build a model to predict ESG risk using features extracted from text.


## Methodology

### Data
- 30 fashion industry ESG reports (2022–2023) collected from company websites.
- ESG risk ratings from [Sustainalytics](https://www.sustainalytics.com/).

### Text Processing
- Tokenization, lemmatization, stopword and company name removal.
- Conversion of raw text to structured formats for analysis.

### Feature Engineering
- `Custom_ESG_Score`: Keyword-based ratio across E, S, and G themes.
- `GRI_Score_norm`: Topic modeling (LDA) weighted against GRI standards.
- `Greenwashing_Score_norm`: Measures text imbalance between narrative and quantitative elements.

### Modeling
- Model: **Random Forest Regressor**
- Performance:
  - R²: 0.62
  - MAE: 1.86
  - RMSE: 2.93
- Top Predictor: GRI-aligned score


## Key Visuals

- ESG keyword frequency & ratio analysis
- Word clouds across all company reports
- GRI standard breakdown by sub-dimension
- Feature importance chart and correlation heatmaps


## Insights

- Environmental keywords dominate due to regulatory scrutiny.
- Companies using vague or overly narrative ESG language scored lower in predictive alignment.
- GRI-based structured reporting leads to stronger correlation with actual risk ratings.


## Business Implications

- ESG communication needs to be transparent, verifiable, and standardized.
- Regulators and investors should encourage (or require) GRI or EU Taxonomy compliance.
- ESG ratings should consider both *what* is being said and *how* it’s being said.


## Limitations & Future Work

- Small sample size (n=30) may limit model generalizability.
- Ratings sourced from only one provider (Sustainalytics).
- Future improvements:
  - Expand dataset over time and industries.
  - Use ESG-specific language models (e.g., BERT for ESG).
  - Build a web-based dashboard with real-time data integration.


## Team

Developed as part of the **ESG Analytics** module at Trinity Business School, 2025.

