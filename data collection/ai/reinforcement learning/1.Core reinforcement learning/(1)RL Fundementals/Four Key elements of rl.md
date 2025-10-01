Once you've grasped the 5 basic concepts of reinforcement learning, there are also four policies that we have to understand.

One of them being policy (π); it's basically the agent's strategy book. It maps observed states (s) of the environment to the action (a) it takes when in those states. In simple terms, it is the "brain" that is used to fin the optimal policy (π∗) or maximizes the agent's expected cumulative reward over the long term.

After that is the reward signal (R[t]); it is the immediate, scalar feedback that the agent receives from the environment after taking an action. It is the sole indicator of the immediate desirability of the agent's action.

Next up on the list is called the value function; it is a mathematical tool that estimates the expected cumulative reward an agent can recieve from a given state or state-action pair while following a particular policy (strategy). It serves as a guide for the agent to evaluate the long term desirability of different states or actions, helping it make decisions that maximize total future rewards.

Lastly is model; it is a representation that allows the agent to predict the next state and the reward it will receive if it takes a particular action from a given state. Simply put, the model answers the question: "What will happen if I take action "a" in state "s"?"