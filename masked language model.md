#language

A [[language model|language model]] that predicts the probability of
candidate tokens to fill in blanks in a sequence. For instance, a
masked language model can calculate probabilities for candidate word(s)
to replace the underline in the following sentence:

<blockquote>
The ____ in the hat came back.
</blockquote>

The literature typically uses the string &quot;MASK&quot; instead of an underline.
For example:

<blockquote>
The &quot;MASK&quot; in the hat came back.
</blockquote>

Most modern masked language models are [[bidirectional|bidirectional]].

