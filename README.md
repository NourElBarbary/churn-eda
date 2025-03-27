# Churn Modelling - Exploratory Data Analysis (EDA)

This project focuses on performing Exploratory Data Analysis (EDA) on a customer churn dataset to understand customer behavior and identify factors leading to churn. The dataset contains information about bank customers, including demographic details, account balances, and banking behavior.

## Project Overview

The primary goal of this project is to analyze the customer churn dataset to:

-   Understand the distribution of various features.
-   Identify outliers and missing values.
-   Explore correlations between features.
-   Gain insights into customer churn patterns.

## Tasks Performed

This notebook covers the following key EDA tasks:

1.  **Dealing with Missing Values:**
    -   The dataset was checked for missing values. Fortunately, no missing values were found.
2.  **Dealing with Outliers:**
    -   Outliers were identified in the `CreditScore` and `Age` columns.
    -   Boxplots were used to visualize outliers.
    -   `CreditScore` was binned into categorical features to handle outliers and improve analysis.
3.  **Correlation Analysis:**
    -   Correlation between numerical features was analyzed using a heatmap.
    -   Correlation between categorical features was analyzed using Cramer's V.
    -   Correlation between categorical and numerical features was analyzed using point-biserial correlation and ANOVA.
4.  **Exploratory Data Analysis (EDA):**
    -   Descriptive statistics of the dataset.
    -   Distribution of categorical and numerical features.
    -   Analysis of customer churn by various features (Geography, Gender, Age, Tenure, Balance, Number of Products, Credit Card Ownership, Active Membership).
    -   Feature engineering was used to create new features such as `CreditScore_Category` and `Age_Group`.
    -   Visualization using `matplotlib`, `seaborn`, and `plotly`.

## Dataset Description

The dataset `Churn_Modelling.csv` contains the following columns:

-   `RowNumber`: Index of the row.
-   `CustomerId`: Unique identifier for each customer.
-   `Surname`: Last name of the customer.
-   `CreditScore`: Numerical creditworthiness score.
-   `Geography`: Country where the customer is located.
-   `Gender`: Customer's gender.
-   `Age`: Customer's age.
-   `Tenure`: Number of years the customer has been with the bank.
-   `Balance`: Customer's bank account balance.
-   `NumOfProducts`: Number of bank products the customer has.
-   `HasCrCard`: Whether the customer owns a credit card.
-   `IsActiveMember`: Whether the customer is actively using the bank’s services.
-   `EstimatedSalary`: Customer’s estimated annual salary.
-   `Exited`: Whether the customer left the bank (target variable).

## Libraries Used

-   `pandas`
-   `numpy`
-   `matplotlib.pyplot`
-   `seaborn`
-   `plotly.express`
-   `plotly.graph_objects`
-   `plotly.figure_factory`
-   `scipy.stats`
-   `sklearn.preprocessing`
-   `statsmodels.api`
-   `geopy.geocoders`
-   `re`

## Notebook Structure

The Jupyter Notebook `Churn_Modelling.ipynb` contains the following sections:

1.  **Importing Libraries and Reading Data:** Loading necessary libraries and the dataset.
2.  **Dataset Description:** Overview of the dataset and column descriptions.
3.  **Task 1: Explore and Familiarize with the Dataset:** Initial data exploration.
4.  **Outlier Analysis:** Identifying and visualizing outliers.
5.  **Feature Engineering:** Creating new features to improve analysis.
6.  **Correlation Analysis:** Analyzing correlations between features.
7.  **Visualization:** Creating various plots to understand data distributions and relationships.

## Key Findings

-      Most exited customers are from Germany and France.
-      Females are the most who exited.
-      Customers with poor and fair credit scores are more likely to churn.
-      Ages between 20-35 and 60-75 are the most exited groups.
-      Customers who have used only one product are more likely to churn.
-      Non-active members are more likely to churn.
-      Exited mostly correlates with balance and age.
-   Geography, Age Group, and Credit Score Category have strong influences on balance, tenure, and churn.
-   Surname is not useful for prediction.

## Future Work

-   Apply machine learning models to predict customer churn.
-   Further feature engineering to improve model performance.
-   Advanced statistical analysis to uncover deeper insights.
-   Implement interactive dashboards for better visualization.
