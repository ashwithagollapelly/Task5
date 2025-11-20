.

 Titanic Survival Prediction — Machine Learning Project
Exploratory Data Analysis (EDA) + Feature Engineering + Model Building + Prediction
 Project Overview

This project explores the Titanic dataset to understand survival patterns and build machine-learning models that predict whether a passenger survived the Titanic disaster.
Steps include:

Data cleaning

Exploratory data analysis (EDA)

Feature engineering

Model training & comparison

Predicting survival for new passengers

Generating a summary PDF report

 Dataset

The project uses the classic Titanic dataset, containing:

Demographics (Age, Sex)

Travel details (Class, Fare, Embarked)

Family information (SibSp, Parch)

Survival label (0 = No, 1 = Yes)

 1. Data Preprocessing

Performed before modeling:

Handling missing values

Encoding categorical columns

Scaling numerical features

Adding new features:

FamilySize = SibSp + Parch + 1

AgeGroup (Child, Adult, Senior categories)

 2. Exploratory Data Analysis (EDA)

Analyzed survival patterns using:

Histograms

Countplots

Heatmaps

Pairplots

Boxplots

Key Findings:

Females survived more than males

First-class passengers had higher survival

Younger passengers (children) survived more

Higher fare → higher survival rate

 3. Machine Learning Models Used

Trained and compared 4 models:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

KNN Classifier

Best Model:

Random Forest Classifier
Achieved highest accuracy among all models.

 4. Model Accuracy
Model	Accuracy
Logistic Regression	~0.80
Decision Tree	~0.78
Random Forest	~0.83
KNN	~0.79
 5. Predicting a New Passenger

A sample passenger dictionary is passed to the trained model.
The model predicts:

1 → Survived

0 → Did not survive

Example prediction output:

Survived (1=yes, 0=no): 1

 6. PDF Report

A full PDF report summarizing the analysis is generated:

Introduction

Dataset Information

EDA

Modeling

Results

Conclusion

 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

ReportLab (PDF generation)
 7. Project Structure
Titanic_Project/
│
├── titanics.ipynb        # Main Jupyter Notebook
├── Titanic_Analysis_Report.pdf
├── README.md
└── data/
    └── train.csv

 8. Conclusion

This project demonstrates:

Understanding of data analysis

Strong feature engineering

Multiple machine-learning models

Real prediction capability

Random Forest gave the best accuracy and is recommended for deployment.
