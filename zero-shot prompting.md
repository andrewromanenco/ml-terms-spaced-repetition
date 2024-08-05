#language, #generativeAI

A [[prompt|prompt]] that does <em>not</em> provide an example of how you want
the [[large language model|large language model]] to respond. For example:

<table>
  <tr> <th>Parts of one prompt</th> <th>Notes</th> </tr>
  <tr>
    <td><tt>What is the official currency of the specified country?</tt></td>
    <td>The question you want the LLM to answer.</td>
  </tr>
  <tr> <td><tt>India:</tt></td>              <td>The actual query.</td> </tr>
</table>

The large language model might respond with any of the following:

<ul>
<li>Rupee</li>
<li>INR</li>
<li>₹</li>
<li>Indian rupee</li>
<li>The rupee</li>
<li>The Indian rupee</li>
</ul>

All of the answers are correct, though you might prefer a particular format.

Compare and contrast <strong>zero-shot prompting</strong> with the following terms:

<ul>
<li>[[one-shot prompting|one-shot prompting]]</li>
<li>[[few-shot prompting|few-shot prompting]]</li>
</ul>

