This is an exercise of course Machine Learning with Python.

This prediction model predicts which people are likely to develop diabetes with 70% or greater accuracy using a sligthly modified Pima Indians Diabetes Data Set from UCI Machine Learning Repository. Scikit-learn library is used in training and evaluation.

Steps:

1) Prepare Data:<br>
  Read in demo data<br>
  Identify correlated features<br>
  Clean data<br>
  Mold data<br>
  Check True/False ratio<br>
  <br>
2) Select Algorithm<br>
  We want to predict, so it must be supervised algorithm<br>
  Our result type is classification, and particularly binary classification -> algorithm must support that<br>
  Eliminate "ensemble" algorithm as this is initial training<br>
  Choose basic, not enhanced, as this is a basic exercise..<br>
  --> let's select Naive Bayes as it's simple to understand, it's fast and it's stable<br>
  
3) Train the Model<br>
  Split data set to 70% training set and 30% testing set<br>
  Select training features<br>
  verify predicted value was split well<br>
  post-split data preparation:<br>
    hidden missing values? missing data is common problem, false zeroes cause bias<br>
    replace with mean/median, replace with expert knowledge derived value<br>
 And train!<br>
  
4) Test model's accuracy<br>
    Improve performance:<br>
      adjust current algorithm<br>
      get more data or improve data<br>
      improve training by preventing overfitting by using regularization hyperparameter and cross validation<br>
      switch algorithm?<br>
      -> split data into training, test and validation data? not enough data usually for this<br>
      -> K-Fold Cross Validation<br>
        for each fold, determine best hyperparameter value<br>
        next. set model hyperparameter value to average best<br>
        = Use Algorithm CV variants (algorithm + cross validation libraries)<br>
        
  
    
