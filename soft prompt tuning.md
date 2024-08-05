#language, #generativeAI

A technique for tuning a [[large language model|large language model]]
for a particular task, without resource intensive
[[fine tuning|fine-tuning]]. Instead of retraining all the
[[weight|weights]] in the model, soft prompt tuning
automatically adjusts a [[prompt|prompt]] to achieve the same goal.

Given a textual prompt, soft prompt tuning
typically appends additional token embeddings to the prompt and uses
backpropagation to optimize the input.

A &quot;hard&quot; prompt contains actual tokens instead of token embeddings.

