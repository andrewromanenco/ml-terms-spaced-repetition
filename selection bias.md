#fairness

Errors in conclusions drawn from sampled data due to a selection process
that generates systematic differences between samples observed in the data
and those not observed. The following forms of selection bias exist:

<ul>
<li><strong>coverage bias</strong>: The population represented in the dataset doesn&#39;t
match the population that the machine learning model is making
predictions about.</li>
<li><strong>sampling bias</strong>: Data is not collected randomly from the target group.</li>
<li><strong>non-response bias</strong> (also called <strong>participation bias</strong>): Users from
certain groups opt-out of surveys at different rates than users from
other groups.</li>
</ul>

For example, suppose you are creating a machine learning model that predicts
people&#39;s enjoyment of a movie. To collect training data,
you hand out a survey to everyone in the front row of a theater
showing the movie. Offhand, this may sound like a reasonable way
to gather a dataset; however, this form of data collection may
introduce the following forms of selection bias:

<ul>
<li>coverage bias: By sampling from a population who chose to see
the movie, your model&#39;s predictions may not generalize to people
who did not already express that level of interest in the movie.</li>
<li>sampling bias: Rather than randomly sampling from the
intended population (all the people at the movie), you sampled only
the people in the front row. It is possible that the people sitting
in the front row were more interested in the movie than those in
other rows.</li>
<li>non-response bias: In general, people with strong opinions tend
to respond to optional surveys more frequently than people with mild
opinions. Since the movie survey is optional, the responses
are more likely to form a
<a href="https://wikipedia.org/wiki/Multimodal_distribution"
target="T">bimodal distribution</a>
than a normal (bell-shaped) distribution.</li>
</ul>

