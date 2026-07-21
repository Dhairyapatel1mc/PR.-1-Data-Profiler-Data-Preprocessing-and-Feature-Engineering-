<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=timeGradient&height=220&section=header&text=Data%20Profiler&fontSize=52&fontAlignY=38&desc=Data%20Preprocessing%20%26%20Feature%20Engineering&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-4DABCF?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white"/>
  <img src="https://img.shields.io/badge/REST%20API-005571?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-2D7D7D?style=flat-square"/>
  <img src="https://img.shields.io/badge/Type-Data%20Preprocessing-C9A84C?style=flat-square"/>
  <img src="https://img.shields.io/badge/Duration-5%20Hours-A0394A?style=flat-square"/>
</p>

<p align="center">
  <a href="https://github.com/Dhairyapatel1mc"><img src="https://skillicons.dev/icons?i=github" height="40"/></a>
  &nbsp;
  <a href="https://www.linkedin.com/in/ghost-patel-0267663b7/"><img src="https://skillicons.dev/icons?i=linkedin" height="40"/></a>
  &nbsp;
  <a href="https://www.instagram.com/ghost_6927/?hl=en"><img src="https://skillicons.dev/icons?i=instagram" height="40"/></a>
</p>

---

<a name="toc"></a>
## 📌 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [🎯 Project Objectives](#-project-objectives)
- [🚀 Features](#-features)
- [📊 Dataset Attributes](#-dataset-attributes)
- [📁 Project Structure](#-project-structure)
- [🧠 Statistical Concepts Used](#-statistical-concepts-used)
- [🧰 Technologies Used](#-technologies-used)
- [⚙️ Installation](#️-installation)
- [▶️ How to Run](#️-how-to-run)
- [📈 Visualizations](#-visualizations)
- [📄 Sample Results](#-sample-results)
- [🎓 Learning Outcomes](#-learning-outcomes)
- [💡 Future Improvements](#-future-improvements)
- [👤 Author](#-author)
- [⭐ Support](#-support)
- [🏆 Final Conclusion](#-final-conclusion)

---

## <a id="-project-overview"></a>🎯 Project Overview

**Data Profiler** takes a customer dataset scattered across four different sources — CSV, JSON, a SQL database, and a REST API — and turns it into a single, clean, ML-ready dataset. Working as a Junior Data Analyst, the task is to unify the data, clean it, explore it, and frame it as a machine learning problem: **predicting customer churn**.

The project is split into five parts, matching the original assignment structure:

| Part | Focus |
|------|-------|
| **Part A — Fundamentals** | Data analysis theory, project planning, ML problem framing, and tensors |
| **Part B — Data Acquisition** | Importing and merging data from CSV, JSON, SQL, and an API |
| **Part C — Data Understanding & Cleaning** | Initial exploration, missing values, duplicates, dtype fixes |
| **Part D — Exploratory Data Analysis** | Univariate, bivariate, and multivariate analysis |
| **Part E — Data Profiling** | A custom-built profiling report: missing values, stats, correlations, warnings |

> 🏫 **Title:** Data Profiler &nbsp;·&nbsp; **Duration:** 5 Hours

**[⬆ Back to top](#toc)**

---

## <a id="-project-objectives"></a>🎯 Project Objectives

- Explain core data analysis concepts — the data science project lifecycle, tensors, and how to frame an ML problem
- Import and merge customer data from four different real-world formats
- Identify and resolve missing values, duplicates, and inconsistent data types
- Explore the data through univariate, bivariate, and multivariate analysis
- Build an automated data profiling report highlighting quality issues
- Frame a clear, business-relevant machine learning problem: predicting churn

**[⬆ Back to top](#toc)**

---

## <a id="-features"></a>🚀 Features

- 📓 One structured Jupyter notebook, mirroring the assignment's own Part A–E structure
- 🔌 Genuine multi-source data integration — a real CSV, a real JSON file, a real SQLite database, and a real REST API call (with an offline-safe cached fallback)
- 🧹 Realistic, intentional data quality issues (missing values, duplicates, mixed types) cleaned step-by-step, not a pre-cleaned toy dataset
- 📊 6 exported chart images, so results can be viewed without opening Jupyter
- 🗣️ Every code cell is paired with a plain-English, student-voice markdown explanation
- 📋 A dependency-free, hand-built data profiling report with automated quality warnings
- 🔁 Fully reproducible — fixed random seed, clean and minimal plotting code throughout

**[⬆ Back to top](#toc)**

---

## <a id="-dataset-attributes"></a>📊 Dataset Attributes

| Column | Source | Type | Description |
|--------|--------|------|-------------|
| `Customer_ID` | All | string | Unique customer identifier (join key across sources) |
| `Age` | JSON | float | Customer's age |
| `Income` | JSON | float | Annual income |
| `Region` | JSON | categorical | North / South / East / West |
| `Purchases` | CSV | integer | Number of purchases made |
| `Total_Spent` | CSV | float | Total amount spent |
| `Signup_Date` | CSV | date | Date the customer signed up |
| `Gender` | SQL | categorical | Male / Female |
| `Churn` | SQL | categorical | Whether the customer churned (Yes/No) — the ML target |

~1,000 synthetic customer records, split across sources and merged on `Customer_ID`, with intentional missing values, duplicates, and mixed types for the cleaning tasks.

**[⬆ Back to top](#toc)**

---

## <a id="-project-structure"></a>📁 Project Structure

```
.
├── README.md                             # You are here
├── data_profiler.ipynb                   # Main analysis notebook (Part A–E)
└── sources/                              # Raw multi-format data sources
    ├── customer_transactions.csv         # Part B: CSV source
    ├── customer_demographics.json        # Part B: JSON source
    ├── customers.db                      # Part B: SQL source (SQLite)
    └── cached_api_response.json          # Part B: cached REST API sample
└── charts/                               # Exported chart images (PNG)
    ├── 01_missing_values_before_cleaning.png
    ├── 02_univariate_distributions.png
    ├── 03_bivariate_gender_income_churn.png
    ├── 04_correlation_heatmap.png
    ├── 05_pairplot_feature_interactions.png
    └── 06_profiling_warning_summary.png
```

**[⬆ Back to top](#toc)**

---

## <a id="-statistical-concepts-used"></a>🧠 Statistical Concepts Used

**Part A — Tensors** — Using plain NumPy arrays, the notebook builds a scalar (0-D), a vector (1-D), a matrix (2-D), and a stacked 3-D tensor, checking `.ndim` and `.shape` on each to show how tabular data is really just a tensor of a given dimension — the same representation any ML model receives as input.

**Part B — Multi-Source Acquisition** — `pd.read_csv()` loads the transactional data, `json.load()` parses the demographic file, `pd.read_sql()` pulls the status table out of a SQLite database via `sqlite3.connect()`, and a `requests.get()` call (with a cached-file fallback) demonstrates a live REST API pull. All three core sources are joined into one DataFrame with repeated `.merge()` calls on `Customer_ID`.

**Part C — Cleaning** — `.isnull().sum()` and `.duplicated().sum()` quantify exactly what's wrong before touching anything. Cleaning then applies `drop_duplicates()`, strips stray currency symbols with `.str.replace()` before casting to float, imputes missing `Income` with the median (robust to its right skew), and drops the empty `Notes` column.

**Part D — EDA** — Univariate analysis uses histograms per column to see each variable's shape in isolation. Bivariate analysis uses `sns.boxplot()` to compare a numeric variable's spread across categories (Gender, Churn). Multivariate analysis layers on a `.corr()` heatmap and a full `sns.pairplot()`, colored by `Churn`, to catch relationships a single correlation number would miss.

**Part E — Profiling** — Rather than an external library, the report is hand-built: missing-value percentages, `.describe()` statistics, and a correlation matrix, plus a small rule-based checker that flags high skewness (`.skew()`), high pairwise correlation, and high-cardinality categorical columns — the same categories of issue a tool like `pandas-profiling` reports automatically.

**[⬆ Back to top](#toc)**

---

## <a id="-technologies-used"></a>🧰 Technologies Used

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)

</div>

**[⬆ Back to top](#toc)**

---

## <a id="-installation"></a>⚙️ Installation

```bash
# Clone the repository
git clone <YOUR_REPO_URL>
cd data-profiler

# Install dependencies
pip install numpy pandas matplotlib seaborn requests jupyter
```

**[⬆ Back to top](#toc)**

---

## <a id="-how-to-run"></a>▶️ How to Run

1. Make sure the `sources/` folder (with the CSV, JSON, SQLite `.db`, and cached API response) is in the project directory.
2. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
3. Open `data_profiler.ipynb`.
4. Run all cells in order (**Cell → Run All**). Part C, D, and E all build on the merged and cleaned dataset from earlier cells, so cells should not be skipped.

**[⬆ Back to top](#toc)**

---

## <a id="-visualizations"></a>📈 Visualizations

| | |
|---|---|
| ![Missing Values](charts/01_missing_values_before_cleaning.png) | ![Univariate Distributions](charts/02_univariate_distributions.png) |
| ![Bivariate Analysis](charts/03_bivariate_gender_income_churn.png) | ![Correlation Heatmap](charts/04_correlation_heatmap.png) |
| ![Pair Plot](charts/05_pairplot_feature_interactions.png) | ![Profiling Warnings](charts/06_profiling_warning_summary.png) |

**[⬆ Back to top](#toc)**

---

## <a id="-sample-results"></a>📄 Sample Results

| Task | Finding | Insight |
|---|---|---|
| Data Acquisition | 4 sources merged (CSV, JSON, SQL, API) | Company data is genuinely fragmented across systems |
| Data Cleaning | Duplicates removed, Income imputed, dtypes fixed | Dataset is now ML-ready and type-consistent |
| Univariate Analysis | Income & Purchases are right-skewed | A log transform may help these features for modeling |
| Bivariate Analysis | Lower-income customers show higher churn | Income is a candidate predictor for the churn model |
| Multivariate Analysis | Purchases & Total_Spent are strongly correlated | One of the two may be redundant as a model feature |
| Data Profiling | Automated warnings raised | Report flags exactly what to address before modeling |

*(Exact numeric values are computed live in the notebook and printed under each task.)*

**[⬆ Back to top](#toc)**

---

## <a id="-learning-outcomes"></a>🎓 Learning Outcomes

- How to import and merge data from CSV, JSON, SQL, and REST API sources into one working dataset
- How to systematically detect and fix missing values, duplicates, and inconsistent data types
- How to represent data as tensors and connect that idea back to real DataFrame structures
- How to perform univariate, bivariate, and multivariate EDA with the right chart for each
- How to build a data profiling report from scratch, without relying on a black-box library
- How to frame a business problem as a concrete, well-defined machine learning task

**[⬆ Back to top](#toc)**

---

## <a id="-future-improvements"></a>💡 Future Improvements

- Train an actual churn classification model (e.g. logistic regression) on the cleaned dataset
- Swap the manual profiling report for `ydata-profiling` for an interactive HTML version
- Add feature engineering — e.g. Income-to-Purchases ratio, tenure since Signup_Date
- Automate the pipeline with a scheduled script that re-pulls all four sources on a cadence
- Add data validation checks (e.g. Great Expectations) to catch quality issues at ingestion, not after

**[⬆ Back to top](#toc)**

---

## <a id="-author"></a>👤 Author

<table>
<tr>
<td valign="top">

**Ghost (Patel Dhairya)**

- 🏫 Red and White Skill Education (RWSkill)
- 💻 GitHub — [@Dhairyapatel1mc](https://github.com/Dhairyapatel1mc)
- 💼 LinkedIn — [ghost-patel](https://www.linkedin.com/in/ghost-patel-0267663b7/)
- 📷 Instagram — [@ghost_6927](https://www.instagram.com/ghost_6927/?hl=en)

</td>
<td align="center" valign="middle">

<a href="https://github.com/Dhairyapatel1mc"><img src="https://skillicons.dev/icons?i=github" height="40"/></a>
&nbsp;
<a href="https://www.linkedin.com/in/ghost-patel-0267663b7/"><img src="https://skillicons.dev/icons?i=linkedin" height="40"/></a>
&nbsp;
<a href="https://www.instagram.com/ghost_6927/?hl=en"><img src="https://skillicons.dev/icons?i=instagram" height="40"/></a>

</td>
</tr>
</table>

**[⬆ Back to top](#toc)**

---

## <a id="-support"></a>⭐ Support

If this project helped you:

- ⭐ **Star** this repository
- 🍴 **Fork** it and adapt it for your own dataset
- 📤 **Share** it with your classmates
- 💬 **Open an Issue** for suggestions or bugs

**[⬆ Back to top](#toc)**

---

## <a id="-final-conclusion"></a>🏆 Final Conclusion

Unifying four scattered data sources into one clean, well-understood dataset is most of the real work behind any machine learning project — and it's exactly what this notebook demonstrates end to end. After cleaning, the data shows a clear, business-relevant pattern: customers with lower income churn more often, and purchase count tracks closely with total spend, meaning a churn model likely doesn't need both as separate inputs. With the data now profiled, cleaned, and explored, it's genuinely ready for the next step — training an actual churn prediction model.

**[⬆ Back to top](#toc)**

---

<div align="center">

![Footer](https://capsule-render.vercel.app/api?type=waving&color=timeGradient&height=100&section=footer)

</div>
