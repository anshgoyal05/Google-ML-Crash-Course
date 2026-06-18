# 📈 Logistic Regression

This module is part of the Google Machine Learning Crash Course (MLCC). It introduces Logistic Regression, a supervised machine learning algorithm used for binary classification problems.

## 📌 Objectives

- Understand the purpose of Logistic Regression.
- Learn how probabilities are calculated for classification tasks.
- Understand the sigmoid function.
- Learn about loss functions used in classification.
- Explore regularization techniques to reduce overfitting.
- Understand decision thresholds and classification outcomes.

## 🧠 Concepts Covered

### 1. Introduction to Logistic Regression

Logistic Regression is a classification algorithm used to predict the probability that an input belongs to a particular class.

Examples:

- Email → Spam or Not Spam
- Transaction → Fraudulent or Legitimate
- Student → Pass or Fail

Unlike Linear Regression, Logistic Regression outputs probabilities between **0 and 1**.

---

### 2. Calculating a Probability

Logistic Regression uses the **Sigmoid Function** to convert model outputs into probabilities.

#### Sigmoid Function

```text id="kl5n2s"
P(y=1) = 1 / (1 + e^(-z))
```

Where:

```text id="r3pw7v"
z = w₁x₁ + w₂x₂ + ... + b
```

The output is always between 0 and 1.

Example:

- Probability = 0.90 → Positive Class
- Probability = 0.15 → Negative Class

---

### 3. Classification Threshold

A threshold determines the final prediction.

Common threshold:

```text id="pq1wzx"
0.5
```

Rules:

- Probability ≥ 0.5 → Positive Class
- Probability < 0.5 → Negative Class

Different thresholds affect Precision and Recall.

---

### 4. Loss Function

Logistic Regression uses **Log Loss (Binary Cross-Entropy)** instead of Mean Squared Error.

Purpose:

- Penalizes incorrect predictions.
- Encourages accurate probability estimates.
- Produces better classification performance.

Lower loss values indicate better model performance.

---

### 5. Regularization

Regularization helps prevent overfitting.

#### L1 Regularization (Lasso)

- Encourages sparse models.
- Can eliminate less important features.

#### L2 Regularization (Ridge)

- Reduces excessively large weights.
- Produces smoother models.

Benefits:

- Better generalization
- Reduced overfitting
- Improved performance on unseen data

---

## 📊 Key Terms

| Term | Description |
|--------|------------|
| Sigmoid Function | Converts outputs into probabilities |
| Threshold | Decision boundary for classification |
| Log Loss | Measures classification error |
| Regularization | Prevents overfitting |
| Probability | Likelihood of belonging to a class |

---

## 🎯 Real-World Applications

- Spam Detection
- Fraud Detection
- Medical Diagnosis
- Customer Churn Prediction
- Credit Risk Assessment
- Sentiment Analysis

---

## 📚 Key Learnings

- Logistic Regression is used for binary classification.
- The sigmoid function converts predictions into probabilities.
- Classification decisions depend on thresholds.
- Log Loss is the preferred loss function for classification tasks.
- Regularization helps improve model generalization.
- Logistic Regression serves as a strong baseline model for many classification problems.

---

## 🛠️ Technologies Discussed

- Machine Learning
- Logistic Regression
- Binary Classification
- Sigmoid Function
- Cross-Entropy Loss
- Regularization (L1 & L2)

---

## Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)  
- **Module:** ML
- **Subtopic:** Logistic Regression
