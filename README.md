## Titanic Survival Prediction using Machine Learning with Python

# Titanic Survival Prediction using Machine Learning with Python

## Project Overview

This project aims to predict whether a passenger survived the Titanic disaster using machine learning techniques. The project involves data preprocessing, exploratory data analysis (EDA), feature engineering, model building, evaluation, and comparison of multiple machine learning algorithms.

## Objective

The objective of this project is to develop a machine learning model that predicts passenger survival based on features such as passenger class, age, gender, fare, family size, and embarkation port.

## Dataset

* **Dataset:** Titanic Dataset
* **Source:** Kaggle Titanic Dataset
* **Total Records:** 891
* **Features:** 12 (before feature engineering)
* **Target Variable:** Survived

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## Exploratory Data Analysis (EDA)

The following analyses were performed:

* Dataset overview
* Missing value analysis
* Data cleaning and preprocessing
* Survival distribution
* Gender vs Survival
* Passenger Class vs Survival
* Age vs Survival
* Fare vs Survival
* SibSp vs Survival
* Parch vs Survival
* Embarked vs Survival
* Correlation Heatmap
* Outlier Analysis

## Data Preprocessing

* Filled missing values in the **Age** column using the median.
* Filled missing values in the **Embarked** column using the mode.
* Excluded the **Cabin** column due to a large number of missing values.
* Encoded categorical variables using Label Encoding.
* Standardized numerical features using StandardScaler.

## Feature Engineering

A new feature named **FamilySize** was created using:

FamilySize = SibSp + Parch + 1

This feature improved the understanding of passenger survival patterns.

## Machine Learning Models

The following models were trained and evaluated:

* Logistic Regression
* Decision Tree
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)

## Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Classification Report
* Confusion Matrix
* Cross Validation

## Results

 Model                      Accuracy   
 
 Logistic Regression        80.45%     
 Decision Tree              78.21%     
 K-Nearest Neighbors (KNN)  82.12% 
 Support Vector Machine     81.56%     

Among the evaluated models, K-Nearest Neighbors (KNN) achieved the highest accuracy and was selected as the best-performing model.

## Key Findings

* Female passengers had a significantly higher survival rate than male passengers.
* First-class passengers were more likely to survive than passengers in lower classes.
* Fare and passenger class were important factors influencing survival.
* Small family groups showed better survival rates than passengers traveling alone or in very large families.
* The engineered **FamilySize** feature improved data analysis.

## Future Improvements

* Perform advanced hyperparameter tuning.
* Apply ensemble learning techniques such as Random Forest and XGBoost.
* Deploy the model as a web application using Streamlit or Flask.
* Evaluate additional feature engineering techniques.

## Repository Structure

Titanic-Survival-Prediction
── Titanic Survival Prediction Report
── Titanic_Survival_Prediction.ipynb
── train.csv
── requirements.txt
── README.md

This project was developed as part of a Machine Learning and Data Science learning journey using Python and Google Colab.
