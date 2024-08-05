#language

A tactic of training a model in a sequence of discrete stages. The goal can be
either to speed up the training process, or to achieve better model quality.

An illustration of the progressive stacking approach is shown below:

<ul>
<li>Stage 1 contains 3 hidden layers, stage 2 contains 6 hidden layers, and
stage 3 contains 12 hidden layers.</li>
<li>Stage 2 begins training with the weights learned in the 3 hidden layers
of Stage 1. Stage 3 begins training with the weights learned in the 6
hidden layers of Stage 2.</li>
</ul>


![[ images/staged-training.png ]]


See also [[pipelining|pipelining]].

