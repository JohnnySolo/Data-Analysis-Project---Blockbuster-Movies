# 🎬 Blockbuster Movies Prediction

## 📌 Project Overview

This project builds an end-to-end Machine Learning and Causal Inference pipeline to predict whether a movie will be a commercial success and prescribes actionable strategies to maximize profitability. By analyzing historical film data, we move beyond simply forecasting box office numbers to answering "what-if" business questions for studio executives.

### 💼 The Business Problem & Objective

The motion picture industry is notoriously high-risk, with most films failing to turn a profit. Traditional forecasting relies heavily on intuition. The objective of this project is to identify the true drivers of commercial success (Return on Investment) and provide data-driven recommendations on talent packaging, narrative themes, and release timing to reduce investment risk.

### 🛠️ Methodology & Machine Learning Approach

* Preprocessing Highlights:
  * Merged into master tables (imdb_score_features, roi_features, master_table).
  * Handled the extreme "fat-tail" distribution of box office revenues using logarithmic transformations.
  * Strictly prevented data leakage by removing post-release metrics (like audience votes and scores) before training our pre-release predictive models.

* Exploratory Data Analysis: Utilized the R.I.C.E. framework (Reach, Impact, Confidence, Effort) to uncover industry patterns.

* Statistical Testing: Validated insights using Two-Sample T-Tests, One-Way ANOVA, and Variance Inflation Factor (VIF) checks.

* Predictive Modeling: Trained Logistic Regression (L1), Random Forest, and XGBoost models to predict binary profitability.

* Causal Machine Learning (Prescriptive Strategy): Implemented the X-Learner (Meta-Learner) and DR-Learner (Doubly Robust) to calculate Average Treatment Effects (ATE) and Conditional Average Treatment Effects (CATE) for specific business interventions.

---

## 📂 Dataset

# Datasets for Blockbuster Movies Analysis

Our goal is to build a comprehensive dataset of blockbuster movies and find a model that optimizes all the information we got. We'll combine information from multiple sources. Below are some datasets that align with our project requirements:

---

**1. Movie Data Analysis Dataset**  
- Details about 7,668 movies, including:
  - Titles, ratings, genres, release years
  - IMDb scores, votes
  - Directors, writers, main stars
  - Production countries, budgets, gross earnings
  - Production companies, runtimes  
- **Source**: [GitHub Repository](https://github.com/1tannu5/Movie-Data-Analysis?utm_source=chatgpt.com)

---

**2. Global Movie Franchise Revenue and Budget Data**  
- Comprehensive data on movie franchises worldwide between 2000–2020:
  - Lifetime gross, budget, rating
  - Runtime, release date, vote count/average  
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/thedevastator/global-movie-franchise-revenue-and-budget-data?utm_source=chatgpt.com)

---

**3. TMDB 5000 Movies Dataset**  
- Information on over 5,000 movies:
  - Budget, cast, director
  - Keywords, runtime, genres
  - Production companies, release dates  
- **Source**: [Hugging Face Dataset](https://huggingface.co/datasets/AiresPucrs/tmdb-5000-movies/blob/main/README.md?utm_source=chatgpt.com)

---

**4. Complete Movie Metadata Dataset**  
- Data on over 722,000 movies, including:
  - ID, title, genres, budget, revenue  
- Suitable for analyzing trends in movie popularity, production companies, budgets, and revenues.  
- **Source**: [Gigasheet Dataset](https://www.gigasheet.com/sample-data/movies-daily-update-dataset?utm_source=chatgpt.com)

---

**5. Movie Revenue Analysis Dataset**  
- Approx. 1,800 movies released between 1915 and 2020:
  - Domestic and worldwide gross revenues
  - Production budgets, release dates  
- **Source**: [GitHub Repository](https://github.com/ntdoris/movie-revenue-analysis?utm_source=chatgpt.com)

---

