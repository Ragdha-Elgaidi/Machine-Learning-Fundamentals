# AutoGluon
- AutoGluon is a framework that automates the processing, creating, and tuning of ML models.
- It is part of a class of models call AutoML, which automates the machine learning workflow.
- In AutoGluon, the main parameters you use are: defining the target value for a dataset, and how long to train for.
-  It will automate everything else, trying a variety of models and parameters up to the time limit.
-   Because of its ease of use, it is a new way to easily create a baseline model. Another benefit of AutoGluon is the way it tries so many different models.
-    Providing metrics on all of the models, you can see how different models work on your data that would otherwise not be used.
## Code Example of AutoGluon
```py
import pandas as pd
from autogluon.tabular import TabularPredictor

df = pd.DataFrame(
    [[1, 2, 0], [3, 4, 1], [5, 6, 0], [7, 8, 1]],
    columns=["num", "amount", "target"]
)

predictor = TabularPredictor(label="target").fit(
    train_data=df,
    time_limit=60,
    presets="best_quality"
)
# output a summary of created models
predictor.fit_summary()

# evaluate best model from hyperparameter search
performance = predictor.evaluate(df)
```
