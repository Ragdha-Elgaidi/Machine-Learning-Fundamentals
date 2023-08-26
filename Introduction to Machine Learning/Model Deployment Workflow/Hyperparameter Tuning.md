# Hyperparameter Tuning
- Hyperparameters are the model's configuration parameters that alter how it trains. Changing hyperparameters often increases or decreases the performance of a model. Generally, it is recommended to start working with hyperparameters by first starting with the default parameters. This creates a baseline performance, where you can compare all further optimizations on. For the majority of models, there are many parameters to choose from. This makes it hard to find the right combination that provides the best performance.

- To help solve which of the unlimited parameters are best, two methods will search for the right parameters automatically. Grid search searches parameters in a deterministic fashion across all options. Randomized search randomly selects parameters from available options.
## Code Example
```py
from sklearn.tree import DecisionTreeClassifier

# create baseline with default params
model = DecisionTreeClassifier()

# create model with hyperparameters
model = DecisionTreeClassifier(
    max_depth=10,
    criterion="entropy"
)
```
