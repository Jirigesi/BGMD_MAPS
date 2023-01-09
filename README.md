# Leveraging Feature Bias for Scalable Misprediction Explanation of Machine Learning Models
This repository contains experimental data information and evaluation code for the paper "Leveraging Feature Bias for Scalable Misprediction Explanation of Machine Learning Models". Here, we present the details of the evaluation data and experimental results in Jupyter notebooks for easy reading.

## Experiment results
### Bias Guided Misprediction Diagnoser (BGMD) 
The experiment results of comparing BGMD and EXPLAIN are under folder "BGMD_result".

### Mispredicted Area UPweight Sampling (MAPS)
The experiment results of comparing MAPS, JTT and SMOTE are under folder "MAPS_result".

## Model parameters
### SVM 
C=1.0, kernel='rbf', degree=3, gamma='scale', coef0=0.0, shrinking=True, probability=False, tol=0.001, cache_size=200, class_weight=None, verbose=False, max_iter=-1, decision_function_shape='ovr', break_ties=False, random_state=None 

### Decision tree
criterion='gini', splitter='best', max_depth=None, min_samples_split=2, min_samples_leaf=1, min_weight_fraction_leaf=0.0, max_features=None, random_state=None, max_leaf_nodes=None, min_impurity_decrease=0.0, class_weight=None, ccp_alpha=0.0

### Random forest
n_estimators=100, *, criterion='gini', max_depth=None, min_samples_split=2, min_samples_leaf=1, min_weight_fraction_leaf=0.0, max_features='sqrt', max_leaf_nodes=None, min_impurity_decrease=0.0, bootstrap=True, oob_score=False, n_jobs=None, random_state=None, verbose=0, warm_start=False, class_weight=None, ccp_alpha=0.0, max_samples=None


## Data
Data size is big, so all data is stored in https://drive.google.com/drive/folders/1-m34KJz5bRQ-QO3N5lefu9axPFlFEDJ-?usp=sharing. We used five fold cross validation using below datasets (80%-train, 20%-test) and reports median number in the paper.

### Merge conflict data

| Name               | Ruby | Python | Java | PHP |
|--------------------|----------------|---------------|------------|------------|
| Number of features |      28        |       28      |     28     |   28       |         
| Instance number    |       40,129   |       49,453  | 26,699     |      50,342  |             

### Bug report close time prediction data

| Name               | BRCTP |
|--------------------|-------|
| Number of features |   21  |
| Instance number    |  1,481|

### Kaggle Data
| Name               | Bank_marketing | Hotel Booking | Job Change | Spam Email | Water Quality |
|--------------------|----------------|---------------|------------|------------|---------------|
| Number of features |      20        |    59         | 13         |   100      |       9       |
| Instance number    |        6,797   |      7,135    |   5,748    |    9,000   |       5,940   |




