#fundamentals

Reality.

The thing that actually happened.

For example, consider a [[binary classification|binary classification]]
model that predicts whether a student in their first year of university
will graduate within six years. Ground truth for this model is whether or
not that student actually graduated within six years.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._7" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

We assess model quality against ground truth. However, ground truth
is not always completely, well, truthful. For example, consider the
following examples of potential imperfections in ground truth:

<ul>
  <li>In the graduation example, are we <i>certain</i> that the graduation
      records for each student are always correct?  Is the university's
      record-keeping flawless?</li>
  <li>Suppose the label is a floating-point value measured by instruments
      (for instance, barometers). How can we be sure that each instrument
      is calibrated identically or that each reading was taken under the same
      circumstances?</li>
  <li>If the label is a matter of human opinion, how can we be sure that
      each human <a href="#rater"><b>rater</b></a> is evaluating events in the
      same way?  To improve consistency, <i>expert</i> human raters sometimes
      intervene.</li>
</ul>

</div>

<hr />
</section>

