# 🚕 Linear Regression - Taxi Fare Prediction

This project is part of the **Google Machine Learning Crash Course (MLCC)**. In this lab, a Linear Regression model was trained to predict taxi fares using real-world Chicago taxi trip data.

## 📌 Objectives

- Load and explore a real-world dataset using Pandas.
- Analyze relationships between features and labels.
- Build and train a Linear Regression model.
- Tune hyperparameters such as learning rate and batch size.
- Evaluate model performance using RMSE.
- Generate fare predictions using the trained model.

## 📊 Dataset

The dataset is derived from the Chicago Taxi Trips dataset and includes:

| Feature | Description |
|----------|------------|
| TRIP_MILES | Distance traveled during the trip |
| TRIP_SECONDS | Duration of the trip |
| FARE | Total fare amount |
| COMPANY | Taxi company |
| PAYMENT_TYPE | Payment method |
| TIP_RATE | Percentage tip rate |

## 🔍 Data Exploration

Key observations from the dataset:

- Maximum Fare: **$159.25**
- Average Trip Distance: **8.29 miles**
- Number of Taxi Companies: **31**
- Most Frequent Payment Type: **Credit Card**
- No missing values found

## 📈 Correlation Analysis

Feature correlation with fare:

- **TRIP_MILES** showed the strongest correlation with fare.
- **TRIP_SECONDS** also showed a strong positive correlation.
- **TIP_RATE** showed the weakest correlation.

## 🧪 Experiments

### Experiment 1
Single Feature Model

```python
Feature: TRIP_MILES
Learning Rate: 0.001
Epochs: 20
Batch Size: 50
```

### Experiment 2
Hyperparameter Tuning

- Increased Learning Rate
- Decreased Learning Rate
- Increased Batch Size

### Experiment 3
Two Feature Model

```python
Features:
- TRIP_MILES
- TRIP_MINUTES
```

The two-feature model produced better results than the single-feature model.

## 📉 Evaluation Metrics

The model was evaluated using:

- Root Mean Squared Error (RMSE)
- Loss Curves
- Prediction Comparisons

Lower RMSE values indicate better prediction accuracy.

## 🎯 Results

- The model successfully learned the relationship between trip distance, duration, and fare.
- Adding `TRIP_MINUTES` improved prediction performance.
- Predicted fares were generally close to observed fares.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- TensorFlow
- Keras
- Plotly
- Google Colab

## 📚 Key Learnings

- Fundamentals of Linear Regression
- Feature Selection
- Correlation Analysis
- Hyperparameter Tuning
- Model Evaluation using RMSE
- Making Predictions with Trained Models

## 📁 Files

- `linear_regression_taxi.ipynb` — Complete MLCC notebook and experiments.

---

### Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)  
- **Module:** ML
- **Subtopic:** Linear Regression
