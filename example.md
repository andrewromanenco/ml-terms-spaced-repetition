#fundamentals

The values of one row of [[feature|features]] and possibly
a [[label|label]]. Examples in
[[supervised machine learning|supervised learning]] fall into two
general categories:

<ul>
<li>A [[labeled example|labeled example]] consists of one or more features
and a label. Labeled examples are used during training.</li>
<li>An [[unlabeled example|unlabeled example]] consists of one or
more features but no label. Unlabeled examples are used during inference.</li>
</ul>

For instance, suppose you are training a model to determine the influence
of weather conditions on student test scores. Here are three labeled examples:

<table>
  <tr><th colspan="3">Features</th> <th>Label</th></tr>
  <tr><th width="25%">Temperature</th> <th width="25%">Humidity</th>
      <th width="25%">Pressure</th> <th width="25%">Test score</th></tr>
  <tr><td>15</td> <td>47</td> <td>998</td> <td>Good</td></tr>
  <tr><td>19</td> <td>34</td> <td>1020</td> <td>Excellent</td></tr>
  <tr><td>18</td> <td>92</td> <td>1012</td> <td>Poor</td></tr>
</table>

Here are three unlabeled examples:

<table>
  <tr><th width="25%">Temperature</th> <th width="25%">Humidity</th>
      <th width="25%">Pressure</th> <th width="25%">&nbsp;</th></tr>
  <tr><td>12</td> <td>62</td> <td>1014</td>  <td>&nbsp;</td></tr>
  <tr><td>21</td> <td>47</td> <td>1017</td>  <td>&nbsp;</td></tr>
  <tr><td>19</td> <td>41</td> <td>1021</td>  <td>&nbsp;</td></tr>
</table>

The row of a [[data set or dataset|dataset]] is typically the raw source for an example.
That is, an example typically consists of a subset of the columns in
the dataset. Furthermore, the features in an example can also include
[[synthetic feature|synthetic features]], such as
[[feature cross|feature crosses]].

