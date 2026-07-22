# CDC Diabetes Health Indicators – Data Preprocessing & Model Building

## Overview

This project presents a comprehensive workflow for **data preprocessing, exploratory data analysis (EDA), machine learning, ensemble learning, and deep learning** using the **CDC Diabetes Health Indicators** dataset from the **UCI Machine Learning Repository**.

The project focuses on preparing the dataset for predictive modeling through data cleaning, feature analysis, preprocessing, model development, hyperparameter tuning, and performance evaluation. Multiple machine learning algorithms and an Artificial Neural Network (ANN) were implemented and compared to identify the best-performing model for diabetes prediction.

**Dataset Source:** https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators

---

# Project Structure

## 1. Libraries
- Import required Python libraries
- Configure visualization settings

---

## 2. Reading Data
- Load the dataset using Pandas
- Inspect dataset shape
- Display feature names
- Examine data types
- Generate descriptive statistics

---

# Dataset Features

The dataset consists of **22 attributes**, including **21 predictor variables** and **1 target variable**, describing demographic, lifestyle, and health-related factors associated with diabetes.

| Feature | Description |
|---------|-------------|
| **Diabetes_012** | Target variable indicating diabetes status (0 = No Diabetes, 1 = Prediabetes, 2 = Diabetes). |
| **HighBP** | Indicates whether the individual has high blood pressure (0 = No, 1 = Yes). |
| **HighChol** | Indicates whether the individual has high cholesterol (0 = No, 1 = Yes). |
| **CholCheck** | Indicates whether cholesterol has been checked within the last five years (0 = No, 1 = Yes). |
| **BMI** | Body Mass Index of the individual. |
| **Smoker** | Indicates whether the individual has smoked at least 100 cigarettes in their lifetime (0 = No, 1 = Yes). |
| **Stroke** | Indicates whether the individual has ever had a stroke (0 = No, 1 = Yes). |
| **HeartDiseaseorAttack** | Indicates history of coronary heart disease or heart attack (0 = No, 1 = Yes). |
| **PhysActivity** | Indicates whether the individual participated in physical activity during the past 30 days (0 = No, 1 = Yes). |
| **Fruits** | Indicates regular fruit consumption (0 = No, 1 = Yes). |
| **Veggies** | Indicates regular vegetable consumption (0 = No, 1 = Yes). |
| **HvyAlcoholConsump** | Indicates heavy alcohol consumption (0 = No, 1 = Yes). |
| **AnyHealthcare** | Indicates whether the individual has any form of healthcare coverage (0 = No, 1 = Yes). |
| **NoDocbcCost** | Indicates whether medical care was not sought due to cost (0 = No, 1 = Yes). |
| **GenHlth** | Self-reported general health (1 = Excellent, 2 = Very Good, 3 = Good, 4 = Fair, 5 = Poor). |
| **MentHlth** | Number of mentally unhealthy days during the past 30 days (0–30). |
| **PhysHlth** | Number of physically unhealthy days during the past 30 days (0–30). |
| **DiffWalk** | Indicates serious difficulty walking or climbing stairs (0 = No, 1 = Yes). |
| **Sex** | Gender of the individual (0 = Female, 1 = Male). |
| **Age** | Age group represented as ordinal categories (1–13). |
| **Education** | Highest level of education completed (1–6). |
| **Income** | Annual household income represented as ordinal categories (1–8). |

---

# Exploratory Data Analysis (EDA)

### Histogram Analysis
- Visualize numerical feature distributions
- Analyze skewness of continuous and count variables
- Identify data distribution patterns

### Box Plot Analysis
- Detect potential outliers
- Analyze spread of numerical features

### Correlation Analysis
- Generate a correlation heatmap
- Examine relationships among predictor variables
- Identify potential multicollinearity

---

# Data Preprocessing

## Data Cleaning

- Missing value analysis
- Duplicate detection and removal
- Outlier analysis using box plots

## Data Transformation

### Encoding
- Verified categorical feature encoding
- No additional encoding required

### Scaling
- Applied Min-Max Scaling to the BMI feature

### Feature Selection
- Computed Mutual Information scores to identify important features for diabetes prediction

---

# Machine Learning Models

The following machine learning models were implemented:

- Logistic Regression
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)

---

# Validation Techniques

The following validation techniques were used:

- Train-Test Split
- 5-Fold Cross Validation

---

# Hyperparameter Tuning

The following tuning techniques were applied:

- GridSearchCV
- RandomizedSearchCV

Each machine learning model was tuned using its respective estimator.

---

# Ensemble Models

Bagging classifiers were implemented using:

- Logistic Regression
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)

---

# Deep Learning Model

A Deep Learning model was developed using:

- Artificial Neural Network (ANN)

The ANN model was trained and compared with the best-performing machine learning models.

---

# Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- Weighted F1-Score

The final comparison included:

- Baseline Logistic Regression
- Tuned Decision Tree
- Bagging KNN
- Artificial Neural Network (ANN)

Among all evaluated models, the **Artificial Neural Network (ANN)** achieved the best overall performance.

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
  - Logistic Regression
  - Decision Tree Classifier
  - K-Nearest Neighbors
  - GridSearchCV
  - RandomizedSearchCV
  - KFold Cross Validation
  - BaggingClassifier
  - MinMaxScaler
  - Mutual Information Classifier
- TensorFlow
- Keras
- Google Colab

---

# Instructions to Run the Project

1. Clone this repository.
2. Open the notebook in **Google Colab**.
3. Upload the dataset (`diabetes_012_health_indicators_BRFSS2015.csv`).
4. Run the notebook cells sequentially.
5. The notebook performs:
   - Data preprocessing
   - Exploratory Data Analysis
   - Machine Learning model training
   - Hyperparameter tuning
   - Ensemble learning
   - Deep Learning (ANN)
   - Model evaluation and comparison

---

# Contributors

| Team Member | Contribution |
|-------------|--------------|
| **Govind** | Data transformation, feature scaling, Logistic Regression model, K-Fold Cross Validation, GridSearchCV, RandomizedSearchCV, Bagging using Logistic Regression, and final model comparison. |
| **Namitha** | Missing value analysis, duplicate removal, outlier analysis, Decision Tree model, K-Fold Cross Validation, GridSearchCV, RandomizedSearchCV, Bagging using Decision Tree, and Artificial Neural Network (ANN). |
| **Aathil** | Dataset loading, initial exploration, K-Nearest Neighbors (KNN) model, K-Fold Cross Validation, GridSearchCV, RandomizedSearchCV, and Bagging using KNN. |
| **Abhishek** | Data visualization, histogram analysis, box plot analysis, correlation analysis, and Mutual Information feature importance analysis. |

---

# Repository Structure

```text
CDC_Diabetes_Preprocessing_Model_Building/
│
├── CDC_Diabetes_Preprocessing_Model_Building.ipynb
├── diabetes_012_health_indicators_BRFSS2015.csv
├── README.md
└── LICENSE
```

---

# Dataset Source

**CDC Diabetes Health Indicators Dataset**

UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators
