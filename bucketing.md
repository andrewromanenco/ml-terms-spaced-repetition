#fundamentals

Converting a single [[feature|feature]] into multiple binary features
called <strong>buckets</strong> or <strong>bins</strong>,
typically based on a value range. The chopped feature is typically a
[[continuous feature|continuous feature]].

For example, instead of representing temperature as a single
continuous floating-point feature, you could chop ranges of temperatures
into discrete buckets, such as:

<ul>
<li>&lt;= 10 degrees Celsius would be the &quot;cold&quot; bucket.</li>
<li>11 - 24 degrees Celsius would be the &quot;temperate&quot; bucket.</li>
<li>&gt;= 25 degrees Celsius would be the &quot;warm&quot; bucket.</li>
</ul>

The model will treat every value in the same bucket identically. For
example, the values <code translate="no" dir="ltr">13</code> and <code translate="no" dir="ltr">22</code> are both in the temperate bucket, so the
model treats the two values identically.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._1" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

If you represent temperature as a continuous feature, then the model
treats temperature as a single feature. If you represent temperature
as three buckets, then the model treats each bucket as a separate feature.
That is, a model can learn separate relationships of each bucket to the
<a href="#label"><b>label</b></a>. For example, a
<a href="#linear_regression"><b>linear regression</b></a> model can learn
separate <a href="#weight"><b>weights</b></a> for each bucket.


Increasing the number of buckets makes your model more complicated by
increasing the number of relationships that your model must learn.
For example, the cold, temperate, and warm buckets are essentially
three separate features for your model to train on. If you decide to add
two more buckets--for example, freezing and hot--your model would
now have to train on five separate features.

How do you know how many buckets to create, or what the ranges for each
bucket should be? The answers typically require a fair amount of
experimentation.

</div>

<hr />
</section>


