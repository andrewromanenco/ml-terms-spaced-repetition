#language, #generativeAI

Any text entered as input to a [[large language model|large language model]]
to condition the model to behave in a certain way. Prompts can be as short as a
phrase or arbitrarily long (for example, the entire text of a novel). Prompts
fall into multiple categories, including those shown in the following table:

<table>
  <tr><th>Prompt category</th> <th>Example</th> <th>Notes</th></tr>
  <tr>
    <td>Question</td>
    <td><tt>How fast can a pigeon fly?</tt></td>
  </tr>
  <tr>
    <td>Instruction</td>
    <td><tt>Write a funny poem about arbitrage.</tt></td>
    <td>A prompt that asks the large language model to <i>do</i> something.</td>
  </tr>
  <tr>
    <td>Example</td>
    <td><tt>Translate Markdown code to HTML. For example:
        <br/>
        Markdown: * list item
        <br/>
        HTML: &lt;ul&gt; &lt;li&gt;list item&lt;/li&gt; &lt;/ul&gt;</tt></td>
    <td>The first sentence in this example prompt is an instruction.
        The remainder of the prompt is the example. </td>
  </tr>
  <tr>
    <td><a href="#role-prompting"><b>Role</b></a></td>
    <td><tt>Explain why gradient descent is used in machine learning training to
        a PhD in Physics.</tt></td>
    <td>The first part of the sentence is an instruction; the phrase
        "to a PhD in Physics" is the role portion.</td>
  </tr>
  <tr>
    <td>Partial input for the model to complete</td>
    <td><tt>The Prime Minister of the United Kingdom lives at</tt></td>
    <td>A partial input prompt can either end abruptly (as this example does)
        or end with an underscore.</td>
  </tr>
</table>

A [[generative AI|generative AI]] model can respond to a prompt with text,
code, images, [[embedding vector|embeddings]], videos…almost anything.

