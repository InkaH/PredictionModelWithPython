This is an exercise of course Machine Learning with Python.

This prediction model predicts which people are likely to develop diabetes with 70% or greater accuracy using a sligthly modified Pima Indians Diabetes Data Set from UCI Machine Learning Repository. Scikit-learn library is used in training and evaluation.

Steps:

1) Prepare Data:
  Read in demo data
  Identify correlated features
  Clean data
  Mold data
  Check True/False ratio
  
2) Select Algorithm
  We want to predict, so it must be supervised algorithm
  Our result type is classification, and particularly binary classification -> algorithm must support that
  Eliminate "ensemble" algorithm as this is initial training
  Choose basic, not enhanced, as this is a basic exercise..
  --> let's select Naive Bayes as it's simple to understand, it's fast and it's stable
  
3) Train the Model
  Split data set to 70% training set and 30% testing set
  Select training features
  verify predicted value was split well
  post-split data preparation:
    hidden missing values? missing data is common problem, false zeroes cause bias
    replace with mean/median, replace with expert knowledge derived value
 And train!
  
4) Test model's accuracy
    Improve performance:
      adjust current algorithm
      get more data or improve data
      improve training by preventing overfitting by using regularization hyperparameter and cross validation
      switch algorithm?
      -> split data into training, test and validation data? not enough data usually for this
      -> K-Fold Cross Validation
        for each fold, determine best hyperparameter value
        next. set model hyperparameter value to average best
        = Use Algorithm CV variants (algorithm + cross validation libraries)
        
  
    
