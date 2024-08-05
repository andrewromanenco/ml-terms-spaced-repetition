#df

A training algorithm where weak models are trained to iteratively
improve the quality (reduce the loss) of a strong model. For example,
a weak model could be a linear or small decision tree model.
The strong model becomes the sum of all the previously trained weak models.

In the simplest form of gradient boosting, at each iteration, a weak model
is trained to predict the loss gradient of the strong model. Then, the
strong model&#39;s output is updated by subtracting the predicted gradient,
similar to [[gradient descent|gradient descent]].

<div>
$$F_{0} = 0$$
$$F_{i+1} = F_i - \xi f_i $$
</div>

where:

<ul>
  <li>$F_{0}$ is the starting strong model.</li>
  <li>$F_{i+1}$ is the next strong model.</li>
  <li>$F_{i}$ is the current strong model.</li>
  <li>$\xi$ is a value between 0.0 and 1.0 called <a
      href="#shrinkage"><b>shrinkage</b></a>,
      which is analogous to the
      <a href="#learning_rate"><b>learning rate</b></a> in
      gradient descent.</li>
  <li>$f_{i}$ is the weak model trained to predict the loss gradient of
      $F_{i}$.</li>
</ul>

Modern variations of gradient boosting also include the second derivative
(Hessian) of the loss in their computation.

[[decision tree|Decision trees]] are commonly used as weak models in
gradient boosting. See
[[gradient boosted (decision) trees (GBT)|gradient boosted (decision) trees]].

