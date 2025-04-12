# Disclaimer
Please notice that the dataset used in this problem is generated using Google Gemini for the purpose of practing some Python data science skills and the data science workflow.

This notebook contains a data set with 60000 data points, the actual interpretation of the model might have no real-world meaning.
# Task: Predicting Customer Churn

You are a data scientist at a telecommunications company. The company is concerned about customers leaving their service (churning). You have been tasked with building a model that can predict which customers are likely to churn based on their account information and usage patterns.

In this context, *churning* is the loss of a customer for any reason at all.

## Your goals are to:

1. **Load and Explore the Data**: Load the provided dataset using Pandas. Examine the data to understand its structure, features, and data types.
2. **Perform Basic Data Cleaning**: Check for any missing values or inconsistencies in the data and handle them appropriately.
3. **Perform Exploratory Data Analysis (EDA)**: Visualize the data to understand the relationships between different features and the churn status. Look for any patterns or trends that might be indicative of churn.
4. **Prepare the Data for Modeling**: This might involve encoding categorical features (converting text-based categories into numerical representations) and potentially scaling numerical features.
5. **Build a Simple Classification Model**: Train a basic classification model (e.g., Logistic Regression) using scikit-learn to predict whether a customer will churn or not.
6. **Evaluate the Model**: Assess the performance of your model using appropriate metrics (e.g., accuracy, precision, recall, F1-score).
7. **Document Your Findings**: Explain your steps, the insights you gained from the data, and the performance of your model.