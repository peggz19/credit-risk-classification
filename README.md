# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* **Analysis Purpose** : The purpose of the analysis is to use Machine Learning and predict the level of risk of a loan. More specifically, it predicts the possibility of a loan to default and see how good our model is with predictions.
* Financial Info: The dataset provided information about the loan itself like its size and the interest rate. On the other hand, it also gives information about the borrower, such as their income, their level of debt (debt to income ratio, total debt and derogatory marks), along with their assets (number of accounts). All of these are important details regarding one's financial health and capabilities.
* **Predicted Variables** : Included in our dataset is a column providing the loan status (default or not). Our goal is to predict that status using a machine learning model. Therefore, this makes that column our target, and a way to ask ourselves : "Based on the financial health of the borrower, can we predict if this loan would default ?"
* **Machine Learning Stages and chosen model**: First, we started with a preprocess step by cleaning our data. We assigned the target to our *y* variable and the features to our *x* variable, making sure to drop the loan_status as it is not part of the features. Second, we split the dataset into train and test data. The train data would be used to fit and train our model while the test data would be used to predict the loan statuses and verify the accuracy of that prediction. Next, we created our model. As we are facing a classification problem with a binary outcome, the Logistic Regression seemed the most logical for that process. Next, as explained above, we used a fraction of the dataset to validate and train de model, then, used the other fraction to predict outcomes. Finally, we performed a confusion matrix to see the quality/accuracy of our model; something that was explained in numbers using a classification report.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

- **Accuracy Score**: The accuracy helps us identify the the *overall* performance of our model and how often it was correct. With an accuracy of 99%, way above the 85% threshold, we can confirm that our model correctly predicted/classified values 99% of the time.
- **Recall Score**: The recall helps us identify how well our model found and identified each outcome. We can see that 99% of healthy loans were correctly identified from all the healthy loans in the dataset. This shows that our model already performed very well in predicting the correct values for each loan.
- **Precision Score**: As for the precision, it helps us identify how well our model found and identified each positive outcome correctly. With a value of 100% for healthy loans and a value of 84% for unhealthy loans, we can definitely see that our loan is way too good at finding good loans (almost being overfit) while it's not good at finding unhealthy ones.
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Based on the above results, we can conclude that a Logistic Regression model is definitely good for any classification problem that involves binary outcomes such as credit risk issues.
It performs very fast and with an amazing accuracy. However, I'd suggest making sure the training dataset is balanced in terms of defaulting loans and non defaulting loans to ensure our model is not overfit and is mainly good at predicting non defaulting loans. 
Right now, it would be best to try to balance our dataset and train the model again before recommending it right away.
