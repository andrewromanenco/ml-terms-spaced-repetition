
One measure of how well a [[model|model]] is accomplishing its task.
For example, suppose your task is to read the first few letters of a word
a user is typing on a phone keyboard, and to offer a list of possible
completion words. Perplexity, P, for this task is approximately the number
of guesses you need to offer in order for your list to contain the actual
word the user is trying to type.

Perplexity is related to [[cross-entropy|cross-entropy]] as follows:

<div>
$$P= 2^{-\text{cross entropy}}$$
</div>



