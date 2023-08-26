# Model Evaluation
- Metrics are used to evaluate the outcome of your model. While there are recommendations on which metric is appropriate for the model you are currently using, each model object has different variations that may provide additional insight.
## Regression Metrics
   - Compares predicted output values with real output values
   - The difference between predicted and real value determines the model performance

## R2

- R2 measures the proportion of variance between values. It is somewhat related to correlation and has a value that ranges from -1 to 1. The higher the R2 value, the better the model.
RMSE -Root Mean Squared Error

- RMSE measures the standard deviation of prediction errors to target values. Another term for this is residuals. The lower the RMSE, the better the model.
Classification Metrics

   - Compares the predicted label with the real label value
   - Options to do comparison are either 2 label classification or multiple label classification

## Accuracy

- Accuracy is calculated by the total correct predictions divided by the total number of data points.
## Precision

- Precision is another metric related to accuracy but explains how good the model is at identifying the relevant label. Calculated by the number of true positives divided by the number of true and false positives.
## Recall

- Measures how many relevant labels are actually selected. Calculated by the number of true positives divided by the number of true positives and false negatives.
## Trade-Offs

- While default metrics for algorithms are good for initial evaluation, it is recommended to calculate several metrics to have a better understanding of overall model performance
