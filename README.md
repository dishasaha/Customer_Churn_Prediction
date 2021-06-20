# Customer_Churn_Prediction
Final Project for DSC550 Data Mining

This project was done to see if a prediction model can be created for Churn for the Orange telecom dataset. To do this, some preliminary evaluation of the dataset took place to see if there were any missing data in the datasets that were provided by Kaggle. After I looked at the data, I moved forward by doing some exploratory data analysis.  For me I found plotting the pie chart showing the percentages for True and False really provided me a good visual for the distribution at hand. I was also curious to see if there were any features that were correlating, and so I used the seaborn library to create a pair plot chart to show case the relationship among each variables. Few of the pair plot graphs ended up showing a positive correlation, such as the Total day minutes and Total day charge, Total evening minutes and Total evening  charge, Total night minutes and Total night charge and finally the Total international minutes and Total international charge. Afterwards, I preprocessed the data by establishing variables for the “x_train”, “y_train”, “x_test”, “y_test”.  Going forward, I know that it is best practice is to scale the features/columns so that the rage is normalized, where the standard deviation is 1. To do this task I sed the Standard Scaler function from the “SkLearn.preprocessing” library.  Consequently, the method used in this final project to create a prediction model was done successfully using the KNN classifier model. This was done by using the “KNeighborsClassifier” function from the “sklearn.neighbors” library. Additionally, the evaluating the algorithm was the next logical step. To accomplish this task I calculated the confusion matrix, and the classification report. The results showed an accuracy rate of 90%. I also did an error rate comparison with the K values, which I did my computing the error values in a loop, and then plotting the graph. The graph results showed that the mean error was at the lowest level of 0.10 when K was 7, 9, and 11. For my model I used a K of 7, which made the accuracy to be 90%. Therefore, I was able to successfully create a prediction model for churn for the Orange telecom dataset using the K nearest neighbor algorithm. 
