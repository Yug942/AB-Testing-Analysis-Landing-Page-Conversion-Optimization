# 📊 A/B Testing Analysis: Landing Page Conversion Optimization

## 📌 Project Overview

This project analyzes an A/B testing experiment to evaluate whether a **new landing page** improves user conversion rates compared to the **existing landing page**.

The project follows an end-to-end data analytics workflow, including data cleaning, exploratory data analysis (EDA), statistical hypothesis testing, and business decision-making.

---

## 🎯 Business Problem

A company introduced a new landing page and wanted to determine whether it increases user conversions compared to the existing landing page.

**Objective:** Determine if the new landing page should replace the existing one based on statistical evidence.

---

## 📂 Dataset

The dataset contains user-level A/B testing data with the following features:

| Column | Description |
|---------|-------------|
| `user_id` | Unique identifier for each user |
| `timestamp` | Time of user interaction |
| `group` | Experiment group (control/treatment) |
| `landing_page` | Page shown to the user |
| `converted` | Whether the user converted (1 = Yes, 0 = No) |

- Initial Dataset Size: **294,478 rows**
- Final Cleaned Dataset: **288,540 rows**

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

---

# 🧹 Data Cleaning

The following preprocessing steps were performed:

- ✅ Checked for missing values
- ✅ Removed duplicate users (3,894 duplicates)
- ✅ Removed mismatched experiment records
- ✅ Validated experiment integrity

Final Dataset Shape:

```
288,540 rows × 5 columns
```

---

# 📊 Exploratory Data Analysis

## Experiment Distribution

| Group | Users |
|--------|-------:|
| Control | 144,226 |
| Treatment | 144,314 |

The experiment was evenly randomized (~50% users in each group).

---

## Landing Page Distribution

| Landing Page | Users |
|--------------|-------:|
| Old Page | 144,226 |
| New Page | 144,314 |

---

## Conversion Rate

| Group | Conversion Rate |
|--------|----------------:|
| Control (Old Page) | **12.03%** |
| Treatment (New Page) | **11.87%** |

The new landing page showed a slightly lower conversion rate (0.16 percentage points).

---

# 📈 Visualization

### Conversion Rate by Group

> Add your visualization here after uploading the image.

```markdown
![image_alt](https://github.com/user-attachments/assets/a347f166-8d4a-48e7-b307-0aa6d251406b />)
```

---

# 📐 Statistical Hypothesis Testing

## Hypotheses

### Null Hypothesis (H₀)

There is **no significant difference** in conversion rates between the old and new landing pages.

### Alternative Hypothesis (H₁)

There **is a significant difference** in conversion rates between the two landing pages.

---

## Statistical Test

**Chi-Square Test of Independence**

### Results

| Metric | Value |
|--------|------:|
| Chi-Square Statistic | **1.6602** |
| P-value | **0.1976** |
| Significance Level (α) | **0.05** |

---

# 📌 Interpretation

Since

```
p-value = 0.1976 > 0.05
```

we **fail to reject the null hypothesis**.

There is **no statistically significant evidence** that the new landing page performs differently from the existing landing page.

Although the observed conversion rate for the new page is slightly lower, the difference is small enough to be explained by random variation.

---

# 💼 Business Recommendation

Based on the statistical analysis:

- Do **not** replace the existing landing page.
- The new landing page does not provide a statistically significant improvement.
- Consider redesigning the new page and conducting another A/B experiment before deployment.

---

# 📁 Project Structure

```
ab-testing-product-analytics/
│
├── data/
│   └── ab_data.csv
│
├── notebook/
│   └── AB_Testing_Analysis.ipynb
│
├── images/
│   └── conversion_rate.png
│
├── README.md
│
└── requirements.txt
```

---

# 🚀 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- A/B Testing
- Product Analytics
- Conversion Rate Analysis
- Statistical Hypothesis Testing
- Chi-Square Test
- Business Decision Making
- Data Visualization

---

# 📚 Key Learnings

- Cleaned and validated a real-world A/B testing dataset containing over **288,000 user records**.
- Compared conversion performance between control and treatment groups.
- Applied the Chi-Square test to determine statistical significance.
- Converted statistical findings into actionable business recommendations.

---

## ⭐ Repository Highlights

✔ End-to-end A/B Testing Analysis

✔ Real-world Data Cleaning

✔ Statistical Hypothesis Testing

✔ Product Analytics Case Study

✔ Business-Oriented Insights

---

## 📬 Contact

If you have any suggestions or feedback, feel free to connect with me on LinkedIn or reach out through GitHub.
