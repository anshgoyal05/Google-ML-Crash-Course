# 🌾 Classification - Rice Variety Prediction

This project is part of the Google Machine Learning Crash Course (MLCC). In this lab, a binary classification model was trained to distinguish between two rice varieties (**Cammeo** and **Osmancik**) using geometric features extracted from rice grain images.

## 📌 Objectives

- Load and explore a real-world classification dataset.
- Visualize relationships between features using 2D and 3D plots.
- Normalize numerical features using Z-score normalization.
- Build and train a binary classification model using TensorFlow/Keras.
- Evaluate model performance using classification metrics.
- Compare models trained with selected features versus all available features.
- Analyze model performance using AUC and ROC-related metrics.

## 📊 Dataset

The dataset contains measurements extracted from images of rice grains.

### Features

| Feature | Description |
|----------|-------------|
| Area | Area of the rice grain |
| Convex_Area | Convex hull area |
| Perimeter | Boundary length of the grain |
| Major_Axis_Length | Length of the major axis |
| Minor_Axis_Length | Length of the minor axis |
| Eccentricity | Shape elongation measure |
| Extent | Ratio of area to bounding box area |

### Target Classes

- Cammeo → 1
- Osmancik → 0

## 🔍 Data Exploration

Key observations from the dataset:

- Multiple features showed clear separation between rice varieties.
- Area, Major Axis Length, and Eccentricity appeared to contain the most useful classification information.
- 2D and 3D visualizations helped identify potential class boundaries.
- Several features were strongly correlated with one another.

## 📈 Feature Engineering

### Data Normalization

All numerical features were normalized using **Z-score normalization**:

```text
Z = (x - mean) / standard deviation
```

This ensured all features were on a similar scale and improved model training stability.

### Dataset Split

The dataset was divided into:

- Training Set: 80%
- Validation Set: 10%
- Test Set: 10%

## 🧪 Experiments

### Experiment 1

Selected Features Model

Features:

- Eccentricity
- Major_Axis_Length
- Area

Hyperparameters:

- Learning Rate: 0.001
- Epochs: 60
- Batch Size: 100
- Classification Threshold: 0.35

### Experiment 2

All Features Model

Features:

- Eccentricity
- Major_Axis_Length
- Minor_Axis_Length
- Area
- Convex_Area
- Perimeter
- Extent

Hyperparameters:

- Learning Rate: 0.001
- Epochs: 60
- Batch Size: 100
- Classification Threshold: 0.50

## 📉 Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- AUC (Area Under the ROC Curve)

### Metric Overview

- **Accuracy** → Overall prediction correctness.
- **Precision** → Percentage of positive predictions that are correct.
- **Recall** → Percentage of actual positives correctly identified.
- **AUC** → Measures classification performance across multiple thresholds.

## 🎯 Results

### Selected Features Model

- Achieved approximately 90%+ accuracy.
- Strong AUC performance.
- Demonstrated that a small set of informative features can perform well.

### All Features Model

- Achieved approximately 92% test accuracy.
- AUC close to 0.98.
- Showed slightly better generalization on unseen data.
- Additional features provided only a small performance improvement.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- TensorFlow
- Keras
- Plotly
- Google Colab

## 📚 Key Learnings

- Binary Classification Fundamentals
- Logistic Regression using Sigmoid Activation
- Data Normalization with Z-Scores
- Feature Selection and Visualization
- Model Evaluation using Accuracy, Precision, Recall, and AUC
- Train/Validation/Test Splitting
- Overfitting Detection and Generalization
- Comparing Multiple Classification Models

## 📁 Files

- `binary_classification_rice.ipynb` — Complete MLCC notebook and experiments.
- `README.md` — Summary of concepts, experiments, and results.

## Course Information

**Course:** Google Machine Learning Crash Course (MLCC)  
**Module:** Classification  
**Author:** Ansh Goyal
📈 Feature Engineering

Data Normalization

All numerical features were normalized using Z-score normalization:

Z = (x - mean) / standard deviation

This ensured all features were on a similar scale and improved model training stability.

Dataset Split

The dataset was divided into:

* Training Set: 80%
* Validation Set: 10%
* Test Set: 10%

🧪 Experiments

Experiment 1

Selected Features Model

Features:

* Eccentricity
* Major_Axis_Length
* Area

Hyperparameters:

* Learning Rate: 0.001
* Epochs: 60
* Batch Size: 100
* Classification Threshold: 0.35

Experiment 2

All Features Model

Features:

* Eccentricity
* Major_Axis_Length
* Minor_Axis_Length
* Area
* Convex_Area
* Perimeter
* Extent

Hyperparameters:

* Learning Rate: 0.001
* Epochs: 60
* Batch Size: 100
* Classification Threshold: 0.50

📉 Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* AUC (Area Under the ROC Curve)

Metric Overview

* Accuracy → Overall prediction correctness.
* Precision → Percentage of positive predictions that are correct.
* Recall → Percentage of actual positives correctly identified.
* AUC → Measures classification performance across multiple thresholds.

🎯 Results

Selected Features Model

* Achieved approximately 90%+ accuracy.
* Strong AUC performance.
* Demonstrated that a small set of informative features can perform well.

All Features Model

* Achieved approximately 92% test accuracy.
* AUC close to 0.98.
* Showed slightly better generalization on unseen data.
* Additional features provided only a small performance improvement.

🛠️ Technologies Used

* Python
* Pandas
* NumPy
* TensorFlow
* Keras
* Plotly
* Google Colab

📚 Key Learnings

* Binary Classification Fundamentals
* Logistic Regression using Sigmoid Activation
* Data Normalization with Z-Scores
* Feature Selection and Visualization
* Model Evaluation using Accuracy, Precision, Recall, and AUC
* Train/Validation/Test Splitting
* Overfitting Detection and Generalization
* Comparing Multiple Classification Models

📁 Files

* binary_classification_rice.ipynb — Complete MLCC notebook and experiments.
* README.md — Summary of concepts, experiments, and results.

Course Information

- **Course:** Google Machine Learning Crash Course (MLCC)
- **Module:** ML Models
- **Subtopic:** Classification

