
A generalization of [[least squares regression|least squares regression]]
models, which are based on
<a href="https://wikipedia.org/wiki/Gaussian_noise" target="T">Gaussian
noise</a>, to other
types of models based on other types of noise, such as
<a href="https://wikipedia.org/wiki/Shot_noise" target="T">Poisson noise</a>
or
categorical noise. Examples of generalized linear models include:

<ul>
<li>[[logistic regression|logistic regression]]</li>
<li>multi-class regression</li>
<li>least squares regression</li>
</ul>

The parameters of a generalized linear model can be found through
[[convex optimization|convex optimization]].

Generalized linear models exhibit the following properties:

<ul>
<li>The average prediction of the optimal least squares regression model is
equal to the average label on the training data.</li>
<li>The average probability predicted by the optimal logistic regression
model is equal to the average label on the training data.</li>
</ul>

The power of a generalized linear model is limited by its features. Unlike
a deep model, a generalized linear model cannot &quot;learn new features.&quot;

