# CA04: Ensemble Models
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

### Address the following questions for Random Forest model and each algorithm in 4:
* Q.1 Write your observations about the Classifier’s behavior with respect to the \
number of estimators
* Q.2 Is there an optimal value of the estimator within the given range?

## 2.Finding Optimal Value of a key Ensemble Method Hyper-parameter
For Ensemble Models, one of the key hyper-parameter is number of “estimators”. \
find its best value by creating the following line graphs:

* Accuracy Vs. n_estimators
* AUC Vs. n_estimators

<br>
## 3. Build a Random Forest Models

Using Notebook, and the same data source from CA03, train a Random Forest Model. \
Using similar approach of Section 2 above, plot a graph of Accuracy vs. n_estimator \
and AUC Vs. n_estimator. Use n_estimator values as [50,100,150,200,250,300,350,400,450,500]. \
Keep all other hyperparameter values at default.

<br>

## 4. Build AdaBoost, Gradient Boost, and XGB.
Repeat the process of Section 3 above for AdaBoost, Gradient Boost, and XGB Classifiers.


## 5. Compare Performance

For the best values of Accuracy and AUC for four models (Random Forest, AdaBoost, \
Gradient Boost, XGB) in the previous steps, fill up the following table:

![image](https://user-images.githubusercontent.com/75411111/221019532-70b558ab-3389-426c-bc97-aff4c564c8c0.png)

