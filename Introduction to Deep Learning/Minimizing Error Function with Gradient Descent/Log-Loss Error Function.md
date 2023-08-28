# Log-Loss Error Function 
## Discrete and Continuous Errors

- One approach to reducing errors might be to simply count the number of errors and then make changes until the number of errors is reduced. But taking a discrete approach like this can be problematic—for example, we could change our line in a way that gets closer to the solution, but this change might not (by itself) improve the number of misclassified points.

- Instead, we need to construct an error function that is continuous. That way, we can always tell if a small change in the line gets us closer to the solution. We'll do that in this lesson using the log-loss error function. Generally speaking, the log-loss function will assign a large penalty to incorrectly classified points and small penalties to correctly classified points. For a point that is misclassified, the penalty is roughly the distance from the boundary to the point. For a point that is correctly classified, the penalty is almost zero.

- we can then calculate a total error by adding all the errors from the corresponding points. Then we can use gradient descent to solve the problem, making very tiny changes to the parameters of the line in order to decrease the total error until we have reached an acceptable minimum.
