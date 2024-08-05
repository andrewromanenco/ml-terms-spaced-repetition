#fundamentals

A technique for handling [[outliers|outliers]] by doing
either or both of the following:

<ul>
<li>Reducing [[feature|feature]] values that are greater than a maximum
threshold down to that maximum threshold.</li>
<li>Increasing feature values that are less than a minimum threshold up to that
minimum threshold.</li>
</ul>

For example, suppose that &lt;0.5% of values for a particular feature fall
outside the range 40–60. In this case, you could do the following:

<ul>
<li>Clip all values over 60 (the maximum threshold) to be exactly 60.</li>
<li>Clip all values under 40 (the minimum threshold) to be exactly 40.</li>
</ul>

Outliers can damage models, sometimes causing [[weight|weights]]
to overflow during training. Some outliers can also dramatically spoil
metrics like [[accuracy|accuracy]]. Clipping is a common technique to limit
the damage.

[[gradient clipping|Gradient clipping]] forces
[[gradient|gradient]] values within a designated range during training.

