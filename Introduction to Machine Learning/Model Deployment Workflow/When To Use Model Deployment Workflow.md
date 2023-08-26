# When To Use Model Deployment Workflow
- There are several scenarios where following a strict model deployment will be difficult.

- In the case of having small datasets, it may be so small that you will be unable to perform a train/test or train/validation/test data split. In these cases, building a model will be difficult regardless, because you may lack the data to even be able to train the model successfully.

- There may be data that is already cleaned and processed. Which in this case, it may be useful and insightful personally to clean and process the data yourself. Often times you can skip doing this step altogether. Mainly because the data is already in an adequate state.

- Only use new metrics if you understand how they relate to your data

- Lastly, if using the default parameters of a model work well for you, then spending the time and effort doing a hyperparameter search may not be worth it.
