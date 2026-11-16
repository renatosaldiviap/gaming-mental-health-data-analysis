# 🎮 Gaming Habits & Mental Health | Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)

## 📌 Project Overview

This project presents an in-depth **Exploratory Data Analysis (EDA)** examining the relationship between daily gaming hours, player demographics, lifestyle metrics, and mental health indicators (stress, anxiety, depression, and addiction levels) based on a large-scale dataset of **10M records and 40 features**.

Using **Python**, **Pandas**, and statistical sampling optimization in **Google Colab**, raw behavioral data were audited and visualized to test whether prolonged daily playtime directly correlates with elevated mental health risks.

## 🛠️ Tech Stack & Architecture

- **Python (`Pandas`, `NumPy`):** Large-scale schema auditing, memory optimization, random sampling (`n = 100,000`), and quartile segmentation.
- **Data Visualization (`Matplotlib`, `Seaborn`):** Frequency distributions, boxplots, and correlation heatmaps for multi-dimensional insight communication.
- **Cloud Environment (`Google Colab`, `Google Drive API`):** Scalable notebook execution and dataset integration without local hardware bottlenecks.

```text
[ Kaggle Dataset (10M rows) ] ──► [ Schema & Memory Audit ] ──► [ Stratified Sampling (100k) ] ──► [ Visual & Correlation EDA ]
```

## 🔍 Analytical Methodology & Code Highlights
The notebook follows a four-stage analytical workflow to ensure statistical rigor and computational efficiency:
1. Initial Data Audit: Validated dimensions, schema types, memory consumption, and zero-missing-value consistency across 40 behavioral features.
2. Sampling Optimization: Leveraged a statistically representative random sample (100,000 rows) to compute visual distributions without memory overhead.
3. Distribution & Quartile Analysis: Evaluated age ranges, daily playtime spreads, and stress/addiction frequencies across engagement quartiles.

```python
# Representative sample & bivariate correlation check
sample_df = df.sample(n=100_000, random_state=42)
metrics = ['daily_gaming_hours', 'addiction_level', 'stress_level', 'anxiety_score', 'depression_score']
corr_matrix = sample_df[metrics].corr(method='pearson')
```

## 💡 Key Business & Behavioral Insights
1. Moderate Engagement Dominates: Most players log between 1 and 5 daily hours, with heavy outliers representing a minor proportion of the user base.
2. Hours vs. Addiction Link: A strong positive correlation confirms that increased daily gaming hours closely track higher self-reported addiction levels.
3. Mental Health Decoupling: Stress, anxiety, and depression show negligible linear correlation with raw daily playtime, demonstrating that gaming volume alone does not dictate psychological well-being without accounting for broader lifestyle factors (sleep, physical activity).

## 📁 Repository Structure
```text
├── gaming_mental_health_analysis.ipynb   # Main Jupyter Notebook with full EDA
├── .gitignore                            # Excludes large CSV datasets (10M rows)
└── README.md                             # Project documentation and findings
```

## 🚀 How to Run
1. Clone this repository to your local machine:
```bash
git clone https://github.com/renatosaldiviap/gaming-mental-health-data-analysis.git
```
2. Download the dataset from Kaggle - Gaming and Mental Health Dataset.
3. Place gaming_mental_health_10M_40features.csv in your Google Drive or root directory.
4. Open and run gaming_mental_health_analysis.ipynb in Google Colab or Jupyter Notebook.
