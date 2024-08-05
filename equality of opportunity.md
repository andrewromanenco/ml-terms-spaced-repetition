#fairness

A [[fairness metric|fairness metric]] to assess whether a model is
predicting the desirable outcome equally well for all values of a
[[sensitive attribute|sensitive attribute]]. In other words, if the
desirable outcome for a model is the [[positive class|positive class]],
the goal would be to have the [[true positive rate (TPR)|true positive rate]] be the
same for all groups.

Equality of opportunity is related to [[equalized odds|equalized odds]],
which requires that <em>both</em> the true positive rates and
[[false positive (FP)|false positive rates]] are the same for all groups.

Suppose Glubbdubdrib University admits both Lilliputians and Brobdingnagians
to a rigorous mathematics program. Lilliputians&#39; secondary schools offer a
robust curriculum of math classes, and the vast majority of students are
qualified for the university program. Brobdingnagians&#39; secondary schools don&#39;t
offer math classes at all, and as a result, far fewer of their students are
qualified. Equality of opportunity is satisfied for the preferred label of
&quot;admitted&quot; with respect to nationality (Lilliputian or Brobdingnagian) if
qualified students are equally likely to be admitted irrespective of whether
they&#39;re a Lilliputian or a Brobdingnagian.

For example, suppose 100 Lilliputians and 100 Brobdingnagians apply to
Glubbdubdrib University, and admissions decisions are made as follows:

<strong>Table 1.</strong> Lilliputian applicants (90% are qualified)

<table>
  <tr> <th>&nbsp;</th>   <th>Qualified</th> <th>Unqualified</th> </tr>
  <tr> <th>Admitted</th> <td>45</td>        <td>3</td>           </tr>
  <tr> <th>Rejected</th> <td>45</td>        <td>7</td>           </tr>
  <tr> <th>Total</th>    <td>90</td>        <td>10</td>          </tr>
  <tr>
     <td colspan="3">
        Percentage of qualified students admitted: 45/90 = 50%<br/>
        Percentage of unqualified students rejected: 7/10 = 70%<br/>
        Total percentage of Lilliputian students admitted: (45+3)/100 = 48%
     </td>
  </tr>
</table>

&nbsp;

<strong>Table 2.</strong> Brobdingnagian applicants (10% are qualified):

<table>
  <tr> <th>&nbsp;</th>   <th>Qualified</th> <th>Unqualified</th> </tr>
  <tr> <th>Admitted</th> <td>5</td>         <td>9</td>           </tr>
  <tr> <th>Rejected</th> <td>5</td>         <td>81</td>          </tr>
  <tr> <th>Total</th>    <td>10</td>        <td>90</td>          </tr>
  <tr>
     <td colspan="3">
        Percentage of qualified students admitted: 5/10 = 50%<br/>
        Percentage of unqualified students rejected: 81/90 = 90%<br/>
        Total percentage of Brobdingnagian students admitted: (5+9)/100 = 14%
     </td>
  </tr>
</table>

The preceding examples satisfy equality of opportunity for acceptance of
qualified students because qualified Lilliputians and Brobdingnagians both
have a 50% chance of being admitted.

While equality of opportunity is satisfied, the following two fairness metrics
are not satisfied:

<ul>
<li>[[demographic parity|demographic parity]]: Lilliputians and
 Brobdingnagians are admitted to the university at different rates;
 48% of Lilliputians students are admitted, but only 14% of
 Brobdingnagian students are admitted.</li>
<li>[[equalized odds|equalized odds]]: While qualified Lilliputian
 and Brobdingnagian students both have the same chance of being admitted,
 the additional constraint that unqualified Lilliputians and
 Brobdingnagians both have the same chance of being rejected is not
 satisfied. Unqualified Lilliputians have a 70% rejection rate, whereas
 unqualified Brobdingnagians have a 90% rejection rate.</li>
</ul>

See <a href="https://arxiv.org/pdf/1610.02413.pdf" target="T">&quot;Equality of
Opportunity in Supervised Learning&quot;</a> for a more detailed discussion
of equality of opportunity. Also see
<a href="http://research.google.com/bigpicture/attacking-discrimination-in-ml/" target="T">&quot;Attacking
discrimination with smarter machine learning&quot;</a> for a visualization
exploring the tradeoffs when optimizing for equality of opportunity.

