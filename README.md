# Automatic Ticket Classification

Welcome to this case study on **Automatic Ticket Classification**. In this repository, you will find the implementation of a model that can automatically classify customer complaints based on the products and services mentioned in the tickets.

## Problem Statement

For a financial company, customer complaints play a crucial role in identifying shortcomings in their products and services. Efficiently resolving these complaints is vital for minimizing customer dissatisfaction and retaining strong loyalty. Traditionally, companies assign the task of evaluating and assigning each ticket to relevant departments to multiple support employees, which becomes cumbersome as the company grows.

In this case study, I will work as an NLP engineer for a financial company aiming to automate its customer support ticket system. My task is to build a model that can classify customer complaints based on the products/services mentioned.

## Business Goal

The goal is to build a model capable of classifying customer complaints into relevant categories, facilitating quick issue resolution. By employing non-negative matrix factorization (NMF), I will detect patterns and recurring words in each ticket, which will help me to identify important features for each cluster of categories. The identified clusters will represent the topics of customer complaints.

## Dataset

The dataset provided is in .json format containing 78,313 customer complaints with 22 features. My first task is to convert this dataset into a dataframe for processing.

## Expected Tasks

I am expected to perform the following tasks:

1. **Data Loading**: Import the .json data and create a dataframe.
2. **Text Preprocessing**: Perform operations like filtering text, removing missing values, and renaming column headers.
3. **Exploratory Data Analysis (EDA)**: Analyze data to understand its characteristics.
4. **Feature Extraction**: Extract features using Td-Idf.
5. **Topic Modelling**: Utilize NMF to set the best number of clusters to 5, create word clusters, and map clusters to topics/cluster names.
6. **Model Building**: Prepare train & test data using labels received from NMF. Apply at least two models such as Logistic Regression, Decision Tree, and Random Forest.
7. **Model Training and Evaluation**: Train and evaluate model performance using relevant evaluation metrics to select the best model.
8. **Model Inference**: Apply the best model to predict custom text and assess its performance.

## Evaluation Rubrics

Each stage is assigned a weightage, and the rubrics for meeting expectations are outlined as follows:

1. **Data Reading/Data Understanding**: 5
2. **Data Cleaning**: 10
3. **Data Preprocessing**: 10
4. **Data Visualization**: 10
5. **Feature Extraction**: 5
6. **Topic Modelling**: 25
7. **Model Building**: 20
8. **Model Inference**: 5
9. **Code Readability and Conciseness**: 10

## Conclusions

After completing the tasks, the following conclusions were drawn:

- **Identified Topics**: Payment Issues, Customer Service, Account and Banking, Credit Card Issues, Fraud and Security.
- **Model Performance**:

    | Model              | Accuracy |
    |--------------------|----------|
    | Logistic Regression| 97%      |
    | Decision Tree      | 93%      |
    | Random Forest      | 93%      |
    | Naive Bayes        | 83%      |


