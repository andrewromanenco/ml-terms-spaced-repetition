
A [[semi-supervised learning|semi-supervised learning]] approach
particularly useful when all of the following conditions are true:

<ul>
<li>The ratio of [[unlabeled example|unlabeled examples]] to
[[labeled example|labeled examples]] in the dataset is high.</li>
<li>This is a classification problem ([[binary classification|binary]] or
[[multi-class classification|multi-class]]).</li>
<li>The [[data set or dataset|dataset]] contains two different sets of
predictive features that are independent of each other and complementary.</li>
</ul>

Co-training essentially amplifies independent signals into a stronger signal.
For instance, consider a [[classification model|classification model]] that
categorizes individual used cars as either <em>Good</em> or <em>Bad</em>. One set of
predictive features might focus on aggregate characteristics such as the year,
make, and model of the car; another set of predictive features might focus on
the previous owner&#39;s driving record and the car&#39;s maintenance history.

The seminal paper on co-training is <a href="https://www.cs.cmu.edu/%7Eavrim/Papers/cotrain.pdf">Combining Labeled and Unlabeled Data with
Co-Training</a> by
Blum and Mitchell.

