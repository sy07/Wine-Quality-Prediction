# Wine-Quality-Prediction

## About
This dataset is taken from UCI Machine Learning repository.

This dataset is about classifying quality of wine by using features like: 
- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- density
- pH
- sulphates
- alcohol

we have to classify the quality of wine in between 1-10.

## What I have done
The data which I have taken is already clean data so there's nothing to clean.
So, I split data into 2 parts:
- X contains features like fixed acidity,volatile acidity,citric acid,residual sugar,chlorides etc.
- y contains target which we have to classify.

Then I trained models using X and y.
1) Linear Regression
- Trained data using *linear regression* with default hyperparameter
- Mean Absolute Error: 0.5883868297349942
- Mean Squared Error: 0.5799025320314125
- Mean Squared Log Error: 0.012869847080140091
- R2 Score 0.26132052039754317

2) Logistic Regression
- Trained data using *logistic regression* with hyperparameter solver=newton-cg
- F1 score 0.00,0.00,0.51,0.62,0.27,0.00,0.00
- Accuracy: 0.52

3) K Nearest Neighbors
- Trained data using *K Nearest Neighbors* with hyperparameter n_neighbors=1
- F1 score 0.31,0.17,0.53,0.63,0.46,0.32,0.00
- Accuracy: 0.54

4) Decision Tree
- Trained data using *Decision Tree* with hyperparameter max_depth=15, min_samples_leaf=5, criterion='entropy'
- F1 score 0.00,0.20,0.58,0.59,0.45,0.19,0.00
- Accuracy: 0.53

5) Random Forest
- Trained data using *Random Forest* with hyperparameter n_estimators=100, criterion='entropy'
- F1 score 0.00,0.36,0.65,0.70,0.58,0.42,0.00
- Accuracy: 0.65

## Conclusion

After training data on multiple algorithms. I came to conclusion that Random Forest understood the dataset best.

