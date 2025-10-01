We're finished with the fundementals of reinforcement learning. Now it's time to move on to some algorithms and theory. But first, we have to understand the back bones of all these algorithms, the Markov Decision Process.

The Markov Decision Process or MDP for short is a framework built upon the Markov Chain which is a stochastic process that satisfies the Markov property, meaning the probability of transitioning to the next state depends only on the current state, and not on the sequence of events that preceded it (it's "memoryless").
The Markov chain is defined by only its states and transition probability, while the Markov Decision Process also takes into account the action taken by the agent, the transition probability which is now influenced by the action taken, and also reward. Therse are all here to help introduce the element of decision making and control for the agent.

So the Markov Decision Process at its core is defined by a tuple ⟨S,A,P,R,γ⟩
S = state (The set of all possible situations or configurations the agent can be in. The state must satisfy the Markov property)
A = actions (The set of all possible decisions or moves the agent can make. The available actions may vary depending on the current state)
P = transition probability (A function P(s′∣s,a) that defines the probability of transitioning to the next state "s′" given the current state "s" and the action "a" taken. This is the random element of the environment)
R = reward function (A function R(s,a,s′) that specifies the immediate reward (a numerical value, positive or negative) the agent receives after transitioning from state s to state s′
 by taking action a)
γ = discount factor (A value between 0 and 1 that represents the importance of future rewards compared to immediate rewards. A value near 0 makes the agent "myopic" (focusing only on immediate rewards), while a value near 1 makes it "far-sighted" (considering long-term consequences))


Once you've grasped the core of the Markov Decision Process, let us continue and see how the decision process for the Markov Decision Process is handled.
1. Observation: The agent observes the current state "s[t]".
2. Action Selection: Based on a defined policy "π", the agent selects an action "a[t]".
- Policy is a rule that maps each state to the action (or a probability distribution over actions) the agent will choose in that state (π(s)=a).
3. Transition: When the action "a[t]" is executed in the environment, it causes the system to transition into a new state "s[t+1]" according to the probability P(s[t+1]|s[t],a[t]).
4. Reward: The agent receives an immediate reward "r[t+1]" based on the transition.
5. Repeat: The cycle repeats again starting from "s[t+1]".



Now you might be wondering, "Why do all this the first place? If you've found the end, why not just end it there?" Oh my silly reader, it's so funny for you to be saying that. We are not here to be satisfied with the status quo, we are here to maximize our time or in other words "OPTIMIZATION". 

The ultimate goal in a Markov Decision Process is to reach the optimal policy (π∗) - the policy that maximizes the return over the long run.
In order to do that, algorithms use value functions to estimate how "good" a state or a state-pair is:
1. State-Value Function V(s): The expected return (total discounted reward) starting from state "s" and then following a specific policy π.
2. Action-Value Function Q(s,a): The expected return starting state "s", taking action "a", and thereafter following policy "π". This function is often more useful because it directly tells the agent the expected value of taking a particular action in a particular state.

Besides value functions, there is also an equation called the Bellman Optimality Equation.
This equation periodically breaks down the optimal value function V*(s) into the immediate rewards plus the discounted optimal value of the next state.
*insert equation*
It essentially states that the optimal value of a state "s" is the reward for the best possible action "a", plus the discounted optimal value of the states "s′" that results from taking that action.


In order to solve a Markov Decision Process, you first solve the optimal value function (V* or Q*) and then deriving the optimal policy (π*) from it. It's usually done by using these methods:
1. Dynamic Programming (Value Iteration and Policy Iteration): Used when the full Markov Decision Process model (P and R) is known. These iterative algorithms solve the Bellman equation.
2. Reinforcement Learning (RL): Used when the full Markov Decision Process model is unknown. A Reinforcement Learning agent interacts with the environment (the Markov Decision Process), learns by trial and error, and updates its value function or policy based on the experienced rewards. Examples include Q-Learning and SARSA.