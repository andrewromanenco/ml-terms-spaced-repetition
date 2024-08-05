
An algorithm for predicting a model&#39;s ability to
[[generalization|generalize]] to new data. The <em>k</em> in k-fold refers to the
number of equal groups you divide a dataset&#39;s examples into; that is, you train
and test your model k times. For each round of training and testing, a
different group is the test set, and all remaining groups become the training
set. After k rounds of training and testing, you calculate the mean and
standard deviation of the chosen test metric(s).

For example, suppose your dataset consists of 120 examples. Further suppose,
you decide to set k to 4. Therefore, after shuffling the examples,
you divide the dataset into four equal groups of 30 examples and conduct four
training/testing rounds:


![[ images/k-folds.png ]]


For example, [[Mean Squared Error (MSE)|Mean Squared Error (MSE)]] might
be the most meaningful metric for a linear regression model. Therefore, you
would find the mean and standard deviation of the MSE across all four rounds.

