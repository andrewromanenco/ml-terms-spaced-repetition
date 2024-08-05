#seq, #language

An ordered sequence of N words. For example, <em>truly madly</em> is a 2-gram. Because
order is relevant, <em>madly truly</em> is a different 2-gram than <em>truly madly</em>.

<table>
  <tr>
    <th>N</th>
    <th>Name(s) for this kind of N-gram</th>
    <th>Examples</th>
  </tr>
  <tr>
    <td>2 </td>
    <td>bigram or 2-gram </td>
    <td><em>to go, go to, eat lunch, eat dinner</em> </td>
  </tr>
  <tr>
    <td>3 </td>
    <td>trigram or 3-gram </td>
    <td><em>ate too much, three blind mice, the bell tolls</em> </td>
  </tr>
  <tr>
    <td>4 </td>
    <td>4-gram </td>
    <td><em>walk in the park, dust in the wind, the boy ate lentils</em> </td>
  </tr>
</table>

Many [[natural language understanding|natural language understanding]]
models rely on N-grams to predict the next word that the user will type
or say. For example, suppose a user typed <em>three blind</em>.
An NLU model based on trigrams would likely predict that the
user will next type <em>mice</em>.

Contrast N-grams with [[bag of words|bag of words]], which are
unordered sets of words.

