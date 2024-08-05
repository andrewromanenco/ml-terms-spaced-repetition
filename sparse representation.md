#language, #fundamentals

Storing only the <em>position(s)</em> of nonzero elements in a sparse feature.

For example, suppose a categorical feature named <code translate="no" dir="ltr">species</code> identifies the 36
tree species in a particular forest. Further assume that each
[[example|example]] identifies only a single species.

You could use a one-hot vector to represent the tree species in each example.
A one-hot vector would contain a single <code translate="no" dir="ltr">1</code> (to represent
the particular tree species in that example) and 35 <code translate="no" dir="ltr">0</code>s (to represent the
35 tree species <em>not</em> in that example). So, the one-hot representation
of <code translate="no" dir="ltr">maple</code> might look something like the following:


<img
src="images/One-HotRepresentationOfASparseFeature.png"
     loading="lazy"
     alt="A vector in which positions 0 through 23 hold the value 0, position
          24 holds the value 1, and positions 25 through 35 hold the value 0.">


Alternatively, sparse representation would simply identify the position of the
particular species. If <code translate="no" dir="ltr">maple</code> is at position 24, then the sparse representation
of <code translate="no" dir="ltr">maple</code> would simply be:

<pre translate="no" dir="ltr">
24
</pre>

Notice that the sparse representation is much more compact than the one-hot
representation.
<aside class="note"><strong>Note:</strong><span> You shouldn&#39;t pass a sparse representation as a direct feature input
to a model. Instead, you should convert the sparse representation into a
one-hot representation before training on it.</span></aside>
<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-a-slightly-more-complex-example." data-text=" Click the icon for a slightly more complex example. " tabindex="-1">
Click the icon for a slightly more complex example.
</h4>

<div class="expand-background">

Suppose each example in your model must represent the words—but not
the order of those words—in an English sentence.
English consists of about 170,000 words, so English is a categorical
feature with about 170,000 elements. Most English sentences use an
extremely tiny fraction of those 170,000 words, so the set of words in a
single example is almost certainly going to be sparse data.


Consider the following sentence:

<pre translate="no" dir="ltr">
My dog is a great dog
</pre>


You could use a variant of one-hot vector to represent the words in this
sentence. In this variant, multiple cells in the vector can contain
a nonzero value. Furthermore, in this variant, a cell can contain an integer
other than one. Although the words "my", "is", "a", and "great" appear only
once in the sentence, the word "dog" appears twice. Using this variant of
one-hot vectors to represent the words in this sentence yields the following
170,000-element vector:



<img
src="images/One-HotRepresentationOfWordsInASentence.png"
     loading="lazy"
     alt="A vector of 170,000 integers. The number 1 is at vector position 0,
          45770, 58906, and 91520. The number 2 is at position 26,100.
          Zeroes are at the remaining 169,996 positions.">


A sparse representation of the same sentence would simply be:

<pre class="prettyprint" translate="no" dir="ltr">
0: 1
26100: 2
45770: 1
58906: 1
91520: 1
</pre>

</div>

<hr />
</section>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-if-you-are-confused." data-text=" Click the icon if you are confused. " tabindex="-1">
Click the icon if you are confused.
</h4>

<div class="expand-background">
The term "sparse representation" confuses a lot of people because sparse
representation is itself <i>not a sparse vector</i>. Rather, sparse
representation is actually a <i>dense representation of a sparse vector</i>.
The synonym <b>index representation</b> is a little clearer than
"sparse representation."


</div>

<hr />
</section>

