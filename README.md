**Credit Risk Classification

For this challenge, we had to create a linear regression model using a CSV about safe and high-risk loans. Once the model was made, we needed to write an analysis following the below criteria.

**Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this challenge. This might include:

Explain the purpose of the analysis.
Explain what financial information the data was on and what you needed to predict.
Provide basic information about the variables you were trying to predict (e.g., value_counts).
Describe the stages of the machine learning process you went through as part of this analysis.
Briefly touch on any methods you used (e.g., LogisticRegression, or any other algorithms).


Analysis:
The purpose of this analysis is to determine the health of future loans. This means how well a loan worked out for the company. Is it being paid off on time? Or not at all? How profitable is the loan? These are the questions required to analyze a loan's health. These were the columns in our dataframe: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, loan_status. These columns provided information we used to create a linear regression to notice the trends of past loans to predict future loans. By feeding the machine learning with this information, we were able to gather data regarding how well loan health is predicted and allowed us to gain an understanding of the accuracy of our choices. We used an sklearn model to train our machine with an 80/20 split between training and testing. Using logistic regression made this all possible as it allowed us to create predictions for loan statuses and that allowed us to use a confusion matrix to check how accurate and precise our predictions are.

**Results
Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1:

Description of Model 1 Accuracy, Precision, and Recall scores.


Accuracy: Within this dataset and confusion matrix, the accuracy was 99% on the F1-score. Having such high accuracy but being short of perfect is an incredible achievement to how well the machine functions. This means the model is exceptional at making correct predictions across all classes, be it a true positive case or true negative.

Precision: When it comes to precision, 100% of all healthy loans were predicted while only 86% of high-risk loans were predicted. Normally, 100% is a bad sign as it determines you are only able to predict this one data set. However, with the addition of the 86% precision for high-risk loans, it shows that the overall predictions were decent as it is above the industry standard of being above an 85% threshold. When looking at the macro avg of precision, that number increases to 93%, and for the weighted avg, the number jumps to 99%. These all indicate a strong prediction accuracy and precision for the machine. Therefore, most of the positive predictions (healthy loan prediction) have been true with a very low number of false positives.

Recall: Lastly, the recall score for this model is 100% for healthy loans and 91% for high-risk loans. Once again with the high-risk loans having a slightly lower but still very high percentage, the 100% for healthy loans can be forgiven. The macro avg for recall was 95% with the weighted avg being 99%. Recall is all about how sensitive the model is to positive outcomes. Therefore, this model is highly sensitive to capturing positive scores and has very few false negative scores.

**Summary

Summarize the results of the machine learning models and include a recommendation on the model to use, if any. For example:

Which one seems to perform best? How do you know it performs best?

Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's or predict the 0's?)

If you do not recommend any of the models, please justify your reasoning.


Summary: For this challenge, we only used the logistic regression model. Based on the results mentioned above, this model worked out very well in determining which loans were healthy and high risk with accurate predictability. Therefore, I would recommend using this model as it is simple to follow and effective. This model does solve the problem we have because it accurately predicts both healthy and high-risk loans. When it comes to loans, it is most important to predict which loans will be high risk because these are the ones that will cause a company to lose money if they are not accurately predicted. This model did a very good job at catching the errors and provided an exceptionally high predictability for all outcomes.
