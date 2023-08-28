# Separating Data

- We're still in our quest for an algorithm that will help us pick the best model that separates our data. Now that we have ways of generating a probability for each classification, we can use these probabilities to help us evaluate our model.

- One method we can use for this is called maximum likelihood. In this approach, we pick the model that gives the existing labels in our historical data (which we know are correct) the highest probability.
## Using Probability to Separate Data
- The key idea is that we want to calculate P(all)P(all), which is the product of all the independent probabilities of each point. This helps indicate how well the model performs in classifying all the points. To get the best model, we will want to maximize this probability
