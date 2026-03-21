# 🎬 Hollywood Greenlight Analytics: Predicting and Shaping Movie Profitability

## 📌 Project Overview

This project builds an end-to-end Machine Learning and Causal Inference pipeline to predict whether a movie will be a commercial success and prescribes actionable strategies to maximize profitability. By analyzing historical film data, we move beyond simply forecasting box office numbers to answering "what-if" business questions for studio executives.

### 💼 The Business Problem & Objective

The motion picture industry is notoriously high-risk, with most films failing to turn a profit. Traditional forecasting relies heavily on intuition. The objective of this project is to identify the true drivers of commercial success (Return on Investment) and provide data-driven recommendations on talent packaging, narrative themes, and release timing to reduce investment risk.

### 📂 Data Sources & Preprocessing
We combined information from multiple sources to build a comprehensive dataset of over 7,000 movies:

Sources: The Movie Database (TMDB) 5000 dataset, IMDb metadata, and Kaggle Global Movie Franchise datasets.

* Preprocessing Highlights:
  * Merged into master tables (imdb_score_features, roi_features, master_table).
  * Handled the extreme "fat-tail" distribution of box office revenues using logarithmic transformations.
  * Strictly prevented data leakage by removing post-release metrics (like audience votes and scores) before training our pre-release predictive models.

### 🛠️ Methodology & Machine Learning Approach

* Exploratory Data Analysis: Utilized the R.I.C.E. framework (Reach, Impact, Confidence, Effort) to uncover main insights & industry patterns.

* **Statistical Testing**: Validated EDA insights using Two-Sample T-Tests, One-Way ANOVA, and Variance Inflation Factor (VIF) checks.

* **Predictive Modeling & Evaluation**: Trained Supervised ML Models (Logistic Regression (L1), Random Forest, and XGBoost models) to predict profitability greenflag.

* **Causal Machine Learning (Prescriptive Strategy)**: Implemented the X-Learner (Meta-Learner) and Causal Forest for Segmentation Causal Analysis, calculating Conditional Average Treatment Effects (CATE) for specific business interventions.

### 📊 Key Insights & Business Recommendations

By combining exploratory analysis with Causal Machine Learning methods (X-Learner & Causal Forest), we identified the true drivers of a movie's probability to become profitable:

* **The Talent Multiplier**: Upgrading to a "Proven" director is the ultimate risk-mitigation strategy, actively increasing a movie's baseline probability of profitability by ~18% percentage points. This effect is disproportionately stronger for independent studios that lack the massive marketing safety nets of the "Big 6" studios.

* **The Counter-Programming Advantage**: Releasing an indie or mid-budget film during the summer blockbuster season actually provides a ~7.4% to 9.1% lift in profitability probability. The massive influx of cinema foot traffic outweighs the risk of competition, proving that alternative genres (like Comedy or Drama) can thrive as counter-programming against major action tentpoles.

* **Narrative Optimization**: Anchoring a script on reliable, human-centric thematic hooks (rather than gritty/procedural ones) increases the probability of profitability by 8% to 12.8%. This narrative optimization is especially critical for R-rated films, where the potential audience pool is already restricted by age.


