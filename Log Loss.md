#fundamentals

The [[loss function|loss function]] used in binary
[[logistic regression|logistic regression]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-math._1" data-text=" Click the icon to see the math. " tabindex="-1">
Click the icon to see the math.
</h4>

<div class="expand-background">

The following formula calculates Log Loss:


<div>
$$\text{Log Loss} = \sum_{(x,y)\in D} -y\log(y') - (1 - y)\log(1 - y')$$
</div>

where:

<ul>
  <li>
  \((x,y)\in D\) is the dataset containing many labeled
  examples, which are \((x,y)\) pairs.
  </li>
  <li>
    \(y\) is the label in a labeled example. Since this is logistic regression,
    every value of \(y\) must either be 0 or 1.
  </li>
  <li>
    \(y'\) is the predicted value (somewhere between 0 and 1, exclusive),
    given the set of features in \(x\).
  </li>
</ul>

</div>

<hr />
</section>

