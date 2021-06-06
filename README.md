# BankNote_Forging_Prediction

  In this project we will fit a logistic regression model, lda and qda classifier to predict the
probability of a banknote being forged using the Banknote data set. This data has been
divided into training and testing sets: BankTrain.csv and BankTest.csv (available in the repo). The response variable is y (the fifth column), where y = 1
denotes a forged banknote and y = 0 denotes a genuine banknote. Although this data
set has four predictors, we will be using x1 and x2 to fit our model.

# Observations 

# For threshold 0.5
On calculating the confusion matrix, accuracy rate and error rate with our model on the test data set we obtained the following results,

•	The accuracy rate is 88.59% (2 dp) which implies that 88.59% of the test data is predicted correctly by our model

•	The error rate is 11.41%(2 dp) which implies that 11.41% of the test data is predicted wrongly by our model

•	The specificity is 0.9153 which implies that 91.53% of the actual genuine notes are predicted as genuine

•	The precision is 0.8817 which implies that 88.17%  are actually forged and 11.83% of genuine notes are predicted as forged

•	The sensitivity is 0.8466 which implies that 84.66% of the actual forged notes are predicted as forged by this model.

The above results especially sensitivity projects that this model predicts considerably good.

![image](https://user-images.githubusercontent.com/68840596/120910623-75ffd900-c6d4-11eb-9255-22edc1f0ac37.png)


# For threshold 0.3
Sensitivity = 156/20+156=88.64%(2 dp)

Specificity = 200/200+36=84.75%(2dp)

Accuracy = 86.41%(2dp)

Error rate = 13.59%(2dp)

•	We can visualise that forged noted are predicted better here with the increase in sensitivity to 88.64%

•	Specificity, accuracy reduced in comparison with threshold 0.5

# For threshold 0.7
Sensitivity = 133/43+133 =75.57%(2dp)

Specificity = 223/223+13 = 94.49%(2 dp)

Accuracy = 86.41%(2 dp)

Error rate =  13.59%(2dp)

•	A significant drop in sensitivity to 75.57% marks that forged notes are not predicted as much as with threshold 0.3

•	Accuracy for both the threshold 0.3 and 0.7 are same.

•	Specificity increased.

# On Comparing threshold 0.5, 0.3 and 0.7
For a model with the intention of finding forged note, sensitivity should be considered as the decision maker. In that case, our model with the threshold value 0.3 can be declared the best model in detecting forged notes due to its highest sensitivity 88.64% which means that 88.64% of actual forged notes are detected as forged by the model and serves the purpose.

# LDA, QDA Classifier

LDA Vs QDA and Logistic Regression with   threshold 0.5:

•	LDA has lower accuracy rate of 87.86%(2 dp) when compared with Logistic regression  with 88.59% accuracy and QDA with 89.08% accuracy

•	Again LDA has lower Precision rate of 87.95%(2 dp) and sensitivity rate of 82.95%(2 dp) when compared with Logistic regression and QDA 

•	Same Specificity rate of 91.53%  as logistic regression but minimal than that of QDA.

QDA Vs LDA and Logistic Regression with threshold 0.5:
1.	QDA has the highest accuracy rate of 89.08%(2 dp) when compared to LDA and Logistic Regression
2.	Also QDA has better Precision rate of 89.70%(2 dp) and specificity rate of 92.80%(2 dp) when compared to LDA and logistic regression
3.	Similar sensitivity rate of 84.10%(2 dp) in QDA as of  logistic regression sensitivity rate of 84.66%
As we discussed already sensitivity is the decision maker for our model and since QDA and logistic regression has similar sensitivity we need to look out for other factors.  On comparing , QDA seems to be the better model for detecting forged note due to its high accuracy rate of 89.08% (2 dp) which means the error rate of 10.92%(2 dp) and also due to its better precision and specificity than other models.
