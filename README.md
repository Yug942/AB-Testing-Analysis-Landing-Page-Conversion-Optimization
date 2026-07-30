📊 A/B Testing Analysis: Landing Page Conversion Optimization


📌 Project Overview

This project analyzes an A/B testing experiment conducted to determine whether a new landing page improves user conversion rates compared to the existing landing page.

The analysis follows a complete data analytics workflow:

Data cleaning
Exploratory Data Analysis (EDA)
Data validation
Conversion rate analysis
Statistical hypothesis testing (Chi-square Test)
Business recommendation
🎯 Business Problem

A company introduced a new landing page and wanted to determine whether it leads to higher user conversions than the existing landing page.

The goal of this project is to answer:

Should the company replace the existing landing page with the new one based on experimental data?

📂 Dataset

The dataset contains user-level A/B testing data with the following columns:

Column	Description
user_id	Unique identifier for each user
timestamp	Time of user interaction
group	Experiment group (control or treatment)
landing_page	Page shown (old_page or new_page)
converted	Whether the user converted (1 = Yes, 0 = No)

Initial dataset size:

294,478 records

Final cleaned dataset:

288,540 records
🧹 Data Cleaning

The following preprocessing steps were performed:

✅ Checked missing values

No missing values were found.

✅ Removed duplicate users
Duplicate users detected: 3,894
Retained only the first occurrence of each user.
✅ Removed inconsistent experiment records

Rows where:

Control users viewed the new page
Treatment users viewed the old page

were removed to maintain experiment integrity.

Final dataset:

288,540 rows × 5 columns
📊 Exploratory Data Analysis
Group Distribution
Group	Users
Control	144,226
Treatment	144,314

The experiment was evenly randomized (~50% in each group).

Landing Page Distribution
Landing Page	Users
Old Page	144,226
New Page	144,314
Conversion Rates
Group	Conversion Rate
Control (Old Page)	12.03%
Treatment (New Page)	11.87%

The observed difference is:

0.16 percentage points

Although the old page shows a slightly higher conversion rate, statistical testing is required to determine whether this difference is meaningful.

📈 Visualization

A bar chart was created to compare conversion rates between the control and treatment groups.

(Add your chart image here once uploaded.)

Example:

images/conversion_rate.png
📐 Statistical Analysis
Hypothesis
Null Hypothesis (H₀)

The conversion rates of the old and new landing pages are equal.

Alternative Hypothesis (H₁)

The conversion rates are different.

Statistical Test

Chi-square Test of Independence

Results
Metric	Value
Chi-square Statistic	1.6602
P-value	0.1976
Significance Level	0.05
📌 Conclusion

Since:

P-value = 0.1976 > 0.05

we fail to reject the null hypothesis.

There is no statistically significant evidence that the new landing page performs differently from the old landing page.

Although the observed conversion rate of the new page is slightly lower, the difference can reasonably be explained by random variation.

💼 Business Recommendation

Based on the statistical analysis:

Do not replace the current landing page.
The new landing page does not demonstrate a statistically significant improvement in conversions.
Consider redesigning the new page or conducting another experiment with additional changes.
🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
SciPy
📁 Project Structure
AB-Testing-Analysis/
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
📚 Skills Demonstrated
Data Cleaning
Exploratory Data Analysis (EDA)
Data Validation
Statistical Hypothesis Testing
Chi-square Test
A/B Testing
Conversion Rate Analysis
Business Decision Making
Product Analytics
🚀 Key Takeaways
Cleaned and validated an A/B testing dataset containing over 288,000 user records.
Evaluated conversion performance between control and treatment groups.
Applied the Chi-square hypothesis test to assess statistical significance.
Translated statistical findings into actionable business recommendations.
