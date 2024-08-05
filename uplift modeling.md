
A modeling technique, commonly used in marketing, that models the
&quot;causal effect&quot; (also known as the &quot;incremental impact&quot;) of a
&quot;treatment&quot; on an &quot;individual.&quot; Here are two examples:

<ul>
<li>Doctors might use uplift modeling to predict the mortality decrease
(causal effect) of a medical procedure (treatment) depending on the
age and medical history of a patient (individual).</li>
<li>Marketers might use uplift modeling to predict the increase in
probability of a purchase (causal effect) due to an advertisement
(treatment) on a person (individual).</li>
</ul>

Uplift modeling differs from [[classification model|classification]] or
[[regression model|regression]] in that some labels (for example, half
of the labels in binary treatments) are always missing in uplift modeling.
For example, a patient can either receive or not receive a treatment;
therefore, we can only observe whether the patient is going to heal or
not heal in only one of these two situations (but never both).
The main advantage of an uplift model is that it can generate predictions
for the unobserved situation (the counterfactual) and use it to compute
the causal effect.

