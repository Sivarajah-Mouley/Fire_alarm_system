# Fire Alarm Detection System using Machine Learning

This project focuses on developing a machine learning-based predictive model for fire alarm detection. It addresses key challenges like improving detection accuracy and reducing false alarms using classification models.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Development](#model-development)
- [Performance Evaluation](#performance-evaluation)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [Project Files](#project-files)

## Introduction

This project aims to enhance the reliability and accuracy of fire alarm systems by leveraging machine learning techniques. We trained two models, Random Forest and Support Vector Machine (SVM), to predict fire alarm activation and reduce false alarms.

## Dataset

The dataset used for training the models was obtained from Kaggle, containing 16 columns and over 60,000 rows. The features include air temperature, humidity, CO2 concentration, and particulate matter levels. The target variable is whether a fire alarm is activated (`1`) or not (`0`).

## Data Preprocessing

The preprocessing steps included:
- Removing irrelevant features based on correlation analysis.
- Handling class imbalance using the **Synthetic Minority Over-sampling Technique (SMOTE)**.
- Scaling the numerical features using the Standard Scaler.
- Splitting the data into 80% training and 20% testing sets.

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) provided insights into the relationships between various features and their impact on fire alarm activation. Visualization techniques such as bar charts and box plots were used to identify patterns and outliers.

## Model Development

We used **Random Forest** and **SVM** classifiers for model development. Hyperparameter tuning was conducted using grid search to optimize the performance of both models.

## Performance Evaluation

The models were evaluated using the following metrics:
- **Accuracy**: Random Forest (0.9827), SVM (0.9834)
- **Precision**: Random Forest (1.0), SVM (0.9809)
- **Recall**: Random Forest (0.9758), SVM (0.9961)
- **F1 Score**: Random Forest (0.9877), SVM (0.9885)

The Random Forest model achieved slightly better recall, while the SVM model showed higher precision. The confusion matrix and ROC curve analysis further validated the models' performance.

## Conclusion

This project demonstrates how machine learning can significantly improve the reliability of fire alarm systems. Both models performed well, with potential real-world applications in reducing false alarms and ensuring faster response times during genuine fire incidents.

## How to Run

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/fire-alarm-ml.git
    ```

2. Navigate to the project folder:
    ```bash
    cd fire-alarm-ml
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Jupyter notebook:
    ```bash
    jupyter notebook Fire_Alarm_Smoke_Detection.ipynb
    ```

## Project Files

- `Fire_Alarm_Smoke_Detection.ipynb`: Jupyter notebook containing the full analysis and model development.
- `requirements.txt`: List of Python packages required to run the project.
- `dataset/`: Folder containing the dataset used for training.
