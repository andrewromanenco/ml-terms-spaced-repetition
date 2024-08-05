#df

A method of picking items from a set of candidate items in which the same
item can be picked multiple times. The phrase &quot;with replacement&quot; means
that after each selection, the selected item is returned to the pool
of candidate items. The inverse method, <strong>sampling without replacement</strong>,
means that a candidate item can only be picked once.

For example, consider the following fruit set:

<pre class="prettyprint" translate="no" dir="ltr">
fruit = {kiwi, apple, pear, fig, cherry, lime, mango}
</pre>

Suppose that the system randomly picks <code translate="no" dir="ltr">fig</code> as the first item.
If using sampling with replacement, then the system picks the
second item from the following set:

<pre class="prettyprint" translate="no" dir="ltr">
fruit = {kiwi, apple, pear, fig, cherry, lime, mango}
</pre>

Yes, that&#39;s the same set as before, so the system could potentially
pick <code translate="no" dir="ltr">fig</code> again.

If using sampling without replacement, once picked, a sample can&#39;t be
picked again. For example, if the system randomly picks <code translate="no" dir="ltr">fig</code> as the
first sample, then <code translate="no" dir="ltr">fig</code> can&#39;t be picked again. Therefore, the system
picks the second sample from the following (reduced) set:

<pre class="prettyprint" translate="no" dir="ltr">
fruit = {kiwi, apple, pear, cherry, lime, mango}
</pre>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._15" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

The word <i>replacement</i> in <b>sampling with replacement</b> confuses
many people.  In English, <i>replacement</i> means "substitution."
However, <b>sampling with replacement</b> actually uses the French definition
for <i>replacement</i>, which means "putting something back."

The English word <i>replacement</i> is translated as the French
word <i>remplacement</i>.
</div>

<hr />
</section>

