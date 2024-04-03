# Credit-Risk-Classification
For this challange we had to create a linear regression model a csv about safe and highrisk loans. Once the model was made we needed to write an analysis follwoing the below criteria.

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

Analysis
The purpose of this analysis is to determine the health of future loans. This means how well a loan worked out for the company. is it being paid off on time? or not at all? how profitable is the loan? these are the questions required to analyse a loans health. These were the columns in our dataframe: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, loan_status. these columns provided information we used to create a liniar regression to noticed the trends of past loans to predict future loans. By feeding the machine learning with this information we were able to gather data regarding how well loan health is predicted and allowed us to gain an understandig of the accuracy our choices. We used a sklearn model to train our machine with an 80/20 slpit between taining and testing. using logistic regression made this all possible as it allowed us to create predictions for loan statuses and that allowed us to use a confusion matrix to check how accurate and precise our predictins are.
## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    * Accuracy: Within this dataset and cofusion matric the accuracy was 99% on the f1-score. Having such a high accuracy but being short of perfect is an incredable achievment to how well the machine funstions.
This means the model is exceptional at making correct prediction across all classes be it a true positive case or true negative
    * Precision: When it comes to precison, 100% of all healthy loans were predicted while only 86% of righrisk loans were predicted. Normaly 100% is a bad sigh as it deteremines you are only able to predict this one data set. However, with the addition of the 86% precsion for highrisk loans its shows that the overall predicions were decent as it is above the industry standard of being above 85% threshold. When looking at the macro avg of presion that number increases to 93% and for the weighted avg the number jumps to 99%. These all indicate a strong prediction accuracy and precison for the machine. Therefore, most of the prosative predictions (healthy loan prediction) have been true with a very low number of false positives.
    * Recall:Lastly, the recall score for this model is 100% for healthy loans and 91% for highrisk loans. Once again with the highrisk loans having a slighlt lower but still very high percentage the 100% for healthy loans can be forgiven. The macro avg for recall was 95% with the weighted avg being 99%. Recall is all about how sensative the model is to positive outcomes. therefore, this model is highly senstaive to captureing postive scores and has very few false negative scores. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

