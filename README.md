# diabetes_prediction_ISI
# Diabetes Prediction Using Machine Learning Classification Models

## Overview

This project focuses on predicting whether a patient is diabetic or non-diabetic using Machine Learning classification algorithms. The implementation utilizes the **Pima Indians Diabetes Dataset** and compares the performance of multiple classification models through various evaluation metrics.

The project was developed as part of the **IDEAS Summer Internship Program 2026** to demonstrate the application of supervised machine learning techniques in healthcare analytics and disease prediction.

---

## Problem Statement

Diabetes is a chronic metabolic disorder that affects millions of people worldwide. Early detection of diabetes can help healthcare professionals initiate timely treatment and reduce the risk of severe complications.

The objective of this project is to build predictive models that can classify patients as diabetic or non-diabetic based on medical diagnostic measurements.

---

## Dataset

### Pima Indians Diabetes Dataset

The dataset contains diagnostic information collected from female patients and includes the following features:

| Feature                  | Description                                      |
| ------------------------ | ------------------------------------------------ |
| Pregnancies              | Number of pregnancies                            |
| Glucose                  | Plasma glucose concentration                     |
| BloodPressure            | Diastolic blood pressure                         |
| SkinThickness            | Triceps skin fold thickness                      |
| Insulin                  | 2-Hour serum insulin                             |
| BMI                      | Body Mass Index                                  |
| DiabetesPedigreeFunction | Genetic influence factor                         |
| Age                      | Age of patient                                   |
| Outcome                  | Target variable (0 = Non-Diabetic, 1 = Diabetic) |

### Dataset Statistics

* Total Records: 768
* Features: 8
* Target Classes: 2
* Classification Type: Binary Classification

---

## Project Workflow

### 1. Data Loading and Inspection

* Loaded dataset using Pandas
* Inspected dataset dimensions
* Checked for missing values
* Generated descriptive statistics

### 2. Data Preprocessing

* Feature and target separation
* Train-test split (80:20)
* Stratified sampling
* Feature standardization using StandardScaler

### 3. Model Development

The following machine learning models were implemented:

#### Logistic Regression

A probabilistic linear classifier widely used for binary classification tasks.

#### K-Nearest Neighbors (KNN)

A distance-based classification algorithm that predicts class labels using neighboring samples.

#### Support Vector Machine (SVM)

A powerful classifier that identifies an optimal hyperplane for class separation.

---

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Results

| Model               | Accuracy     | Precision    | Recall   | F1-Score     |
| ------------------- | ------------ | ------------ | -------- | ------------ |
| Logistic Regression | 0.714286     | 0.608696     | 0.518519 | 0.560000     |
| KNN                 | 0.701299     | 0.583333     | 0.518519 | 0.549020     |
| SVM                 | **0.720779** | **0.622222** | 0.518519 | **0.565657** |

### Best Performing Model

**Support Vector Machine (SVM)** achieved the highest overall performance among the evaluated classifiers.

---

## Confusion Matrix Analysis

The performance of each model was further analyzed using confusion matrices:

* Logistic Regression Confusion Matrix
* KNN Confusion Matrix
* SVM Confusion Matrix

These visualizations provide insights into:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Matplotlib
* Jupyter Notebook

---

## Repository Structure

```text
Diabetes-Prediction/
│
├── diabetes.csv
├── Diabetes_Prediction.ipynb
├── README.md
│
├── figures/
│   ├── lr_confusion_matrix.png
│   ├── knn_confusion_matrix.png
│   └── svm_confusion_matrix.png
│
└── report/
    └── Diabetes_Prediction_Report.pdf
```

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Diabetes-Prediction.git
```

### Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib
```

### Run Notebook

```bash
jupyter notebook
```

Open:

```text
Diabetes_Prediction.ipynb
```

and execute all cells sequentially.

---

## Key Learning Outcomes

* Data preprocessing and feature scaling
* Binary classification using machine learning
* Model evaluation and comparison
* Performance analysis using confusion matrices
* Application of machine learning in healthcare analytics

---

## Future Improvements

* Hyperparameter tuning using Grid Search
* Random Forest implementation
* XGBoost classifier
* ROC-AUC analysis
* Deep Learning-based prediction models
* Web application deployment using Flask or Streamlit

---

## Author

**Swapnil Banerjee**

Summer Internship Program 2026

Institute of Data Engineering, Analytics and Science Foundation (IDEAS)

---

## License

This project is intended for academic and educational purposes.
