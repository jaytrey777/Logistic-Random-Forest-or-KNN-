# Logistic Random Forest or KNN?

Using the Wisconsin Breast Cancer Dataset, predict whether a tumor cell is malignant (m) or benign (b).

Link to dataset: https://docs.google.com/spreadsheets/d/e/2PACX-1vTZf6XIYPLjxmCS8BzzEot1DaW4ns7P2q1CVqnZ6qw9f-A3bkCPbXX3H9vOE2_zrGKSxy4ZMaTf7lt4/pub?gid=594194017&single=true&output=csv

Your task in this assignment will be to build the best model you can to diagnose cancer and report on your results.

1.  Logistic Regression

    - Start by creating and evaluating a default logistic regression model using appropriate metrics and a confusion matrix.

    - Then, use GridSearchCV to tune the penalty type and C values (inverse regularization strength) for the model to find the optimal combination of hyperparameter values, and evaluate the resulting tuned model.

- NOTE: Make sure to select an appropriate solver that would allow you to explore both L1 and L2 penalties. In order to choose the right solver, LogisticRegression documentation to see which solvers support which penalty types.

- When you create your parameter dictionary:

    - Your penalties should be ['l1', 'l2']

    - Your C values should be logarithmic: [.0001, .001, .01, .1, 1, 10, 100, 1000, 10000]

- Make sure you have evaluated both the default and the tuned versions using appropriate metrics and a confusion matrix.
- In a text cell, address these questions for your logistic regression models:

  - Which hyperparameters did you tune?
  - What values for those hyperparameters led to the best-tuned model?


2.  K-Nearest Neighbors

  - Start by creating and evaluating a default knn model using appropriate metrics and a confusion matrix

  - Then, use GridSearchCV to tune the model.

- Check the KNN documentation to choose hyperparameters to tune. 
- Make sure you have evaluated both the default and the tuned versions using appropriate metrics and a confusion matrix.
- In a text cell, address these questions for your KNN models:

  - Which hyperparameters did you tune?
  - What values for those hyperparameters led to the best-tuned model?


3. Random Forest

- Start by creating and evaluating a default random forest model using appropriate metrics and a confusion matrix

- The, use GridSearchCV to tune the model.

- Check the random forest documentation to choose hyperparameters to tune. 
- Make sure you have evaluated both the default and the tuned versions using appropriate metrics and a confusion matrix.

- In a text cell, address these questions for your random forest models:

  - Which hyperparameters did you tune?
  - What values for those hyperparameters led to the best-tuned model?


4. Answer these questions in a text cell at the end of your notebook:

- What do 'false positives' and 'false negatives' mean for this problem? 
- Which is worse?
- Which of your models would you recommend for production? 
- Which metric or metrics did you use to decide that, and why?
