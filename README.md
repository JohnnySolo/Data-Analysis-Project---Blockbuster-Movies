# 🎬 Blockbuster Movies Prediction

## 📌 Project Overview

This project aims to build a Machine Learning model that predicts whether a movie can be considered a **blockbuster** — both in terms of audience reception and financial success.

### 🔥 What Is a Blockbuster?

A **blockbuster movie** is generally defined as a film that achieves **both high profitability and high public acclaim**. 
To capture this, we define two measurable targets:
- **IMDB Score**: Proxy for audience satisfaction and critical reception.
- **ROI (Return on Investment)**: Proxy for commercial success.

### 🎯 Project Goals

- Perform **Exploratory Data Analysis (EDA)** to understand patterns behind blockbuster movies.
- Build predictive models for:
  1. **IMDB Score**
  2. **ROI**
- Optionally, create a combined model to classify blockbuster likelihood based on both.

---

## 📂 Dataset

Our data is sourced from multiple tables containing:
- Movie metadata
- Financials (budget, gross)
- Cast and crew
- Genre and keywords
- IMDB ratings

These are merged and cleaned into:
- `imdb_score_features`
- `roi_features`
- `master_table`

---

## 🛠️ Methods & Tools

- Python (Pandas, Scikit-learn)
- Feature engineering based on domain knowledge and EDA
- ML models (regression, classification)

---

## 🤖 Why IMDB Score and ROI?

- **IMDB Score** reflects whether people *liked* the movie — crucial for sustained popularity and brand value.
- **ROI** captures whether the film was a *financial hit* — crucial for studios and investors.

Combining these helps us define and detect "blockbusters" more holistically.

---

## 🚀 Future Work

- Incorporate marketing or release strategy data (e.g., release date, streaming vs theater)
- Refine model into binary classification: "Blockbuster vs Not"
