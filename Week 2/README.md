# CS ML Maymester'18 PREWORK

## Objective
Comparing contrast original classifier with given params to "best version" - with the best params - then to the "optimized" version - with the best params and the best features. Then compare & contrast the results between the three. 

## Data
6000 songs (1500 from each consolidated genre: country, rock, jazz, pop). 

## Support Vector Machine
 - GridSearchCV to find the best params  { 'C': 10, 'gamma': 0.1 } sometimes { 'C': 1, 'gamma': 0.1 }
 - Select K Best to pick the top K features (k = 5: 'energy', 'speechiness', 'acousticness', 'valence', 'mode')

## Random Forest
 - GridSearchCV to find the best params {'max_features': 'sqrt', 'min_samples_split': 4, 'n_estimators': 100}
 - feature_importances_ to rank the features and then SelectFromModel those best features. 
 - RFE (Recursive Feature Elimination to also find the best features. 
 - SelectFromModel to pick the top features

## Logistic Regression
 - GridSearchCV to find the best params {'multi_class': 'ovr', 'solver': 'newton-cg'}
 - SelectFromModel to find the best features


## Video Walkthrough

Here's a walkthrough:

![Video Walkthrough](walkthrough.gif)
