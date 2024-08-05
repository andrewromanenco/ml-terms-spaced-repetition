#fundamentals

A type of [[regression model|regression model]] that predicts a probability.
Logistic regression models have the following characteristics:

<ul>
<li>The label is [[categorical data|categorical]]. The term logistic
regression usually refers to <strong>binary logistic regression</strong>, that is,
to a model that calculates probabilities for labels with two possible values.
A less common variant, <strong>multinomial logistic regression</strong>, calculates
probabilities for labels with more than two possible values.</li>
<li>The loss function during training is [[Log Loss|Log Loss]].
(Multiple Log Loss units can be placed in parallel for labels
with more than two possible values.)</li>
<li>The model has a linear architecture, not a deep neural network.
However, the remainder of this definition also applies to
[[deep model|deep models]] that predict probabilities
for categorical labels.</li>
</ul>

For example, consider a logistic regression model that calculates the
probability of an input email being either spam or not spam.
During inference, suppose the model predicts 0.72. Therefore, the
model is estimating:

<ul>
<li>A 72% chance of the email being spam.</li>
<li>A 28% chance of the email not being spam.</li>
</ul>

A logistic regression model uses the following two-step architecture:

<ol>
<li>The model generates a raw prediction (y&#39;) by applying a linear function
of input features.</li>
<li>The model uses that raw prediction as input to a
[[sigmoid function|sigmoid function]], which converts the raw
prediction to a value between 0 and 1, exclusive.</li>
</ol>

Like any regression model, a logistic regression model predicts a number.
However, this number typically becomes part of a binary classification
model as follows:

<ul>
<li>If the predicted number is <em>greater</em> than the
[[classification threshold|classification threshold]], the
binary classification model predicts the positive class.</li>
<li>If the predicted number is <em>less</em> than the classification threshold,
the binary classification model predicts the negative class.</li>
</ul>

