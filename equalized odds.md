#fairness

A fairness metric to assess whether a model is predicting outcomes equally
well for all values of a [[sensitive attribute|sensitive attribute]] with
respect to both the [[positive class|positive class]] and
[[negative class|negative class]]—not just one class or the other
exclusively. In other words, both the [[true positive rate (TPR)|true positive rate]]
and [[false negative rate|false negative rate]] should be the same for
all groups.

Equalized odds is related to
[[equality of opportunity|equality of opportunity]], which only focuses
on error rates for a single class (positive or negative).

For example, suppose Glubbdubdrib University admits both Lilliputians and
Brobdingnagians to a rigorous mathematics program. Lilliputians&#39; secondary
schools offer a robust curriculum of math classes, and the vast majority of
students are qualified for the university program. Brobdingnagians&#39; secondary
schools don&#39;t offer math classes at all, and as a result, far fewer of
their students are qualified. Equalized odds is satisfied provided that no
matter whether an applicant is a Lilliputian or a Brobdingnagian, if they
are qualified, they are equally as likely to get admitted to the program,
and if they are not qualified, they are equally as likely to get rejected.

Suppose 100 Lilliputians and 100 Brobdingnagians apply to Glubbdubdrib
University, and admissions decisions are made as follows:

<strong>Table 3.</strong> Lilliputian applicants (90% are qualified)

<table>
  <tr> <th>&nbsp;</th>   <th>Qualified</th> <th>Unqualified</th> </tr>
  <tr> <th>Admitted</th> <td>45</td>        <td>2</td>           </tr>
  <tr> <th>Rejected</th> <td>45</td>        <td>8</td>           </tr>
  <tr> <th>Total</th>    <td>90</td>        <td>10</td>          </tr>
  <tr>
     <td colspan="3">
        Percentage of qualified students admitted: 45/90 = 50%<br/>
        Percentage of unqualified students rejected: 8/10 = 80%<br/>
        Total percentage of Lilliputian students admitted: (45+2)/100 = 47%
     </td>
  </tr>
</table>

&nbsp;

<strong>Table 4.</strong> Brobdingnagian applicants (10% are qualified):

<table>
  <tr> <th>&nbsp;</th>   <th>Qualified</th> <th>Unqualified</th> </tr>
  <tr> <th>Admitted</th> <td>5</td>         <td>18</td>           </tr>
  <tr> <th>Rejected</th> <td>5</td>         <td>72</td>           </tr>
  <tr> <th>Total</th>    <td>10</td>        <td>90</td>          </tr>
  <tr>
     <td colspan="3">
        Percentage of qualified students admitted: 5/10 = 50%<br/>
        Percentage of unqualified students rejected: 72/90 = 80%<br/>
        Total percentage of Brobdingnagian students admitted: (5+18)/100 = 23%
     </td>
  </tr>
</table>

Equalized odds is satisfied because qualified Lilliputian and Brobdingnagian
students both have a 50% chance of being admitted, and unqualified Lilliputian
and Brobdingnagian have an 80% chance of being rejected.
<aside class="note"><strong>Note:</strong><span> While equalized odds is satisfied here,
[[demographic parity|demographic parity]] is <em>not satisfied</em>. Lilliputian
and Brobdingnagian students are admitted to Glubbdubdrib University at
different rates; 47% of Lilliputian students are admitted, and 23% of
Brobdingnagian students are admitted.</span></aside>
Equalized odds is formally defined in
<a href="https://arxiv.org/pdf/1610.02413.pdf" target="T">&quot;Equality of
Opportunity in Supervised Learning&quot;</a> as follows:
&quot;predictor Ŷ satisfies equalized odds with respect
to protected attribute A and outcome Y if Ŷ and A are independent,
conditional on Y.&quot;
<aside class="note"><strong>Note:</strong><span> Contrast equalized odds with the more relaxed
[[equality of opportunity|equality of opportunity]] metric.</span></aside>
