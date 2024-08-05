
A model design flaw in which a [[feature|feature]] is a proxy for the
[[label|label]]. For example, consider a
[[binary classification|binary classification]] model that predicts
whether or not a prospective customer will purchase a particular product.
Suppose that one of the features for the model is a Boolean named
<code translate="no" dir="ltr">SpokeToCustomerAgent</code>. Further suppose that a customer agent is only
assigned <em>after</em> the prospective customer has actually purchased the
product. During training, the model will quickly learn the association
between <code translate="no" dir="ltr">SpokeToCustomerAgent</code> and the label.

