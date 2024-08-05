#language, #generativeAI

A [[prompt|prompt]] that contains <em>one</em> example demonstrating how the
[[large language model|large language model]] should respond. For example,
the following prompt contains one example showing a large language model how
it should answer a query.

<table>
  <tr> <th>Parts of one prompt</th> <th>Notes</th> </tr>
  <tr>
    <td><tt>What is the official currency of the specified country?</tt></td>
    <td>The question you want the LLM to answer.</td>
  </tr>
  <tr> <td><tt>France: EUR</tt></td>         <td>One example.</td> </tr>
  <tr> <td><tt>India:</tt></td>              <td>The actual query.</td> </tr>
</table>

Compare and contrast <strong>one-shot prompting</strong> with the following terms:

<ul>
<li>[[zero-shot prompting|zero-shot prompting]]</li>
<li>[[few-shot prompting|few-shot prompting]]</li>
</ul>

