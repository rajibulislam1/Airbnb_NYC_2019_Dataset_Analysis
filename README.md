# Telecom_Churn

# Introduction

The aim of this analysis is to provide insights and develop a customer retention strategy for a specific telecom company. The company's goal is to reduce churn rates and retain its customers. To achieve this goal, we will analyze the provided dataset containing various features related to customer behavior and characteristics. The dataset includes information such as account length, international plan usage, voice mail plan, call metrics, charges, and customer service interactions.

# Data Preprocessing

* In this section, we carried out several preprocessing steps to prepare the data for analysis. The initial steps included importing relevant libraries, loading the dataset, and exploring its structure.
* The dataset contains 3333 rows and 20 columns.

We then performed the following data preprocessing steps:

* Checked for missing values: There were no missing values in any column of the dataset.
* Checked for duplicate values: We identified and removed duplicated rows from the dataset.
* Converted column names to lowercase for consistency.
* Transformed categorical variables: We converted binary categorical variables (such as 'International plan' and 'Voice mail plan') into numerical format (0 for 'No' and 1 for 'Yes').
# Exploratory Data Analysis (EDA)

During the exploratory data analysis phase, we examined the data distribution and relationships between variables. Key findings include:

* We visualized the distribution of various features such as 'International plan', 'Voice mail plan', and 'Area code' with respect to the 'Churn' outcome.
* Histograms were plotted for features like 'Total day minutes', 'Total day calls', 'Total eve minutes', and others to understand the distribution patterns for churned and retained customers.

# Imbalanced Dataset Analysis

* We examined features such as 'Total night calls', 'Total day calls', 'Total eve calls', and others for their distribution patterns with respect to the 'Churn' outcome.
* These analyses provided insights into how these features might contribute to customer churn.

# Correlation Analysis

* We computed the correlation matrix to understand the relationships between different numerical features.
*  Notable correlations were found between 'Churn' and features like 'International plan', 'Total day charge', and 'Customer service calls'.
*  This suggests that these features might have a significant impact on churn rates.

# Heatmap Visualization

* A heatmap visualization of the correlation matrix was created to provide a visual representation of the relationships between different features.
* This visualization helped identify which features are strongly correlated with each other and with the 'Churn' outcome.

# Building the Machine Learning Model

* To predict customer churn, we built a machine-learning model using a logistic regression algorithm. I selected the features 'International plan', 'Total day charge', and 'Customer service calls' as independent variables.
* We split the data into training and testing sets and applied feature scaling to ensure uniformity among feature ranges.

# Model Evaluation

 * Trained the logistic regression model on the training data and evaluated its performance on the testing data.
 * We used classification metrics such as accuracy, precision, recall, and F1-score to assess the model's effectiveness in predicting customer churn.

# Conclusion and Recommendations

* In this analysis, we explored a telecom company's dataset to understand customer behavior and characteristics related to churn.
* We identified important features like 'International plan', 'Total day charge', and 'Customer service calls' that are correlated with churn rates.
* Additionally, we built a logistic regression model to predict customer churn with a reasonable level of accuracy.

Based on our analysis, we recommend the following strategies to the telecom company for improving customer retention:

* Focus on improving customer service interactions, as higher customer service call numbers were associated with increased churn.
* Consider providing incentives or personalized offers to customers using international plans, as they showed a higher likelihood of churning.
* Monitor and manage charges for customers with high 'Total day charge', as this feature also exhibited a correlation with churn.

