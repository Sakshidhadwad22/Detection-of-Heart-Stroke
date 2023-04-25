# Detection-of-Heart-Stroke
Introduction:
The project I worked on is called "Detection of Heart Stroke". Its purpose is to identify whether a person is at risk of having a heart stroke or not based on the features provided in the dataset. The objective of the project was to find the best model that gives the maximum accuracy to predict whether a person has a stroke or not.

Data Preprocessing:
To begin with, I imported the necessary libraries such as Matplotlib, Seaborn, Pandas, and Numpy to visualize and analyze the dataset. Then, I performed EDA to understand the data better. During this step, I checked for missing values and found that the BMI feature had some null values. I replaced those values with the mean of that feature since the percentage of missing data was only 4%. I also removed the ID column from the dataset since it was not necessary for future forecasting.

Next, I plotted various graphs like pair plots, bar graphs, pie charts, histograms, count plots, and scatter plots to gain insights into each feature or column. I used the df.describe() function to find the range of data and discovered that the ages ranged from 8 months to 82 years, with an average age of 43 years old.

Afterward, I performed encoding using ordinal encoder and checked for correlations between the features and the target column. The correlation was not ideal in the case of hypertension, average glucose level, and BMI columns, but I decided not to remove skewness since these features could differ from person to person, and removing them could lead to a loss of important data.

Model Building:
I split the data into x and y using the train-test split method and then applied different algorithms such as KNN classifier, logistic regression, support vector machine, and decision tree. I found the highest accuracy with the support vector machine algorithm and continued to use it in my further analysis.

To improve the accuracy of the model, I used pipeline and standard scaler but did not observe any significant improvement. Then, I applied GridSearchCV to find the best parameter for the model, and the accuracy remained the same. Next, I applied cross-validation, ensemble learning, and hyperparameter tuning. These methods helped me improve the accuracy of the model.

Conclusion:
In the end, I was able to create a model that predicts whether a person is at risk of having a stroke or not. The accuracy of the model was determined to be the highest with the support vector machine algorithm, and further improvements were made by using cross-validation, ensemble learning, and hyperparameter tuning. However, it's worth noting that the model's performance may be limited due to the data's inherent biases, and there is a need for more diverse datasets for better predictions.
