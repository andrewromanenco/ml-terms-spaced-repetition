#language, #generativeAI

A [[prompt engineering|prompt engineering]] technique that encourages
a [[large language model|large language model]] (LLM) to explain its
reasoning, step by step. For example, consider the following prompt, paying
particular attention to the second sentence:

<blockquote>
How many g forces would a driver experience in a car that goes from 0 to 60
miles per hour in 7 seconds? In the answer, show all relevant calculations.
</blockquote>

The LLM&#39;s response would likely:

<ul>
<li>Show a sequence of physics formulas, plugging in the values 0, 60, and 7
in appropriate places.</li>
<li>Explain why it chose those formulas and what the various variables mean.</li>
</ul>

Chain-of-thought prompting forces the LLM to perform all the calculations,
which might lead to a more correct answer. In addition, chain-of-thought
prompting enables the user to examine the LLM&#39;s steps to determine whether
or not the answer makes sense.

