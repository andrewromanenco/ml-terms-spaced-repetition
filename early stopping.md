#fundamentals

A method for [[regularization|regularization]] that involves ending
[[training|training]] <em>before</em> training loss finishes
decreasing. In early stopping, you intentionally stop training the model
when the loss on a [[validation set|validation dataset]] starts to
increase; that is, when
[[generalization|generalization]] performance worsens.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._5" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

Early stopping may seem counterintuitive. After all, telling a model to halt
training while the loss is still decreasing may seem like telling a chef to
stop cooking before the dessert has fully baked. However, training a model for
too long can lead to <a href="#overfitting">overfitting</a>. That is, if you
train a model too long, the model may fit the training data so closely that
the model doesn't make good predictions on new examples.

</div>

<hr />
</section>

