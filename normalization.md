#fundamentals

Broadly speaking, the process of converting a variable&#39;s actual range
of values into a standard range of values, such as:

<ul>
<li>-1 to +1</li>
<li>0 to 1</li>
<li>the normal distribution</li>
</ul>

For example, suppose the actual range of values of a certain feature is
800 to 2,400. As part of [[feature engineering|feature engineering]],
you could normalize the actual values down to a standard range, such
as -1 to +1.

Normalization is a common task in
[[feature engineering|feature engineering]]. Models usually train faster
(and produce better predictions) when every numerical feature in the
[[feature vector|feature vector]] has roughly the same range.

