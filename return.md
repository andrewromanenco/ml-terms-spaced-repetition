#rl

In reinforcement learning, given a certain policy and a certain state, the
return is the sum of all [[reward|rewards]] that the [[agent|agent]]
expects to receive when following the [[policy|policy]] from the
[[state|state]] to the end of the [[episode|episode]]. The agent
accounts for the delayed nature of expected rewards by discounting rewards
according to the state transitions required to obtain the reward.

Therefore, if the discount factor is \(\gamma\), and \(r_0, \ldots, r_{N}\)
denote the rewards until the end of the episode, then the return calculation
is as follows:

<div>
$$\text{Return} = r_0 + \gamma r_1 + \gamma^2 r_2 + \ldots + \gamma^{N-1} r_{N-1}$$
</div>

