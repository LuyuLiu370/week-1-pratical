# Portfolio 4
Portfolio 4 is about self-exploration. I chose to explore the association between the top ten countries in terms of cases due to COVID-19 and the CPI values of COVID-19 these ten countries after 2019.

First, the CSV file of global data on COVID-19 was processed and some data cleaning, sorting and grouping operations were performed.
A new DataFrame df_cleaned is created with the columns 'Name' (country name), 'WHO Region' (WHO region), and 'cases-cumulative total' (cumulative number of confirmed Cases) from the original data box.
Sorted by cumulative number of confirmed cases in descending order
The cumulative number of confirmed cases was grouped by WHO region
Together, these steps help me understand and analyze COVID-19 global data for further visualization or analytical work.
A pie chart showing the share of cumulative confirmed cases in each WHO region is created.
A horizontal bar chart showing the data for the top ten countries (by cumulative number of confirmed cases) after global data is excluded helps to compare the situation in these countries.
The Consumer Price Index (CPI) data for designated countries since 2019 is extracted and a line chart of the CPI values for these countries is plotted over the period from 2019 to 2024.
A line chart of the growth rate of the Consumer Price Index (CPI) for the specified countries from 2019 to 2024 is drawn to help analyze the economic trends of each country.
Each set of codes has its specific data processing and visualization purpose to present and analyze trends and comparisons in COVID-19 case data or economic indicator data.
The top 10 countries were selected based on the cumulative number of confirmed cases, and a horizontal bar chart was drawn to compare the epidemic situation in these countries.
The data of the top 10 countries with the cumulative number of confirmed cases were screened from CPI data and combined with COVID-19 data to prepare data for subsequent modeling.
The linear regression model was used to analyze the linear relationship between cumulative confirmed cases and CPI, and the coefficient of the model was output.
Polynomial regression model was used to further analyze the nonlinear relationship between cumulative confirmed cases and CPI values, and output the coefficients of the model.
Recursive feature elimination (RFE) techniques are used to select the features that are most important for the prediction of cumulative confirmed cases and output the names of these features.
Output the performance evaluation index of the linear regression model with the top 3 features selected by RFE, namely the R-squared value. 
This value reflects how well the model explains the variance of the target variable (cumulative number of confirmed cases).
This enables a complete process from data filtering, model building to performance evaluation. 
This helps analyze the relationship between COVID-19 and the Economic Indicators (CPI) and identify the factors that have the most significant impact on the epidemic.
Several conclusions can be drawn from the above analysis:
Model fit: The linear regression model was used to predict the relationship between cumulative COVID-19 confirmed cases and CPI value. 
The R-squared value of the model was 0.67, indicating that the model could explain about 67% of the variance of the target variable (cumulative number of confirmed cases).
This indicates that the selected CPI features have a certain predictive ability to explain the impact of the epidemic, but there is still a part of the variance that cannot be explained by the model.
Regional characteristics of outbreaks: The top 10 countries with cumulative confirmed cases typically have high population densities and well-developed international transport networks, 
which make it easier for the virus to spread. These factors add to the challenges of responding to the outbreak in these countries.
Economic impact of COVID-19: Combined with the chart of changes in CPI values, it can be seen that higher CPI values may reflect increased economic activity, inflation and rising prices, 
which may lead to increased population movements and social interactions, thereby increasing the risk of COVID-19 transmission. 
In addition, changes in CPI values may also reflect changes in the economic policies adopted by the government in response to the COVID-19 outbreak at different stages and in the mentality and behavior of the people.
Key features selected by RFE: The top 3 features selected by RFE are CPI values for 2019, 2022 and 2024. 
These years represent different economic and social contexts in the early, peak and later stages of the outbreak, which have a significant impact on the spread of the outbreak and economic recovery.
Changes in the rate of growth of CPI values: CPI values in these countries increased from 2019 to 2022, and then began to decline from 2022 to 2024. 
This change can be influenced by a variety of factors, including economic conditions, monetary policy, supply and demand, and government policy adjustments.
