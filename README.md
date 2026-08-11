# 🎬 IMDB Movie Analysis

### Exploratory Data Analysis of the IMDB Movies Dataset using Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

This project explores and analyzes the **IMDB Movies dataset** to uncover trends in genre popularity, rating patterns, and the factors that influence a movie's commercial and critical success. Using Python and its data analysis stack, the project answers a series of business-style questions about what drives movie ratings and revenue, and delivers actionable insights based on the findings.

---

## 📖 Table of Contents

- [Tools & Libraries](#-tools--libraries)
- [About IMDb](#-about-imdb)
- [Dataset Overview](#-dataset-overview)
- [Analysis Workflow](#-analysis-workflow)
- [Key Findings](#-key-findings)
- [Insights & Summary](#-insights--summary)

---

## 🛠 Tools & Libraries

| Tool | Purpose |
|---|---|
| **Python** | Core language for the analysis |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Advanced statistical visualization |

---

## 🎥 About IMDb

IMDb (Internet Movie Database) is a comprehensive online database of information about films, television shows, video games, and streaming content — including cast and crew details, plot summaries, user reviews, trivia, and ratings. Established in 1990 and owned by Amazon since 1998, IMDb is one of the most widely used platforms for movie enthusiasts and industry professionals, offering both user-generated content and professional critiques through its proprietary rating system.

---

## 📂 Dataset Overview

The dataset contains **10,178 movies** across 12 columns:

| Column | Description |
|---|---|
| `names` | Movie title |
| `date_x` | Release date |
| `score` | IMDB rating |
| `genre` | Genre(s) |
| `overview` | Movie summary |
| `crew` | Cast and crew information |
| `orig_title` | Original title |
| `status` | Release status (e.g., Released, Post-Production) |
| `orig_lang` | Original language |
| `budget_x` | Production budget |
| `revenue` | Box office revenue |
| `country` | Production country |

---

## 🔍 Analysis Workflow

The analysis follows a standard EDA pipeline:

1. **Data Loading & Initial Setup** — imported the dataset and reviewed its structure (shape, data types, and sample rows).
2. **Data Cleaning** — converted `date_x` to a proper datetime type; filled missing `genre` and `crew` values (85 and 56 missing respectively) with `"unavailable"`.
3. **Univariate Analysis** — examined the distribution of IMDB scores and identified the most common genres.
4. **Bivariate Analysis** — explored relationships between budget, revenue, and score, including correlation analysis and a boxplot of ratings by country.
5. **Genre-Specific Analysis** — compared average ratings and budgets across genres, and tracked genre popularity over time.
6. **Year & Trend Analysis** — analyzed how average ratings, release volume, and budgets have changed over the years.
7. **Multivariate Analysis** — examined genre popularity by decade and built a correlation heatmap covering budget, genre, country, and revenue.
8. **Additional Analysis** — looked at ratings by country and original language, and how release status affects average revenue.

---

## 📊 Key Findings

- **Score distribution** is roughly normal with a slight left skew — most movies score between 50–80, with very few at the extremes (0 or 100).
- **Most common genre:** Drama.
- **Budget vs. Revenue:** a moderate positive correlation (**0.67**) — higher-budget movies tend to earn more, though there are notable high-budget flops and low-budget hits.
- **Score vs. Budget:** a weak negative correlation (**-0.24**) — bigger budgets don't reliably translate into better ratings.
- **Score vs. Revenue:** a very weak positive correlation (**0.10**) — critical/audience reception has little bearing on box office performance.
- **Highest average ratings by genre:** combinations like *Fantasy/Drama/Crime* and *Adventure/Animation/Comedy/Fantasy/Mystery* topped the list.
- **Release volume:** 2022 had the highest number of releases in the dataset; 1903 had the lowest.
- **Genre budgets:** Drama commands the highest average budget among major genres, while Action tends to have a lower average budget than Comedy or Drama.
- **Ratings by country:** average ratings vary meaningfully by country of production, with SU (Soviet Union–coded entries) topping the list in this dataset.
- **Release status:** movies marked "Released" show the highest average revenue compared to other status categories.

---

## 💡 Insights & Summary

**1. Budget and Revenue Correlation**
There is a strong positive correlation (0.67) between budget and revenue, indicating that movies with higher budgets tend to generate more revenue. This suggests that investing more in movie production is likely to lead to higher financial returns. However, a higher budget doesn't guarantee success — some high-budget films still underperform, while mid-budget films sometimes outperform expectations.

**2. Consistent Movie Ratings Over Time**
From 1980 to 2020, average IMDB ratings remained relatively stable, suggesting movie quality (as measured by user ratings) hasn't changed drastically. A slight decline appears after 2020, possibly linked to shifting audience expectations, pandemic-related disruptions to the movie industry, or changes in the type of content being produced.

**3. Genre-Specific Trends in Budget and Ratings**
Genres like Fantasy, Drama, and Crime tend to receive higher average ratings, while Action movies often have lower budgets than Comedy or Drama. This suggests that more dramatic or fantasy-driven films may benefit from stronger storytelling, while Action films — despite lower production costs — can still perform well commercially, indicating broader accessibility and popularity relative to their budget.

---

<p align="center">
Built with ❤️ using Python, Pandas, and Seaborn
</p>
