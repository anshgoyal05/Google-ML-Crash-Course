# 📊 Datasets, Generalization, and Overfitting

This module is part of the Google Machine Learning Crash Course (MLCC). It introduces the fundamentals of preparing datasets, improving model generalization, preventing overfitting, and understanding how model complexity affects performance.

## 📌 Objectives

- Understand the characteristics of a good dataset.
- Learn the importance of high-quality labels.
- Explore the challenges of imbalanced datasets.
- Divide data into training, validation, and test sets.
- Apply data transformations before training.
- Understand generalization and overfitting.
- Learn how model complexity impacts performance.
- Prevent overfitting using L2 regularization.
- Interpret loss curves during model training.

---

## 📖 Dataset Characteristics

A high-quality dataset should be:

- Accurate
- Complete
- Consistent
- Representative of real-world data
- Free from unnecessary duplicates and errors

Well-prepared datasets lead to better machine learning models.

---

## 🏷️ Labels

Labels represent the correct output that a model learns to predict.

Examples:

| Task | Label |
|------|-------|
| Spam Detection | Spam / Not Spam |
| House Price Prediction | House Price |
| Image Classification | Cat / Dog |
| Sentiment Analysis | Positive / Negative |

Incorrect or inconsistent labels reduce model performance.

---

## ⚖️ Imbalanced Datasets

An imbalanced dataset occurs when one class contains significantly more samples than another.

### Example

```text
Fraud Detection

Normal Transactions : 99%
Fraudulent Transactions : 1%
```

### Common Solutions

- Oversampling minority classes
- Undersampling majority classes
- Collecting additional data
- Using class weights during training

---

## ✂️ Dataset Splitting

Datasets are typically divided into three parts:

| Dataset | Purpose |
|----------|----------|
| Training Set | Learn model parameters |
| Validation Set | Tune hyperparameters |
| Test Set | Evaluate final model performance |

Typical split:

- Training: 80%
- Validation: 10%
- Test: 10%

Keeping these datasets separate helps avoid data leakage.

---

## 🔄 Data Transformation

Before training, data is often transformed by:

- Normalization
- Standardization
- Encoding categorical features
- Handling missing values
- Removing duplicates
- Scaling numerical features

These preprocessing steps improve model performance and stability.

---

## 🌍 Generalization

Generalization is the ability of a model to perform well on unseen data.

A model with good generalization:

- Learns meaningful patterns.
- Performs consistently on new datasets.
- Avoids memorizing the training data.

---

## ⚠️ Overfitting

Overfitting occurs when a model learns the training data too closely, including noise and random patterns.

### Characteristics

- Very high training accuracy
- Lower validation and test accuracy
- Poor performance on unseen data

Common causes include:

- Excessively complex models
- Small datasets
- Too many training epochs
- Insufficient regularization

---

## 🧩 Model Complexity

Choosing the right model complexity is essential.

### Underfitting

- Model is too simple.
- Fails to capture important patterns.

### Good Fit

- Learns useful relationships.
- Generalizes well.

### Overfitting

- Model is too complex.
- Memorizes the training data.

The goal is to find a balance between simplicity and complexity.

---

## 🛡️ L2 Regularization

L2 Regularization reduces overfitting by discouraging very large model weights.

Benefits:

- Improves generalization
- Reduces model complexity
- Produces smoother decision boundaries
- Helps prevent memorization of training data

---

## 📈 Interpreting Loss Curves

Loss curves help monitor training progress.

### Healthy Training

- Training loss decreases.
- Validation loss decreases.
- Both curves remain close together.

### Overfitting

- Training loss continues decreasing.
- Validation loss begins increasing.

### Underfitting

- Both training and validation losses remain high.

Monitoring loss curves helps determine when to stop training.

---

## 🎯 Key Takeaways

- High-quality datasets are essential for accurate models.
- Proper labeling directly impacts model performance.
- Dataset imbalance can introduce bias.
- Training, validation, and test sets serve different purposes.
- Data preprocessing improves learning efficiency.
- Good models should generalize well to unseen data.
- Overfitting reduces real-world performance.
- L2 Regularization helps improve generalization.
- Loss curves are valuable for monitoring training behavior.

---

## 🛠️ Technologies Discussed

- Machine Learning
- Data Preprocessing
- Dataset Splitting
- Regularization
- Model Evaluation
- Loss Functions

---

## 📚 Key Learnings

- Dataset Characteristics
- Label Quality
- Imbalanced Datasets
- Train, Validation, and Test Splits
- Data Transformation
- Generalization
- Overfitting
- Model Complexity
- L2 Regularization
- Loss Curve Interpretation

---

## 📁 Files

- `README.md` — Summary of concepts and key learnings for the module.

---

## 📘 Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)
- **Module:** Data
- **Subtopic:** Datasets, Generalization, and Overfitting
