# Portfolio 1
The topic of portfolio 1 is Analysis of an E-commerce Dataset. First you need to Remove missing data, then Descriptive statistics, then Plotting and Analysis, and finally detecting and removing outliers.

Specific operation explain and reflection:
Q1
Import the required libraries and Settings.
Read and examine the original data set: Read the data from the CSV file and store it in origin_df.
The info() method provides an overview of the data, including column names, nonnull counts, and data types.
isnull().sum() calculates the number of missing values in each column.
Print initial data length.
Copying the DataFrame: You create a copy of the origin_df DataFrame called clean_df_occ.
Removing Rows with 'none' in the 'review' Column:  You iterate over each row of the origin_df DataFrame and remove rows where the 'review' column has the value 'none'. You  also count how many rows are removed.
Removing Rows with Missing Values:  You remove any remaining rows with missing values from the clean_df_occ DataFrame and assign the result to clean_df.
Printing the Lengths After Cleaning:  You print the length of the clean_df_occ DataFrame after removing rows with 'none' in the 'review' column,  and the length of the clean_df DataFrame after removing all rows with any missing values.
To summarize, this code reads an e-commerce dataset, examines its initial state,  removes rows with 'none' in the 'review' column, drops any rows with missing values,  and finally prints the number of rows removed and the lengths of the cleaned DataFrames.
Q2
Counting Unique Users: You extract the unique user IDs from the 'userId' column of the clean_df DataFrame and count them.
Counting Unique Reviews: You extract the unique values from the 'review' column and count them.
Counting Unique Items: You extract the unique values from the 'item' column and count them.
Counting Unique Categories: You extract the unique values from the 'category' column and count them.
Describing the 'rating' Column: You display summary statistics of the 'rating' column.
Counting Items Rated by Gender: You group the DataFrame by 'gender' and count the number of items rated by each gender.
Describing the Count of Items Rated by Gender: You display summary statistics of the counts of items rated by gender.
Counting Ratings per Item: You group the DataFrame by 'item' and count the number of ratings for each item.
Describing the Count of Ratings per Item: You display summary statistics of the counts of ratings per item.
In summary, these steps analyze the uniqueness and distribution of various attributes in the cleaned dataset, providing insights into user activity, review diversity, item variety, category diversity, and the distribution of ratings across different dimensions.
Q3
Box Plot of Ratings by Gender
Box Plot of Ratings by Helpfulness
Box Plot of Ratings by Category
These box plots provide a visual summary of how ratings are distributed across different genders, levels of helpfulness, and categories.
They help in identifying patterns, central tendencies, and potential outliers in the ratings based on these categorical variables.
Rotating the x-axis labels ensures that the categorical labels are readable, making the plots more interpretable.
Q4
Removing Outliers Based on Helpfulness:clean_df.index[(clean_df['helpfulness'] <= 2)] gets the indices of the rows where the 'helpfulness' score is <= 2.
Grouping by User and Counting Ratings.
Previewing Grouped User Data
Filtering Users with at Least 7 Ratings:group_user_df[group_user_df['count'] >= 7] filters for users with at least 7 ratings.
Keeping Only Relevant Users in the DataFrame：keeps only the rows where 'userId' is in the userIds list.
Grouping by Item and Counting Ratings
Filtering Items with at Least 11 Ratings
Keeping Only Relevant Items in the DataFrame
Saving the Cleaned DataFrame
This process helps ensure that the dataset only includes users and items with sufficient activity, improving the quality of the analysis.

The above code is intended to further clean and optimize the data set to ensure the quality and accuracy of the analysis.
Specifically, the above code can be used to remove records with low help scores, group and tally scores by user, filter active users, and group and tally scores by product.
