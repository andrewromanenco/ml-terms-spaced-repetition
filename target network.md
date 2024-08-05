#rl

In [[Q-learning|Deep Q-learning]], a neural network that is a stable
approximation of the main neural network, where the main neural network
implements either a [[Q-function|Q-function]] or a [[policy|policy]].
Then, you can train the main network on the Q-values predicted by the target
network. Therefore, you prevent the feedback loop that occurs when the main
network trains on Q-values predicted by itself. By avoiding this feedback,
training stability increases.

