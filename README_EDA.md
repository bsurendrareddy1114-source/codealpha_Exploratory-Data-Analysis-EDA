# 🔎 Books Dataset — Exploratory Data Analysis (EDA)

> Before you chart it, before you model it — you ask it questions. This is that step.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 🗂️ What is this?

This project is **Task 2** of the **CodeAlpha Data Analytics Internship**. It's the middle chapter in a three-part series: after [scraping 1,000 books](https://github.com/bsurendrareddy1114-source/codealpha_Web-Scraping-) and before [visualizing them](https://github.com/bsurendrareddy1114-source/codealpha_Data-Visualization), this notebook sits down with the raw numbers and interrogates them — structure, quality, and the relationships hiding underneath.

No charts here. Just clean, deliberate questioning of the data.

## ❓ The Questions Driving the Analysis

The whole notebook is framed around five core questions:

1. How many books are available in the dataset?
2. What is the average price of books?
3. Which rating appears most frequently?
4. Are there any missing or duplicate records?
5. Does book rating affect book price?

## 🧭 What it does

1. **Load** the cleaned dataset from the Web Scraping task
2. **Inspect structure** — shape, column types, non-null counts
3. **Summarize statistically** — mean, min, max, std across price
4. **Audit data quality** — checks for missing values and duplicate rows
5. **Break down ratings** — frequency of each star rating
6. **Surface key insights** — total books, price extremes, rating distribution

## 📊 Findings at a Glance

| Question | Answer |
|---|---|
| Total books in the dataset | **1,000** |
| Average price | **£35.07** |
| Most frequent rating | **One star** (226 books) |
| Missing values | **None significant** |
| Duplicate records | **Checked and verified** |
| Price range | **£10.00 – £59.99** |

## 🔍 Key Insights

- The dataset is complete and consistent — no meaningful missing data or unresolved duplicates, which meant the analysis could proceed straight to interpretation without extra cleanup.
- **One-star** ratings are the single most common in the dataset, ahead of every other rating tier — a quirk of this being demo/mock data rather than real customer reviews.
- Price spread is wide (roughly £10 to £60) with no single price point dominating, suggesting rating and price aren't strongly tied together in this catalogue.

## 🛠️ Tech Stack

| Tool | Role |
|---|---|
| `pandas` | Structural inspection, statistics, and quality checks |
| `matplotlib` | Imported for continuity with the visualization stage |

## 📁 Project Structure

```
├── Task2.ipynb                    # Full notebook: structure → quality checks → insights
├── books_dataset_cleaned.csv      # Cleaned dataset (from the Web Scraping task)
└── Screenshot *.png                # Output snapshots from the notebook run
```

## 🚀 Getting Started

**1. Clone the repo**
```bash
git clone https://github.com/bsurendrareddy1114-source/codealpha_Exploratory-Data-Analysis-EDA.git
cd codealpha_Exploratory-Data-Analysis-EDA
```

**2. Install dependencies**
```bash
pip install pandas matplotlib jupyter
```

**3. Update the dataset path**

The notebook currently points to a local Windows path — swap it for the CSV in this repo before running:
```python
df = pd.read_csv("books_dataset_cleaned.csv")
```

**4. Run the notebook**
```bash
jupyter notebook Task2.ipynb
```

## 🎯 Skills Demonstrated

- Framing an analysis around clear, answerable questions
- Dataset structure inspection (`.info()`, `.describe()`, `.shape`)
- Data quality auditing — nulls and duplicates
- Descriptive statistics and grouped frequency analysis
- Translating raw output into plain-language insight

## 🙌 Acknowledgements

Built during the **CodeAlpha Data Analytics Internship**, using the cleaned dataset from the companion [Web Scraping project](https://github.com/bsurendrareddy1114-source/codealpha_Web-Scraping-). Its findings feed directly into the [Data Visualization project](https://github.com/bsurendrareddy1114-source/codealpha_Data-Visualization).

---

*If you found this useful, consider ⭐ starring the repo!*
