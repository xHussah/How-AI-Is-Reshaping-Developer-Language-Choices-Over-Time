# How AI Is Reshaping Developer Language Choices Over Time

This project investigates whether the rise of large language models — specifically the release of ChatGPT in November 2022 — influenced programming language preferences in open-source AI development. Using metadata collected from ~5,750 AI-related GitHub repositories spanning 2020–2025, the study tracks shifts in language popularity, repository engagement, and ecosystem composition before and after ChatGPT's release.

## Key findings 
Python's share among new AI repositories declined from 47.86% to 40.41% post-ChatGPT, while the average stars received by Python repositories surged by 168% (2,171 → 5,812), indicating a shift from Python as the default language to Python as the high-impact platform for LLM projects. A Random Forest regression model achieved R² = 0.912 in predicting secondary language complexity from repository success metrics.

## Dataset
Data was collected via the GitHub REST API, targeting the top-starred AI-related repositories from 2020 to 2025 (250 per quarter per year, ~1,000 per year).

**Features collected per repository:** name, owner, URL, description, stars, forks, creation date, last push date, primary language, all languages (bytes), topics, contributors count.

**Total observations:** ~5,750 repositories.

## Technologies Used
**Language:**
- Python

**Platform:**
- Google Colab

## Models & Results

| Model | MSE | R² |
|---|---|---|
| Baseline (Mean Prediction) | 23.82 | -0.000 |
| Linear Regression | 15.78 | 0.337 |
| Decision Tree Regressor | 3.70 | 0.845 |
| **Random Forest Regressor (Best)** | **2.11** | **0.912** |

**Clustering:** K-Means (K=4, Silhouette Score = 0.383) identified outlier clusters of high-star/high-fork repositories. DBSCAN confirmed most repos form one dense group.

**Hypothesis Testing:** Two-sample t-tests (α = 0.05) confirmed statistically significant changes in both Python's proportion and popularity post-ChatGPT (p < 0.001).


## Developers
- Afnan Alkharji
- Deema Alfarhoud
- Hussah Alotaibi
- Falwa Alkhalifah
- Sana Alotaibi

This project was completed in November 2025. 
