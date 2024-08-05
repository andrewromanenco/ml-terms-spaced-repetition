#fundamentals

Representing categorical data as a vector in which:

<ul>
<li>One element is set to 1.</li>
<li>All other elements are set to 0.</li>
</ul>

One-hot encoding is commonly used to represent strings or identifiers that
have a finite set of possible values.
For example, suppose a certain categorical feature named
<code translate="no" dir="ltr">Scandinavia</code> has five possible values:

<ul>
<li>&quot;Denmark&quot;</li>
<li>&quot;Sweden&quot;</li>
<li>&quot;Norway&quot;</li>
<li>&quot;Finland&quot;</li>
<li>&quot;Iceland&quot;</li>
</ul>

One-hot encoding could represent each of the five values as follows:

<table>
  <tr><th>country</th> <th colspan=5">Vector</th></tr>
  <tr><td>"Denmark"</td> <td>1</td> <td>0</td> <td>0</td> <td>0</td>
      <td>0</td></tr>
  <tr><td>"Sweden"</td> <td>0</td> <td>1</td> <td>0</td> <td>0</td>
      <td>0</td></tr>
  <tr><td>"Norway"</td> <td>0</td> <td>0</td> <td>1</td> <td>0</td>
      <td>0</td></tr>
  <tr><td>"Finland"</td> <td>0</td> <td>0</td> <td>0</td> <td>1</td>
      <td>0</td></tr>
  <tr><td>"Iceland"</td> <td>0</td> <td>0</td> <td>0</td> <td>0</td>
      <td>1</td></tr>
</table>

Thanks to one-hot encoding, a model can learn different connections
based on each of the five countries.

Representing a feature as [[numerical data|numerical data]] is an
alternative to one-hot encoding. Unfortunately, representing the
Scandinavian countries numerically is not a good choice. For example,
consider the following numeric representation:

<ul>
<li>&quot;Denmark&quot; is 0</li>
<li>&quot;Sweden&quot; is 1</li>
<li>&quot;Norway&quot; is 2</li>
<li>&quot;Finland&quot; is 3</li>
<li>&quot;Iceland&quot; is 4</li>
</ul>

With numeric encoding, a model would interpret the raw numbers
mathematically and would try to train on those numbers.
However, Iceland isn&#39;t actually twice as much (or half as much) of
something as Norway, so the model would come to some strange conclusions.

