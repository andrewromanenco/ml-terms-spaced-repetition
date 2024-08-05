
The process of replacing a missing value with an acceptable substitute.
When a value is missing, you can either discard the entire example or you
can use value imputation to salvage the example.

For example, consider a dataset containing a <code translate="no" dir="ltr">temperature</code> feature that is
supposed to be recorded every hour. However, the temperature reading was
unavailable for a particular hour. Here is a section of the dataset:

<table>
<tr><th>Timestamp</th> <th>Temperature</th></tr>
<tr><td>1680561000</td> <td>10</td></tr>
<tr><td>1680564600</td> <td>12</td></tr>
<tr><td>1680568200</td> <td>missing</td></tr>
<tr><td>1680571800</td> <td>20</td></tr>
<tr><td>1680575400</td> <td>21</td></tr>
<tr><td>1680579000</td> <td>21</td></tr>
</table>

A system could either delete the missing example or impute the missing
temperature as 12, 16, 18, or 20, depending on the imputation algorithm.



