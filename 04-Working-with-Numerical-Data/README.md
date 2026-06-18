# 🔢 Working with Numerical Data

This module is part of the Google Machine Learning Crash Course (MLCC). It focuses on understanding numerical datasets, identifying outliers, analyzing statistical distributions, and detecting bad or inconsistent data using both statistical and visual techniques.

## 📌 Objectives

- Explore numerical datasets using descriptive statistics.
- Understand measures such as mean, median, standard deviation, and percentiles.
- Identify potential outliers in datasets.
- Visualize data using scatter plots.
- Detect hidden data quality issues.
- Compare statistical analysis with visual inspection.
- Learn how bad data can impact machine learning models.

---

## 📊 Exercise 1: Statistics on a Dataset

### Dataset

The exercise used the California Housing dataset containing features such as:

- Total Rooms
- Total Bedrooms
- Population
- Households
- Median Income

### Key Analysis

Using the `describe()` function, the following statistics were analyzed:

- Count
- Mean
- Standard Deviation
- Minimum Value
- Quartiles (25%, 50%, 75%)
- Maximum Value

### Outlier Detection

Potential outliers were identified by comparing:

- Mean vs Standard Deviation
- 75th Percentile vs Maximum Value
- Distribution spread across numerical features

### Findings

Possible outlier columns:

- Total Rooms
- Total Bedrooms
- Population
- Households
- Median Income

Indicators:

- Standard deviation was nearly as large as the mean.
- Maximum values were significantly larger than the upper quartile.
- Data distributions appeared heavily skewed.

---

## 📈 Exercise 2: Finding Bad Values in a Dataset

### Dataset

A synthetic dataset containing:

| Feature | Description |
|----------|-------------|
| Calories | Number of breakfast calories consumed |
| Test Score | Student math test score |

Dataset characteristics:

- 1,400 records
- 50 students
- 28 consecutive days of observations

### Initial Statistical Analysis

The basic statistics suggested:

- No obvious outliers
- Standard deviations were much smaller than means
- Quartile ranges appeared balanced

This demonstrated that bad data is not always visible through summary statistics alone.

---

## 📉 Data Visualization

Scatter plots were used to visualize:

- Calories vs Test Score

Key observation:

- A cluster of unusual points appeared with:
  - Very low calorie values
  - Unexpectedly high test scores

These points became more noticeable as more data points were plotted.

---

## 🔍 Investigating Data Quality Issues

### Weekly Analysis

Data was grouped by week and analyzed separately.

Results:

- Weekly statistics were very similar.
- No significant differences were found between weeks.

### Daily Analysis

Data was then grouped by day.

Results:

- Day 4 showed a significantly different calorie range.
- Most days contained calorie values between 0 and 400.
- Day 4 contained calorie values between 0 and 200.

This suggested a data encoding or measurement issue.

---

## 🎯 Key Findings

- Summary statistics alone may fail to reveal hidden data problems.
- Visualization is essential for detecting unusual patterns.
- Outliers can be identified through both statistical and graphical methods.
- Data inconsistencies may result from measurement or encoding errors.
- Investigating subsets of data can help locate problematic records.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Google Colab

---

## 📚 Key Learnings

- Descriptive Statistics
- Mean, Median, and Standard Deviation
- Percentiles and Quartiles
- Outlier Detection
- Data Visualization
- Scatter Plot Analysis
- Data Quality Assessment
- Identifying Encoding Errors
- Exploratory Data Analysis (EDA)

---

## 📁 Files

- `numerical_data_stats.ipynb` — Statistical analysis and outlier detection.
- `numerical_data_bad_values.ipynb` — Identifying hidden bad values using visualization and statistical analysis.
- `README.md` — Summary of concepts, experiments, and findings.

---

## 📘 Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)
- **Module:** Data
- **Subtopic:** Working with Numerical Data
