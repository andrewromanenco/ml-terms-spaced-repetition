#fundamentals

Data used to approximate labels not directly available in a dataset.

For example, suppose you must train a model to predict employee
stress level. Your dataset contains a lot of predictive features but
doesn&#39;t contain a label named <em>stress level.</em>
Undaunted, you pick &quot;workplace accidents&quot; as a proxy label for
stress level. After all, employees under high stress get into more
accidents than calm employees. Or do they? Maybe workplace accidents
actually rise and fall for multiple reasons.

As a second example, suppose you want <em>is it raining?</em> to be a Boolean label
for your dataset, but your dataset doesn&#39;t contain rain data. If
photographs are available, you might establish pictures of people
carrying umbrellas as a proxy label for <em>is it raining?</em> Is that
a good proxy label? Possibly, but people in some cultures may be
more likely to carry umbrellas to protect against sun than the rain.

Proxy labels are often imperfect. When possible, choose actual labels over
proxy labels. That said, when an actual label is absent, pick the proxy
label very carefully, choosing the least horrible proxy label candidate.

