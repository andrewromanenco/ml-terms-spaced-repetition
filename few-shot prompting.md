#language, #generativeAI

A [[prompt|prompt]] that contains more than one (a &quot;few&quot;) example
demonstrating how the [[large language model|large language model]]
should respond. For example, the following lengthy prompt contains two
examples showing a large language model how to answer a query.

<table>
  <tr> <th>Parts of one prompt</th> <th>Notes</th> </tr>
  <tr>
    <td><tt>What is the official currency of the specified country?</tt></td>
    <td>The question you want the LLM to answer.</td>
  </tr>
  <tr> <td><tt>France: EUR</tt></td>         <td>One example.</td> </tr>
  <tr> <td><tt>United Kingdom: GBP</tt></td> <td>Another example.</td> </tr>
  <tr> <td><tt>India:</tt></td>              <td>The actual query.</td> </tr>
</table>

Few-shot prompting generally produces more desirable results than
[[zero-shot prompting|zero-shot prompting]] and
[[one-shot prompting|one-shot prompting]]. However, few-shot prompting
requires a lengthier prompt.

Few-shot prompting is a form of [[few-shot learning|few-shot learning]]
applied to [[prompt-based learning|prompt-based learning]].

