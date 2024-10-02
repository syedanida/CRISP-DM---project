# **Titanic Survival Prediction using CRISP-DM Methodology**

## **Project Overview**
This project aims to demonstrate the use of the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology to build a predictive model for Titanic passenger survival. The dataset used includes information on various passenger attributes such as age, gender, class, and fare. By applying CRISP-DM's six phases—Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment—this project identifies key factors influencing survival and builds a robust classification model using machine learning techniques.

The goal is to provide a structured approach to data science and develop a model that accurately predicts whether a passenger would survive based on their profile.

## **CRISP-DM Methodology**
CRISP-DM is a widely used methodology for data mining projects. It consists of six phases, each focusing on a specific aspect of the data science process:

### **1. Business Understanding**
- **Project Objective**: Understand the factors influencing Titanic passenger survival and build a predictive model.
- **Success Criteria**: Achieve at least 80% accuracy in predicting survival on the test dataset.

### **2. Data Understanding**
- Loaded the Titanic dataset from Kaggle containing 891 rows and 12 columns.
- Analyzed the distribution of features such as `Sex`, `Pclass`, and `Age` to understand their relationship with survival.
- Performed initial visualizations to identify class imbalance and key patterns.

### **3. Data Preparation**
- Handled missing values in the `Age` column using median imputation.
- Dropped irrelevant columns such as `Cabin` due to high missing rates.
- Converted categorical variables like `Sex` and `Embarked` into numerical representations using one-hot encoding.
- Engineered new features such as `FamilySize` and `IsAlone` to capture social relationships and improve model accuracy.

### **4. Modeling**
- Implemented multiple machine learning algorithms, including Logistic Regression, Decision Trees, and Random Forests.
- Hyperparameter tuning was performed using Grid Search to optimize model performance.
- Random Forest was chosen as the final model due to its high accuracy and balanced performance.

### **5. Evaluation**
- Evaluated model performance using metrics such as Precision, Recall, F1-Score, and ROC-AUC.
- The Random Forest model achieved an accuracy of 85% and an F1-Score of 0.84.
- Visualized the results using a confusion matrix and ROC curve.

### **6. Deployment**
- Deployed the final model using a Flask API, allowing users to input passenger attributes and receive survival predictions.
- Hosted the application on AWS for scalability and real-time predictions.

## **Dataset Information**
The dataset used for this project is the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic) dataset from Kaggle. It includes the following key features:

- **PassengerId**: Unique ID for each passenger.
- **Survived**: Survival indicator (0 = No, 1 = Yes).
- **Pclass**: Passenger class (1 = First, 2 = Second, 3 = Third).
- **Name**: Name of the passenger.
- **Sex**: Gender of the passenger.
- **Age**: Age of the passenger.
- **SibSp**: Number of siblings or spouses aboard the Titanic.
- **Parch**: Number of parents or children aboard.
- **Fare**: Ticket fare.
- **Embarked**: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton).

## **Medium Article**
https://medium.com/@syedanidakhader/predicting-survival-on-the-titanic-a-data-science-journey-9ca5a49f69b5
