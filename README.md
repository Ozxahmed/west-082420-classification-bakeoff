# Classification Bake Off

![Baking](https://media.giphy.com/media/xT0xePLIUyxnXso8co/giphy.gif)

## Challenge 

The goal for this challenge is to predict whether a person will default on their loan. In doing so, we want to utilize all of the different tools we have learned over the course: data cleaning, EDA, feature engineering/transformation, feature selection, hyperparameter tuning, and model evaluation.

## Data Files

In this repo you will find two csv files.

1. `train_data.csv`
This includes the features and target variables that you will use to train a predictive model

2. `test_features.csv`
This includes a testing set of data with the `default payment next month` column removed. You will make your final predictions on these observations and submit the predictions as a csv file.

## Feature Descriptions

* ID: ID of each client
* LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit
* SEX: Gender (1=male, 2=female)
* EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
* MARRIAGE: Marital status (1=married, 2=single, 3=others)
* AGE: Age in years
* PAY_0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)
* PAY_2: Repayment status in August, 2005 (scale same as above)
* PAY_3: Repayment status in July, 2005 (scale same as above)
* PAY_4: Repayment status in June, 2005 (scale same as above)
* PAY_5: Repayment status in May, 2005 (scale same as above)
* PAY_6: Repayment status in April, 2005 (scale same as above)
* BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
* BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
* BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
* BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
* BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
* BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)
* PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
* PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
* PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
* PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
* PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
* PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)
* default.payment.next.month: Default payment (1=yes, 0=no)

## Submissions
Save your predictions as a .csv file with the following pattern. 
- `credit_default_preds_yourteaminitials.csv`
- For example, if Erin and Joel were a team, their submission would look like `credit_default_preds_ehjc.csv`

- There are different ways to turn arrays to as .csv file.  You can use any method you choose, but be sure your submission has no heading, no index and one column. Your submission must match the number of records in the `test_features.csv`. A valid submission could look like below. 

0<br>
0<br>
1<br>
1<br>
...

***It is highly recommended that after saving your predictions to csv you import the csv file with `header=False` and ensure that the file only has 1 column and the same number of rows as the testing features!***

- You have until 10 Pacific/12 Central to build your best model using the training data. This challenge hasa hard cuttoff. Any late submissions will not be considered. 
- Submit your .csv file to the `#west-ds-082420` channel as a comment to the message from the `Bake Off Bot` before time is up. Any submissions after the deadline will be evaluated, but not included in the judging.

## Metrics
Test results will be scored by F1-score. The group which submitted predictions with the highest F1-score will be announced Monday morning. As a reward, they will receive a round of applause. 

## Share
- After submission, push your repo with your work to your forked repo! In this way, your peers will be able to gain valuable wisdom from the different tactics employed!

