Once you've grasped the 5 basic concepts of reinforcement learning, there are also four policies that we have to understand.

One of them being policy (π); it defines the learning agent’s way of behaving at a given time. Roughly speaking, a policy is a mapping from perceived states of the environment to actions to be taken when in those states.

After that is the reward signal (R[t]); it defines the goal in a reinforcement learning problem. On each time step, the environment sends to the reinforcement learning agent a single number, a reward. The agent’s sole objective is to maximize the total reward it receives over the long run.

Next up on the list is called the value function; it specifies what is good in the long run. Roughly speaking, the value of a state is the total amount of reward an agent can expect to accumulate over the future, starting from that state.

Lastly is model; it is something that mimics the behavior of the environment, or more generally, that allows inferences to be made about how the environment will behave.