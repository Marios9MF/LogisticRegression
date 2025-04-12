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


# Workflow Notes
## In my own words!! This might not be accurate.

1. **Business Understanding** - Understand the needs of the business and therefore understand what the business is operating in and what kind of problem needs to solved.
2. **Data collection** - While some data needs to be collected from the business and recorded, it is also possible for the data scientist to collect more data from other sources. Additional data can also be collected from databases (SQL) and from websites that host datasets, such as the Data Asset Exchange (DAX). It is also possible to use Generative AI to generate plausible data that can expand the dataset and help with the training of the model.
3. **Data Cleaning and Preparation** - Remove missing values, drop "Not a Number" NaN values. It might also be necessary to reorganise the data in a way that is more meaningful and easy to operate.
4. **Exploratory Data Analysis (EDA)** - The first step when the data is obtained is to understand what it contains. Let's assume that like in the exercise you load the dataset with the Pandas library.
	4.1 You want to understand how many elements it contains. *dataset.size*
	4.2 You want to check how many rows and columns are present. *dataset.shape*
	4.3 It would be helpful to know what data types are contained per column. Are these integer numbers, decimal (floating-point) numbers, text (objects)? *dataset.dtype*
	4.4 Run some column descriptive statistics to see the mean, std.dev., *etc*. of each column.
	4.4 Plot some of the columns to visualise how different information are related to one another.
5. **Feature Engineering** - When the data has been explored and somewhat understood, we can proceed to fitting a model. We need to choose an appropriate model. In the exercise this is logistic regression. Before feeding the selected x values and y values (in the case of a supervised model) we need to choose whether to **clean** and **manipulate** the data. An example would be to normalised or standardise the data so that all values are from 0 and 1, or in such a way that all the values are distributed around the mean taken as a 0 (read further).
6. **Machine Learning** - Split the data into a training set and a test set. Reason about the hyperparameters that you could tune. Given the hyperparameters, decide whether to run a **grid search**. Decide whether to use **cross-validation**. More than one model could be used to fit and predict the data depending on what the final objective is. In the exercise, a logistic regression model was used from the library scikit-learn.
7. **Model Evaluation** - Goes without saying. Use metrics to understand if your model predicts stuff well. Thins like **accuracy**, **precision**, **recall**, **F1-Score**, using a **confusion matrix** to visually evaluate the True/False Positive and True/False Negatives of a model, if this applies to it. More specific metrics, such as the **log-loss** "cost" function can be used. Visualising the predicted data and the scores is also a good idea.
8. **Deploy the model** - if the model is good enough for the purpose, the model can actively be used by businesses. The model is monitored, refined and data is added to it to train it even further for better prediction. This ultimately leads to having to go back a few steps and repeating them.
