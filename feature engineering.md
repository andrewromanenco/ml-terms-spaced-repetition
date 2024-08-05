#fundamentals, #TensorFlow

A process that involves the following steps:

<ol>
<li>Determining which [[feature|features]] might be useful
in training a model.</li>
<li>Converting raw data from the dataset into efficient versions of
those features.</li>
</ol>

For example, you might determine that <code translate="no" dir="ltr">temperature</code> might be a useful
feature. Then, you might experiment with [[bucketing|bucketing]]
to optimize what the model can learn from different <code translate="no" dir="ltr">temperature</code> ranges.

Feature engineering is sometimes called
[[feature extraction|feature extraction]] or
[[featurization|featurization]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes-about-tensorflow." data-text=" Click the icon for additional notes about TensorFlow. " tabindex="-1">
Click the icon for additional notes about TensorFlow.
</h4>

<div class="expand-background">

In TensorFlow, feature engineering often means converting raw log file
entries to <a href="#tf.Example"><b>tf.Example</b></a> protocol buffers.
See also
<a href="https://github.com/tensorflow/transform" target="T">tf.Transform</a>.

</div>

<hr />
</section>

