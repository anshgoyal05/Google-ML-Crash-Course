# 🏷️ Working with Categorical Data

This module is part of the Google Machine Learning Crash Course (MLCC). It introduces categorical data, encoding techniques, feature crosses, and best practices for preparing categorical features for machine learning models.

## 📌 Objectives

- Understand what categorical data is.
- Learn how machine learning models process categorical features.
- Convert categorical values into numerical representations using one-hot encoding.
- Understand common challenges associated with categorical data.
- Learn how feature crosses improve model performance.
- Explore practical examples of feature engineering with categorical features.

---

## 📖 Introduction

Categorical data represents values that belong to a fixed set of categories rather than continuous numerical values.

### Examples

| Feature | Categories |
|----------|------------|
| Color | Red, Blue, Green |
| Payment Method | Cash, Card, UPI |
| City | Delhi, Mumbai, Bengaluru |
| Browser | Chrome, Firefox, Safari |

Unlike numerical data, categorical values cannot be directly used by most machine learning algorithms.

---

## 🔠 Vocabulary and One-Hot Encoding

Machine learning models require numerical inputs, so categorical values must be encoded.

### Vocabulary

A vocabulary is the complete list of unique categories present in a feature.

Example:

```text
Color:
Red
Blue
Green
Yellow
```

### One-Hot Encoding

One-hot encoding converts each category into a binary vector.

Example:

| Color | Red | Blue | Green |
|--------|----:|-----:|------:|
| Red | 1 | 0 | 0 |
| Blue | 0 | 1 | 0 |
| Green | 0 | 0 | 1 |

This prevents the model from assuming an incorrect numerical relationship between categories.

---

## ⚠️ Common Issues with Categorical Data

Some common challenges include:

- High-cardinality features (too many unique values)
- Missing or unknown categories
- Rare categories with very few examples
- Increased dimensionality after one-hot encoding
- Memory and computational overhead

Proper preprocessing helps improve model performance and generalization.

---

## 🔀 Feature Crosses

A feature cross combines two or more features into a single feature to capture interactions between them.

### Example

Instead of using:

- Age
- Occupation

A crossed feature may be:

```text
Age × Occupation
```

This enables the model to learn relationships that individual features cannot represent on their own.

---

## 🚀 Benefits of Feature Crosses

- Capture interactions between features.
- Improve prediction accuracy.
- Learn more complex decision boundaries.
- Enhance feature engineering for linear models.

---

## 🎯 Key Takeaways

- Categorical data represents labels or categories rather than numeric values.
- Machine learning models require categorical data to be encoded.
- One-hot encoding is one of the most common encoding techniques.
- Large vocabularies can increase model complexity.
- Feature crosses help models learn interactions between multiple features.
- Proper feature engineering can significantly improve model performance.

---

## 🛠️ Technologies Discussed

- Machine Learning
- Feature Engineering
- One-Hot Encoding
- Feature Crosses
- Categorical Feature Processing

---

## 📚 Key Learnings

- Understanding Categorical Data
- Vocabulary Creation
- One-Hot Encoding
- Handling High-Cardinality Features
- Feature Engineering
- Feature Crosses
- Data Preprocessing Best Practices

---

## 📁 Files

- `README.md` — Summary of concepts and key learnings for the module.

---

## 📘 Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)
- **Module:** Data
- **Subtopic:** Working with Categorical Data
