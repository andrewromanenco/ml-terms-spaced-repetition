#fundamentals

A technique for improving the quality of
[[large language model|large language model (LLM)]] output
by grounding it with sources of knowledge retrieved after the model was trained.
RAG improves the accuracy of LLM responses by providing the trained LLM with
access to information retrieved from trusted knowledge bases or documents.

Common motivations to use retrieval-augmented generation include:

<ul>
<li>Increasing the factual accuracy of a model&#39;s generated responses.</li>
<li>Giving the model access to knowledge it was not trained on.</li>
<li>Changing the knowledge that the model uses.</li>
<li>Enabling the model to cite sources.</li>
</ul>

For example, suppose that a chemistry app uses the <a href="https://developers.generativeai.google/products/palm">PaLM
API</a> to generate summaries
related to user queries. When the app&#39;s backend receives a query, the backend:

<ol>
<li>Searches for (&quot;retrieves&quot;) data that&#39;s relevant to the user&#39;s query.</li>
<li>Appends (&quot;augments&quot;) the relevant chemistry data to the user&#39;s query.</li>
<li>Instructs the LLM to create a summary based on the appended data.</li>
</ol>

