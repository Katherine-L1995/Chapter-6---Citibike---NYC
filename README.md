*6.4 - Task*

**Overview**
In this section, I explored the relationship between trip duration and start hour of the day, as well as analyzed the relationship between subscriber status and weekday usage. The analysis involved creating a linear regression model to predict trip duration based on start hour and performing a Chi-Square test to examine the relationship between weekday and subscriber status.

**Step-by-Step Breakdown**

Data Preparation and Cleaning:

Imported necessary libraries (e.g., pandas, numpy, matplotlib, seaborn, scikit-learn).
Cleaned the data by handling missing values and converting the start time to extract the start hour of the day.
Exploratory Data Analysis (EDA):

Visualized the relationship between trip duration and start hour using a scatter plot to identify trends.

Linear Regression Model:
Defined the independent variable (start_hour) and dependent variable (trip_duration).
Split the data into training and test sets, then trained a linear regression model on the training data.
Predicted trip duration based on start hour and visualized the results with a regression line.

Model Evaluation:
Evaluated the model’s performance using Mean Squared Error (MSE) and R² score.
The results showed a weak correlation between trip duration and start hour, as reflected by the low R² score and high MSE.

Subscriber Status and Weekday Analysis:
Performed a Chi-Square test to examine the relationship between weekday and subscriber status.
Created a heatmap to visually display the distribution of subscribers vs non-subscribers across weekdays.
Findings indicated a strong relationship between subscriber status and weekday, with weekday users being primarily subscribers.
