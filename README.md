![logo](https://github.com/user-attachments/assets/ac1eda16-88d0-405b-a8dd-2c902c7995ab)

# Airline Customer Satisfaction Predictor: A Machine Learning Model for Predicting Customer Satisfaction

1. [Introduction](#introduction-)
2. [Description](#description-)
3. [Installation](#installation-)
4. [Contact](#contact-)
5. [Sidenotes](#sidenotes-)

## Introduction 📝
This project is about predicting customer satisfaction regarding their flight experience which is affected by numerous features. Some of these features include basic information such as age and class, however, there are more specific features that detail the flight experience such as departure and arrival delays, legroom service, Flight distance, and many more.    

**Technologies and Concepts used**
1. Python for building and implementing machine learning models.
2. Skicit-learn used for data preprocessing, feature selection, and implementing machine learning
3. Matplotlib and Seaborn for data visualizations
4. LightGBM and Decision Tree for the Machine Learning models
5. Streamlit for ML deployment
6. Joblib for saving and loading machine learning models efficiently.


## Description 🎯
**EDA** (Below are examples of the EDA performed and its results)
![heatmap](https://github.com/user-attachments/assets/0c1b6e03-3854-4c8b-bcd2-b324e9e2384e)

Correlation Heatmap Summary
The heatmap highlights key correlations in the dataset:

Positive Correlations:

"Ease of Online Booking" and "Online Boarding" (0.71).
"Class" (0.49) and "Loyal Customer" (0.39) strongly influence satisfaction.
"Inflight Entertainment" and "Inflight Service" (0.61).
Minimal Impact:

Delays show negligible correlation with satisfaction (-0.01 to -0.02).

![sample](https://github.com/user-attachments/assets/6cf69aa2-e0be-46ab-a4fb-d39d3b458769)

Flight Distance Data Analysis
The data is right-skewed, with most flights under 1000 units.
The boxplot highlights a compact range for typical flights and several outliers beyond 4000 units, representing long-haul flights.
Most flights are short, with a small number of extremely long-distance flights.

**Preprocessing**

![smote](https://github.com/user-attachments/assets/a5130e7a-e7ee-458d-9d89-ead0ac586b93)
![SMOT2](https://github.com/user-attachments/assets/7648e631-55a4-4c3e-a632-d34eec6fc572)

The images above showcase SMOTE being used to handle class imbalance.

**MACHINE LEARNING**

![dec1](https://github.com/user-attachments/assets/1d58ab07-89b7-4a00-9eed-ac40234f9506)
![dec2](https://github.com/user-attachments/assets/e81857b2-b4db-4f20-b656-91f89cd49efc)

Training vs Test Performance:

The model performs slightly better on the training set (86% accuracy) than on the test set (82%), indicating minor overfitting.
Class Imbalance Handling:

High recall for class 1 (positive class) indicates strong performance in identifying positives.
Lower recall for class 0 (negative class) on both sets highlights the difficulty in detecting all negative cases.
Precision and Recall Trade-Off:

Precision for class 1 drops on the test set (0.71), suggesting more false positives on unseen data.


**Feature importance**

![FEATURE](https://github.com/user-attachments/assets/8323ec71-ea96-4b67-bbc9-32bed9fe1a5f)

Acquire top 10 features that affect customer satisfaction, which can be used to fine-tune models further.



















## Installation ⚙️

**Clone the repo**
```bash
git clone https://github.com/jaylesmajor/Classification-ML-Deployment
```

## Contact 📧
Jayles Escolar - jayles.escolar@yahoo.com

Project link: https://github.com/jaylesmajor/Classification-ML-Deployment

## Sidenotes
1. Local deployment using Streamlit works perfectly, however, using StreamliT Cloud will cause an error due to SHAP****
