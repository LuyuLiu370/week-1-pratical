Name：Luyu Liu
Student-ID：45522367
Assignment: Reflective Report

The process of problem solving and learning to use the notebook:
1. data collection: obtaining datasets of COVID-19 cumulative confirmed cases and CPI values from WHO and USDA.
2. data cleaning: filtering and cleaning the data, including removing missing values and irrelevant data.
3. data analysis: preliminary analysis and visualization of the data to understand the distribution of the number of confirmed cases and CPI values across countries.
-Calculates and plots the cumulative number of confirmed cases for each WHO region;
-Plot line graphs of CPI values and growth rates for each country.
4. Feature selection: the most important features are selected using the RFE technique.
-screen data for the top 10 countries with the highest cumulative number of confirmed cases;
-screened CPI data for these countries;
-merge COVID-19 and CPI data.
5. Model training: train and evaluate the data using linear regression and polynomial regression models.
-linear regression model;
-polynomial regression model;
-recursive feature elimination (RFE).
6. Result Analysis: Interpret the coefficients and performance of the model and analyze it in context.
-Linear regression model: the coefficients indicate the effect of CPI values on the cumulative number of confirmed cases in different years. The R-squared value of the linear regression model indicates that the model explains 67% of the variables, which suggests a strong linear relationship between CPI values and the number of confirmed cases.
-Polynomial regression model: polynomial regression has more complex coefficients, indicating a nonlinear relationship. It captures more complex patterns than linear models.
-Recursive Feature Elimination (RFE): The R-squared value of the linear regression model was 0.67, indicating good explanatory power of the model.
7. Summary conclusions: Summarize the findings of the study and compare them to intuitive expectations. By analyzing the data on the number of confirmed cases and CPI values of COVID-19, I found that: changes in CPI values during the epidemic had a significant effect on the number of confirmed cases. Both linear regression and polynomial regression models indicated a relationship.The RFE technique helped identify the most important characteristic years and contributed to the understanding of the specific impact of CPI values on the spread of the epidemic.
These results provide a basis for further research and can be used to develop more effective public health and economic policies.

How is it going? What would you be interested in doing in the future?
Throughout portfolio 4, I have significantly deepened in several key areas:
1. data collection and cleaning: efficiently clean and prepare COVID-19 and CPI datasets for analysis.
2. Exploratory Data Analysis (EDA): Create detailed visualizations such as pie charts, bar charts, etc. to summarize COVID-19 case distributions and CPI value trends.
3. Characterization and Selection: Use RFE to successfully identify the most influential years for CPI values affecting COVID-19 cases.
4. Modeling and Evaluation: Linear and polynomial regression models were developed and evaluated to examine the relationship between CPI values and new cases of Crown pneumonia.
5. Summary Reporting: Provide a comprehensive report on the process, results, and interpretation of the analysis of the 2019 coronavirus disease outbreak and CPI data.
Future Interests and Applications:
1. using advanced modeling to predict future trends in epidemiologic and economic indicators.
2. working with public health organizations and policy makers to provide data-driven insights for better decision making. Or, use data analytics to inform and shape public policy responses to health and economic challenges.
3. develop systems for monitoring and responding to public health crises in real time, integrating data from a variety of sources to achieve comprehensive situational awareness.
By continuing to build on the foundation laid in this unit, my goal is to make meaningful contributions to solving real-world problems through data-driven insights and innovations.

Discussion based on portfolio 4:
1) Why the dataset used for the portfolio was chosen
The reasons for selecting the dataset of COVID-19 cumulative confirmed cases and CPI values are:
-Global impact: the COVID-19 pandemic has had a profound impact on the economies and public health systems of various countries around the globe, and analyzing its impact can provide valuable insights.
-Data Availability: The World Health Organization (WHO) provides detailed data on confirmed cases of COVID-19, while the U.S. Department of Agriculture (USDA) provides CPI data for each country, which are easily accessible and of high quality.
-Cross-domain analysis: These datasets allow us to analyze across public health and economics to explore the specific impact of the outbreak on economic indicators.
2) Can you explain well the insights or conclusions you drew from the study? Do the results match your intuitive expectations?
Key insights and conclusions drawn from the study include:
-Relationship between CPI and outbreak spread: the model showed that CPI values had some explanatory power (R-squared value of 0.67) in predicting confirmed cases of COVID-19. This suggests that there is a correlation between economic activity and price levels and the spread of the epidemic.
-Key years: the key features selected for the RFE were 2019, 2022, and 2024, which represent the early, peak, and late stages of the epidemic, respectively. They are the most important for predicting the number of confirmed cases of the epidemic, which is consistent with intuitive expectations, as these three time points represent different stages of the epidemic.
-Trends in CPI: From 2019 to 2022, CPI values generally increase, likely reflecting economic uncertainty and inflationary pressures at the beginning and peak of the epidemic.CPI values decrease after 2022, likely reflecting a controlled epidemic and gradual economic recovery.
These results are consistent with intuitive expectations, as the impact of the epidemic on global economic activity and price levels was significant.
