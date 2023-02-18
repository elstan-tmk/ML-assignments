# CA03: Decision Tree Algorithm

The dataset is obtained from the Census Bureau and represents salaries of people along \
with seven demographic variables. The following is a description of our dataset: 
* Number of target classes: 2 ('>50K' and '<=50K') [ Labels: 1, 0 ] 
* Number of attributes (Columns): 7 
* Number of instances (Rows): 48,842 

## 1. Data Sources:
"https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true"
<br>

Training and Test Data: There is a column indicating the rows to be used as “Training Data”
and “Testing Data”. Programmatically create the Training and Testing datasets as
separate dataframes in the code based on this column value.

### Address the following questions during the model building:
* Q.1 Why does it makes sense to discretize columns for this problem?
* Q.2 What might be the issues (if any) if we DID NOT discretize the columns.
* Q.3 Decision Tree Hyper-parameter variation vs. performance
* Q.4 How long was your total run time to train the best model?
* Q.5 Did you find the BEST TREE?
* Q.6 Write your observations from the visualization of the best tree
* Q.7 Will this Tree “overfit”? (Hint: Is this tree “fully grown”)
* Q.8 What is the probability that your prediction for this person is correct?

## 2. Data Quality Analysis (DQA)
* Perform a Data Quality Analysis to find missing values, outliers, NaNs etc.
* Display descriptive statistics of each column
* Create a Data Quality Report
* Perform necessary data cleansing and transformation based on your observations from the data quality analysis

## 3. Build Decision Tree Classifier Models
