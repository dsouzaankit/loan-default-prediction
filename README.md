# loan-default-prediction
Predict customers who are likely to default on their very first loan

Problem Statement:

The data includes both information that were known at the time of application and repayment information for the loan. 
Each of the loans included were the first loan that the customer took.

Please look at the information and do the following:

A. Calculate the realized profit based only on the information provided

B. Recommend a credit policy that dictates (sets business rules for) who we should approve and what loan amount we should allow them to take. This policy should use some (but not necessarily all) of the data available at application. Be sure to detail any assumptions or other factors taken into consideration

C. Comment on any additional information that would be desired in setting credit policy

My Approach:

Dataset contains all approved customers with mostly Good to Excellent credit rating (>=0.7), but still 17% people defaulted and we saw net Loss of $8,370
Mean Loss/customer (-$14.5) is 5-6x of mean Profit/customer ($2.8)

I fit a Logistic Regression model on available data, which predicted whether a new user will default or not

Assuming new users behave similarly to past ones, I identified key drivers behind loan defaults & decided on individual outcomes
Resulted into Losses turning to Profits, with 60% loss of New customers

Individual models were fit for $10, $20 & $30 loan amounts to determine key factors in each case
