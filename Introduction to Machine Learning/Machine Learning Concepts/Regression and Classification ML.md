# Regression and Classification ML
## Regression
   - Prediction is an estimate of the target value based on feature values
   - Target values are a quantity
   - Metric of success is the distance or score of the predicted value to the target value
```py
from sklearn.linear_model import LinearRegression

features = [[5, 3.4, 6], [1, 0.4, 10], [2, 0.1, 1]]
target = [1.4, 0.5, 1]

reg = LinearRegression().fit(features, target)

# Score model with features and target
print(reg.score(features, target))
# Predict new values based on features
print(reg.predict(features))


# output
1.0
[1.4 0.5 1. ]
```
## Classification
   - Prediction are labels based on the feature values
   - Target values are a discrete number of labels, which can be 2 or more
   - Metric of success is related to labeling correctly when compared to target values
```py
from sklearn.linear_model import RidgeClassifier

features = [[5, 3.4, 6], [1, 0.4, 10], [2, 0.1, 1]]
target = [0, 1, 1]

# Used alpha parameter in model creation
clf = RidgeClassifier(alpha=3.0).fit(
features, target
)

# Score model with features and target
print(clf.score(features, target))
# Predict new values based on features
print(clf.predict(features))


# output
1.0
[0 1 1
```
