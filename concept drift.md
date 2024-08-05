
A shift in the relationship between features and the label.
Over time, concept drift reduces a model&#39;s quality.

During training, the model learns the relationship between the features and
their labels in the training set. If the labels in the training set are
good proxies for the real-world, then the model <em>should</em> make good
real world predictions. However, due to concept drift, the model&#39;s
predictions tend to degrade over time.

For example, consider a [[binary classification|binary classification]]
model that predicts whether or not a certain car model is &quot;fuel efficient.&quot;
That is, the features could be:

<ul>
<li>car weight</li>
<li>engine compression</li>
<li>transmission type</li>
</ul>

while the label is either:

<ul>
<li>fuel efficient</li>
<li>not fuel efficient</li>
</ul>

However, the concept of &quot;fuel efficient car&quot; keeps
changing. A car model labeled <em>fuel efficient</em> in 1994 would almost certainly
be labeled <em>not fuel efficient</em> in 2024. A model suffering from concept drift
tends to make less and less useful predictions over time.

Compare and contrast with [[nonstationarity|nonstationarity]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._3" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

To compensate for concept drift, retrain models faster than the <i>rate</i> of
concept drift. For example, if concept drift reduces model precision by a
meaningful margin every two months, then retrain your model more frequently
than every two months.

</div>

<hr />
</section>

