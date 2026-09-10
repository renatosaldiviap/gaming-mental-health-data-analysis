# Gaming Habits & Mental Health: Exploratory Data Analysis (EDA)

An in-depth exploratory data analysis examining the relationship between daily gaming hours, player demographics, lifestyle metrics, and mental health indicators (stress, anxiety, depression, and addiction levels).

---

## Project Overview
Video games are one of the most prominent entertainment industries globally, sparking ongoing discussions regarding their impact on well-being. This project analyzes a large-scale gaming dataset to uncover whether prolonged daily playtime correlates with elevated mental health risks or distinct behavioral patterns.

- **Primary Goal:** Investigate correlations between daily gaming hours and well-being scores.
- **Dataset Source:** [Kaggle - Gaming and Mental Health Dataset](https://www.kaggle.com/datasets/sharmajicoder/gaming-and-mental-health) (10M records, 40 features).
- **Methodology:** Exploratory Data Analysis (EDA), statistical profiling, sample-based visual distributions, and correlation analysis.

---

## Tech Stack & Tools
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Google Colab, Google Drive API

---

## Key Highlights & Analytical Flow
1. **Initial Data Audit:** Validated dimensions, schema types, memory consumption, and zero-missing-value consistency.
2. **Sampling Optimization:** Leveraged a statistically representative random sample (100,000 rows) to run high-performance visual distributions without computational overhead.
3. **Distribution Analysis:** Analyzed age ranges, gaming hours spreads, and stress level frequencies.
4. **Bivariate Exploration:** Evaluated gaming time quartiles against reported addiction and stress metrics.

---

## Key Insights & Conclusions
* **Moderate Engagement Dominates:** Most players log between 1 and 5 daily hours, with heavy outliers representing a minor proportion of the user base.
* **Hours vs. Addiction Link:** A strong positive correlation confirms that increased daily gaming hours closely track higher self-reported addiction levels.
* **Mental Health Decoupling:** Stress, anxiety, and depression show negligible linear correlation with raw daily playtime, challenging common assumptions that gaming volume alone dictates psychological well-being.
* **Analytical Takeaway:** Gaming intensity correlates with perceived addiction, but broader lifestyle factors (sleep, physical activity) and psychological metrics operate largely independently within this dataset. Future iterations should explore cluster-based behavioral segmentation.

---

## Repository Structure
```text
├── gaming_mental_health_analysis.ipynb   # Main Jupyter Notebook with full EDA
├── .gitignore                           # Excludes large CSV datasets
└── README.md                            # Project documentation and findings
```

## How to Run
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/RenatoSaldivia/gaming-mental-health-data-analysis.git
   ```
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/sharmajicoder/gaming-and-mental-health).
3. Place `gaming_mental_health_10M_40features.csv` in your Google Drive or root directory.
4. Run `gaming_mental_health_analysis.ipynb` using Jupyter Notebook or Google Colab.