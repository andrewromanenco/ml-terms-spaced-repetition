#fairness

A fairness metric that checks whether similar individuals are classified
similarly. For example, Brobdingnagian Academy might want to satisfy
individual fairness by ensuring that two students with identical grades
and standardized test scores are equally likely to gain admission.

Note that individual fairness relies entirely on how you define &quot;similarity&quot;
(in this case, grades and test scores), and you can run the risk of
introducing new fairness problems if your similarity metric misses important
information (such as the rigor of a student&#39;s curriculum).

See <a href="https://arxiv.org/pdf/1104.3913.pdf" target="T">&quot;Fairness Through
Awareness&quot;</a> for a more detailed discussion of individual fairness.

