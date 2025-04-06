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
