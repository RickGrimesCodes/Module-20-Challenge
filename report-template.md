# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The purpose of the analysis is to determine whether a loan is healthy or not. 
The financial data revolves around loans, not revolving loans, but just static loans.
used all columns for training, with loan_size, interest_rate, borrower_income, dept_to_income, derogatory_marks and total_dept
being used for the x variable, and loan_status as the y variable. The model used was logistic regression.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    * Logistic regression for healthy loans had a high precision, recall and f1-score. 100%, 99% and 100% respectably
    * Logistic regression for high risk loans had a decent precision, good recall and decent f1-score. 84%, 94% and 89% respectably,
this is most likely due to less data for high risk loans.
 
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Since we used logistical regression, it seems to perform extremely well. High risk was less precise, but still a solid 84% accuracy.
It would be great to have more accuracy on a high-risk loan, because if a high-risk customer where to stop paying, it could be thousands lost for the company.