#df

In a [[decision tree|decision tree]], a [[condition|condition]]
that tests for the presence of one item in a set of items.
For example, the following is an in-set condition:
<pre class="prettyprint" translate="no" dir="ltr"><code translate="no" dir="ltr">  house-style in [tudor, colonial, cape]
</code></pre>
During inference, if the value of the house-style [[feature|feature]]
is <code translate="no" dir="ltr">tudor</code> or <code translate="no" dir="ltr">colonial</code> or <code translate="no" dir="ltr">cape</code>, then this condition evaluates to Yes. If
the value of the house-style feature is something else (for example, <code translate="no" dir="ltr">ranch</code>),
then this condition evaluates to No.

In-set conditions usually lead to more efficient decision trees than
conditions that test [[one-hot encoding|one-hot encoded]] features.

