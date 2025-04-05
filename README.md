# Reinforcement Learning Tasks

This repository contains a collection of reinforcement learning tasks designed to facilitate learning and experimentation with the [Gymnasium](https://gymnasium.farama.org/) framework.

We'll consider the following equations when solving these exercises:

### The Agent–Environment Interface

In a finite MDP, the sets of states, actions, and rewards ($S$, $A$, and $R$) all have a finite
number of elements. In this case, the random variables $R_t$ and $S_t$ have well defined
discrete probability distributions dependent only on the preceding state and action. That
is, for particular values of these random variables, $s' \in S$ and $r \in R$, there is a probability
of those values occurring at time t, given particular values of the preceding state and
action:

$$
p(s',r|s,a) = Pr\{S_t=s', R_t=r | S_{t-1} = s, A_{t-1} = a\}
$$

for all $s',s \in S, r \in R$, and $a \in A(s)$. The function $p$ defines the dynamics of the MDP.
The dot over the equals sign in the equation reminds us that it is a definition (in this
case of the function $p$) rather than a fact that follows from previous definitions. The
dynamics function $p : S \times R \times S \times A \to [0, 1]$ is an ordinary deterministic function of four
arguments.
