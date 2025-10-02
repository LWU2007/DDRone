Once you've grasped how the Markov Decision Process fundementally works, we'll finally be able to jump into the algorithms built upon the Markov Decision Process framework.


Value-Based Methods:
First up is the value based method, it focuses on learning the optimal value function which estimates the expected return (cumulative reward) for being in a particular state or taking a particular action. They ultimately work by:
1. Goal: they learn the the optimal action-value function "Q*(s,a)", which is the expected return for taking action "a" in state "s" and following the optimal policy thereafter.
2. Policy: The policy "π" is implicit and is often ϵ-greedy, meaning that it selects the action with the highest Q-value (exploitation) most of the time, but occasionally selects a random action (exploration) to find potentially better actions.
3. Advantage: Effective for problems with discrete action spaces.
4. Limitation: Struggles with continuous action spaces because it's impossible to maximize over an infinite number of actions.

Some algorithms from value-based methods are: Q-Learning, SARSA, and Deep Q-Networks (DQN).


Policy-Based Methods:
Also known as Policy Gradient methods, directly learns a parameterized policy that maps states to actions without explicitly learning a value function. They work by:
1. Goal: Directly learning the optimal policy "πθ(a∣s)", which is a set of parameters "θ" (e.g weights of a neural network) that determines the probability of taking action "a" in state "s".
2. Optimization: The parameters "θ" are adjusted using gradient ascent to maximize an objective function that represents the expected cumulative reward (the performance of the policy).
3. Policy Gradiet Theorem: Provides the mathematical foundation for calculating the gradient of the performance objective with respect to the policy parameters.
4. Advantage: Excellent for problems with continuous action spaces and can learn stochastic policies (probabilistic actions).
5. Limitation: Updates can have high variance, leading to unstable or slow training.

Some algorithms from policy-based methods are: REINFORCE (Monte Carlo Policy Gradient) and Vanilla Policy Gradient.


Actor-Critic Methods:
It combines both the strengths of both value-based and policy-based approaches by using two seperate components that learn concurrently. They work by:
1. Actor: The policy function (the "actor") decides which action to take. This is updated using a policy gradient, simillar to policy-based methods.
2. Critic: The value function (the "critic") evaluates the action taken by the actor by estimating the expected value of the current state "V(s)" or state-action pair "Q(s,a)".
3. Advantage: The critic's value estimate is used to calculate the advantage, which acts as a more stable and low-variance (baseline) to guide the actor's policy update. This often leads to faster and more stable learning than pure policy-based methods.
4. Balance: They balance the explicit policy learning of policy-based methods with the stability of value-based estimation.

Some algorithms that uses this actor-critic methods are: A2C/A3C, DDPG, and TD3.