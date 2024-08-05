#fairness

Factoring subjects&#39; [[sensitive attribute|sensitive attributes]]
into an algorithmic decision-making process such that different subgroups
of people are treated differently.

For example, consider an algorithm that
determines Lilliputians&#39; eligibility for a miniature-home loan based on the
data they provide in their loan application. If the algorithm uses a
Lilliputian&#39;s affiliation as Big-Endian or Little-Endian as an input, it
is enacting disparate treatment along that dimension.

Contrast with [[disparate impact|disparate impact]], which focuses
on disparities in the societal impacts of algorithmic decisions on subgroups,
irrespective of whether those subgroups are inputs to the model.
<aside class="warning"><strong>Warning:</strong><span> Because sensitive attributes are almost always correlated with
other features the data may have, explicitly removing sensitive attribute
information doesn&#39;t guarantee that subgroups will be treated equally.
For example, removing sensitive demographic attributes from a training
dataset that still includes postal code as a feature may address disparate
treatment of subgroups, but there still might be
disparate impact upon these groups because
postal code might serve as a [[proxy (sensitive attributes)|proxy]] for other
demographic information.</span></aside>
