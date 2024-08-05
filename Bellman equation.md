#rl

In reinforcement learning, the following identity satisfied by the optimal
[[Q-function|Q-function]]:

\[Q(s, a) = r(s, a) + \gamma \mathbb{E}_{s&#39;|s,a} \max_{a&#39;} Q(s&#39;, a&#39;)\]

[[reinforcement learning (RL)|Reinforcement learning]] algorithms apply this
identity to create [[Q-learning|Q-learning]] via the following update rule:

\[Q(s,a) \gets Q(s,a) + \alpha
  \left[r(s,a)
      + \gamma \displaystyle\max_{\substack{a_1}} Q(s&#39;,a&#39;)
    - Q(s,a) \right]
\]

Beyond reinforcement learning, the Bellman equation has applications to
dynamic programming. See the
<a href="https://wikipedia.org/wiki/Bellman_equation" target="T">
Wikipedia entry for Bellman equation</a>.

