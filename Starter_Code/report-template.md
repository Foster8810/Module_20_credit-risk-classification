# Module 20 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The purpose of the analysis was to train the create a model that could predict all future values of anyone with a loan to try and see if they are in good standing with their loan with the information provided.  We calculate the information by taking the loan size, interest rate, borrower income, debt to income ratio, number of accounts they own, derogatory marks they have, and the total amount of the debt.  Using these information, we were trying to predict the status of the loan.  If they are in a healthy status they would receive a 0, and if they are at risk of defaulting they would be classified as 1.  Throughout this assignment, we took the time to split the data into the y variables (what we are trying to find/predict) and the X variables (the features or data we are trying to predict from).  We then take some of the information from the data frame and train our machine learning model to learn from them, and finally test to see how we did compared to the entire data set with the acutal results we got.  We used logistic regression for the method since, if we were to visualize the data set they would follow a logistic model.  Also since the values have one dependent variable y which is binary and multiple independent variables it works well with a logistic regression.  
## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
1. Accuracy: the accuracy of the model that we created was 0.99 or 99% (rounded).  This compares all of the correct values (true positive, true negative) over all the values in the confusion matrix.  This shows how accurate we were able to train the data set and correctly find the right values for each feature.  
2. Precision: Precision calculates all of the correct values in a specific target over all of the target values we found in the training set.  In our case for 0 (healthy loans) we would look for how many correctly guessed 0 there were over all 0 we found in the machine learning model.  For 1 (unheatlhty loans/default risk) we would count how many correct 1 we had over total 1s we had in the trained model.  
3. Recall: Recall is how complete our positive predictions were.  We can calculate this by the correct value of a single target over the total acutal target we wanted.  For 0, we would find the true positives and divide that by the amount of true positives plus the amount of false negatives and vice versa for 1.  


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The machine learning model that we used for this particular assignment worked really well.  We can see from the accuracy that we were able to accurately train the model to find the correct answer 99% of the time.  We can even see from the other metrics (pprecision and recall) that this model was had a very good measure of quality and quantity.  I believe that this model is best fir for the logistic regression model and we can see that from the result.  For the real world example this type of machine learning model probably exists in the real world very often.  The performance of this problem it is much more important to guess the 1's or unhealthy loans that are at a risk of defaulting rather than the 0's the healthy ones.  This is because finding the unhealhty loans would provide a risk analysis of our overall loans.  Although in this case the values are binary finding one would find the other.  
