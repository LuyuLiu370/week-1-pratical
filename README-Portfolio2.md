# Portfolio 2
The topic of portfolio 2 is Analysis of an E-commerce Dataset Part 2. First, we Import Cleaned E-commerce Dataset, then Explore the Dataset, Split Training and Testing Data, Train Linear Regression Models with Feature Selection under Cases 1 & 2, Evaluate Models, Finally Visualize, Compare and Analyze the Results.

Step analysis:
Explore the Dataset：
Import and preview data
Encode the categorical variables
Calculate correlations between variables
Calculate the correlation matrix between all the variables
Find out which features are most and least correlated with rating
Objective: To identify the most relevant and least relevant features through the ordinal encoding of categorical variables, calculate the correlation between different variables and rating.
Effect: Help to understand which variables have a significant impact on the score, and provide reference for subsequent analysis and modeling.

Split Training and Testing Data：
Dividing the data by 10% : test_size=0.1 means that the test set accounts for 10% of the total data set, and the remaining 90% is used for the training set. random_state=142 is used to set the random seed to ensure that the split results are consistent each time the code is run. train_10, test_10 are the training set and the test set respectively.
Dividing the data by 90% : test_size=0.9 means that the test set accounts for 90% of the total data set, and the remaining 10% is used for the training set. random_state=142 is used to set the random seed to ensure that the split results are consistent each time the code is run. train_90, test_90 are the training set and the test set respectively.
Objective: To divide the data set into training set and test set for the training and evaluation of the model. The performance of the model under different data amounts can be verified by different partition ratios.
Effect:
Case 1 (10% test set) : Reserve 10% of the data for testing and 90% for training. This is often used for model training when the amount of data is sufficient.
Case 2 (90% test set) : Keep 90% of the data for testing and 10% for training. This extreme division may be used for testing and verification in special scenarios.

Train Linear Regression Models with Feature Selection under Cases 1 & 2：
Initialize the linear regression model
Feature selection: Suppose there is a function select_features that selects the most and least relevant features based on the correlation matrix (which contains only numerical features) of the entered data set. These features are used for subsequent model training.
Prepare the training data: X_train_a_1 and y_train_a_1 are trained using the most relevant features in case 1.
X_train_b_1 and y_train_b_1 are trained using the least relevant features in case 1.
X_train_c_2 and y_train_c_2 were trained using the most relevant features in case 2.
X_train_d_2 and y_train_d_2 were trained using the least relevant features in case 2.
Train and evaluate linear regression models.
This code shows how to use linear regression models for training and evaluation under different feature sets and data set partitions. By selecting the most relevant and least relevant features, the performance of the model under different data set configurations can be compared to find the best feature set and model configuration. This is important for optimizing the predictive power and generalization power of the model.

Evaluate Models:
Calculate the root mean square error (RMSE) : RMSE is the root mean square error, which measures the average deviation between the predicted value and the actual value.
The MSE and RMSE of each model were printed separately in order to compare the model's prediction errors under different feature selection and data set partitioning.
RMSE can intuitively evaluate the predictive performance of each model in order to select the optimal model or optimize the feature selection strategy.

Visualize, Compare and Analyze the Results：
Two bar charts were drawn to compare the performance of four different models under two evaluation indexes (mean square error MSE and root mean square error RMSE).
Through the chart, we can quickly understand the prediction error size of each model and its changing trend under different feature selection and data set partitioning, which is helpful to select the optimal model configuration or optimize the feature selection strategy.
