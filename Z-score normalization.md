#fundamentals

A [[scaling|scaling]] technique that replaces a raw
[[feature|feature]] value with a floating-point value representing
the number of standard deviations from that feature&#39;s mean.
For example, consider a feature whose mean is 800 and whose standard
deviation is 100. The following table shows how Z-score normalization
would map the raw value to its Z-score:

<table>
  <tr> <th>Raw value</th> <th>Z-score</th> </tr>
  <tr> <td>800</td>       <td>0</td>       </tr>
  <tr> <td>950</td>       <td>+1.5</td>    </tr>
  <tr> <td>575</td>       <td>-2.25</td>   </tr>
</table>

The machine learning model then trains on the Z-scores
for that feature instead of on the raw values.
  
