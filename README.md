# Movie Industry Correlation Analysis

## Overview
This project analyzes over 7,600 movies released between 1980 and 2020 to uncover what factors most influence a movie's gross earnings. Using Python for data cleaning and exploratory data analysis, the project identifies key relationships between movie features like budget, votes, and revenue through correlation analysis and visualizations.

---

## Tools Used
- **Python** — data cleaning, EDA, and correlation analysis
- **Pandas** — data manipulation and cleaning
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — KNN Imputation for missing values
- **Jupyter Notebook** — development environment

---

## Dataset
- **movies.csv** — 7,668 movie records with 15 features
- Features include: name, rating, genre, year, budget, gross, score, votes, director, star, company, runtime, and more
- Time range: 1980 – 2020

---

## What I Analyzed
- Budget vs gross earnings relationship
- Correlation between all numeric and categorical movie features
- Key drivers of gross revenue
- Movie revenue trends across four decades

---

## Data Cleaning Steps
- Checked and removed duplicate records
- Dropped rows with irrecoverable null values (released, writer, star, country, company)
- Applied **KNN Imputation** (K=5) to fill missing numeric values — budget, gross, votes, score, runtime
- Used group-based mode fill for missing movie ratings by genre
- Extracted and corrected release year from the released column
- Converted budget and gross to integer data types

---

## Key Findings
- **Budget and gross are strongly correlated (0.75)** — higher budget movies tend to earn more
- **Votes** also showed strong correlation with gross earnings
- **Company** had minimal correlation with gross earnings
- These insights suggest that production investment and audience engagement are the strongest predictors of a movie's financial success

---

## Visualizations
- Scatter plot — Budget vs Gross Earnings
- Regression plot — Budget vs Gross with trend line
- Correlation heatmap — numeric features only
- Correlation heatmap — all features including encoded categoricals

---

## Project Structure
```
movie-correlation-analysis/
│
├── Movies_FullProject.ipynb      # Full Python analysis notebook
├── movies.csv                    # Raw dataset
└── README.md
```

---

## How to Run
1. Clone this repository
2. Open `Movies_FullProject.ipynb` in Jupyter Notebook
3. Run all cells in order

**Required libraries:**
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Author
**Divya Idupulapati**
- Email: idupulapatidivya07@gmail.com
- [LinkedIn](#) | [Portfolio](#) | [GitHub](#)
