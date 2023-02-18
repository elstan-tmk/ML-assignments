# CA03: Decision Tree Algorithm

The dataset is obtained from the Census Bureau and represents salaries of people along \
with seven demographic variables. The following is a description of our dataset: 
* Number of target classes: 2 ('>50K' and '<=50K') [ Labels: 1, 0 ] 
* Number of attributes (Columns): 7 
* Number of instances (Rows): 48,842 
* ![image](https://user-images.githubusercontent.com/75411111/219848977-8278b91b-8c19-488c-9287-95c50b89cba0.png)

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
<b>Definition:</b> Given a data of attributes together with its classes, a decision tree produces a
sequence of rules that can be used to classify the data. 
<br><br>
<b>Advantages:</b> Decision Tree is simple to understand and visualise, requires little data
preparation, and can handle both numerical and categorical data.
<br><br>
<b>Disadvantages:</b> Decision tree can create complex trees that do not generalize well, and
decision trees can be unstable because small variations in the data might result in a
completely different tree being generated.
<br><br>
Use “DecisionTreeClassifier” algorithm from scikit learn. Find details of sklearn tree
algorithm below. Scitkit Learn implements an optimized version of CART algorithm and can
be used for binary class as well as multi-class classifications. It can be used for
classification, as well as regression. Study the following link thoroughly, including Section
1.10.5 (Tips on Practical Use).<br>
https://scikit-learn.org/stable/modules/tree.html#tree-algorithms-id3-c4-5-c5-0-and-cart 
<br>
<br>
## 4. Evaluate Decision Tree Performance
Calculate and display the following. Do all of these inside your Notebook.
* Confusion Matrix (TP, TN, FP, FN … etc.)
* Accuracy, Precision, Recall, F1 Score


## 5. Tune Decision Tree Performance

Learn about all hyper-parameters and methods of Scikit Learn DecisionTreeClassifier
algorithm at:<br>
https://scikitlearn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html#sklearn.tree.DecisionTreeClassifier


Try varying FOUR of the hyperparameters manually, as per the following table, and train /
score your model for each set of these hyperparameters. Record your Tree’s performance
with respect to each of these sets of hyperparameters in the Model Performance section of
the following table.
<br>
Four Hyperparameters to vary:
<br>
* Split Criteria – ‘Entropy’ or ‘Gini Impurity’
* Maximum Features – The number of features to consider when looking for the best
split. If float, then max_features is a fraction
and max(1, int(max_features * n_features_in_)) features are considered at each split.
*  Minimum Sample Leaf – Minimum of samples in a leaf node to stop further splitting
(becomes a leaf node)
*  Maximum Depth – Maximum depth of the tree allowed
<br>
For Run 1, vary Run 1 columns only and keep other columns to "default". <br>
For Run 2, use the BEST hyper-parameter value of Split Criteria from Run 1, <br>
For Run 3, use the BEST hyper-parameter values of Split Criteria and Minimum Sample Leaf from Run 1&2, <br>
For Run 4, use the Best values of Split Crteria, Minimum Sample Leaf, Maximum Feature from previous runs. <br><br>
Judge the BEST hyper-parameter values with respect to "Accuracy".<br>
For each run, your will “fill up” a table with all performance parameters as follows. <br>
So, there will be 4 tables like this for 4 runs, based on the number of rows of the hyper-parameters.<br>
For the Split Criteria, obviously you will have two rows only.<br>
<br>
To determine the BEST hyper-parameter value, create line-graphs with the hyper-parameter
as x-axis and accuracy as y-axis. A sample is provided below for a graph of Minimum
Sample Leaf Vs. Accuracy. You don’t need graph Split Criteria Vs. Accuracy. So you will
have 3 graphs altogether.<br>
<br>
You can use the model training and testing in a loop for each of the hyper-parameters as
the code sample below. You can modify the code to capture each of the performance
parameters and display them in the table format inside your notebook like the above
figure. <br>

## 6. Visualize Your Best Decision Tree using GraphViz
Get the detail of how to do this from the following link:<br>
https://medium.com/@rnbrown/creating-and-visualizing-decision-trees-with-python-f8e8fa394176
<br><br>
Once you have the best hyper-parameters from 4 runs, you will know the hyper-parameter
combination of your BEST-performing Tree with respect to “accuracy”. Use these set of
hyper-parameters to build the BEST Tree, record it’s performance parameter (all of them)
and then “visualize” this best tree.

## 7. Prediction using your “trained” Decision Tree Model
Based on the Performance Tuning effort in the previous section, pick your BEST
PERFORMING TREE. Now make prediction of a “new” individual’s Income Category ( <=50K,
or >50K ) with the following information. <br>
* Hours Worked per Week = 48
* Occupation Category = Mid - Low
* Marriage Status & Relationships = High
* Capital Gain = Yes
* Race-Sex Group = Mid
* Number of Years of Education = 12
* Education Category = High
* Work Class = Income
* Age = 58

