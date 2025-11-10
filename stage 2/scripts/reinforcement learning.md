*Page 1*
Now we've finally reached the part in which we learn about reinforcement learning. So what is reinforcement learning? Reinforcement Learning is an interdisciplinary area of machine learning and optimal control concerned with how an intelligent agent should take actions in a dynamic environment in order to maximize a reward signal. Reinforcement learning is one of the three basic machine learning paradigms, alongside supervised learning and unsupervised learning.
 
 Before digging any further, we first have to understand the 5 concepts withing reinforcement learning. The first one is the agent; it is basically the one who is in control. Next is the environment, more or less what the agent is able to interact with.

 *Page 2*
 Third is the state, it can be described as a picture in time so that the agent is able to process it more easily. Fourth is the action, in summary, the thing that the agent acts upon. And lastly is the reward, which is given after the agent does an action.

 Next up is the 4 policies.
 First up on the list is policy with the symbol PI, you can think of it as how the agent will react or behave. Next up is the reward signal or R(t) which tells the agent what is "should" do. 
 
 *Page 3*
 After that is the value function which estimates the expected total reward it can recieve from a specific state or state-action pair from a particular policy. Lastly is the model, it helps predict the consequences the agent will recieve if it had chosen that option or state/

*Page 4*
Fundamental done, now we'll see how the machine is trained. There are two ways, one is online and the other is offline.

In online, the machine or ai is able to see the surroundings and act accordingly live. This is very useful in examples such as trying to teach a robot how to work.

This has an advantage of:
- continuously adapting to a changing environment.
- maximizes performance by achieving the optimal policy by exploring and collecting new, highly relevant data.
- the data collected always matches the agent's current policy (on-policy), avoiding data mismatch issues.

But this also has a disadvantage of:
- the agent performing unsafe or highly suboptimal actions during the learning phase (i.e robots crashing).
- requiring continuous, real-time compute resources attached to the environment making it highly expensive and slow to operate.

*Page 5*
In offline, the robot is basically has no sensory organs and is asked to learn from other's past experiences. This is very much helpful in training ai for autonomous vehicles in order to reduce fatalities done by autonomous vehicles.

This has an advantage of:
- removing the risk of dangerous exploration and making it ideal for safety-critical domains (healthcare and autonomous driving).
- being able to be trained flexibly and on pre-allocated compute resources without needing real-time environment access.
- leveraging historical data collected over years, which is often infeasable for a single training run.

But it also has the disadvantage of:
- the agent's learnt policy that may choose actions not seen in the dataset(out-of-distribution), leading to an uncertain and highly-unreliable performance.
- the policy's performance that is fundementally limited by the quality and coverage of the static dataset.
- requiring complex and specialized algorithms yo correct for the distributional shift problem.

*Page 6*
Now, we're moving on to the algorithm and theory.
All reinforcement learning models are built from the markov decision process which is built upon the markov chain. This is due to the markov chain having a memoryless trait that no other probability models have.


*Page 7*
Markov Decision Process is defined by action, state, transition probability, reward function and discount factor.
Transition probability being the chance it moves to the other state from the current state. And discount factor being the one that decides if it's important or not.

*Page 8*
Next up is how MDP works.
It first sees the current state then chooses what it's going to do next. It then executes the action and gets the reward. Rinse and repeat.

*Page 9*
This is all done for optimization. Why? They want to make their jobs even harder.
In order to do that, they use value functions to see how good a state-pair is.

- State-Value Function V(s): The expected return (total discounted reward) starting from state "s" and then following a specific policy π.

- Action-Value Function Q(s,a): The expected return starting state "s", taking action "a", and thereafter following policy "π". This function is often more useful because it directly tells the agent the expected value of taking a particular action in a particular state.

*Page 10*
Besides value functions, there is also an equation called the Bellman Optimality. This breaks down the optimal value function into the immediate rewards plus the discounted optimal value of the next state.

*Page 11*
In order to solve a Markov Decision Process, you first solve the optimal value function (V* or Q*) and then deriving the optimal policy (π*) from it. It's usually done by using these methods:

First is dynamic programming which is used when the full MDP model is known. Second is reinforcement learning, it's used when the the full MDP model is unknown.

*Page 12*
Now let's jump to the algorithms built upon MDP.
First is value-based methods: it focuses on learning the optimal value function which estimates the expected return (cumulative reward) for being in a particular state or taking a particular action.

*Page 13*
Second policy based methods: it is directly learns a parameterized policy that maps states to actions without explicitly learning a value function.

*Page 14*
Last is the Actor-Critic Methods: It combines both the strengths of both value-based and policy-based approaches by using two seperate components that learn concurrently.

*Page 15*
Use cases of reinforcement learning is in simulated starship training, openai five, tesla full self-driving, and stockfish (although not fully reinforcement learning since it also use alpha-beta search and neural networks evaluation)

*Page 16*
Up next is about advanced and new research topics.
First up is ethical research alignment which focuses on transparency and accountability.

1. Reinforcement Learning from Human Feedback (RLHF) and Alignment:
- Focus: Using human preferences to train a reward model that aligns the AI's behavior with human values, this is key for social media algorithms and LLMs.

2. Explainable Reinforcement Learning (XRL):
- Focus: Breaking open the "black-box" nature of Deep RL to generate human-understandable explanations for the agent's decision and actions.

*Page 17*
Next is Human-Computer Interaction (HCI) and UX/UI Research leverages RL to create interfaces that is specifically catered to an individual over time, rather than presenting a static design.

1. Model-Based RL for User-Adaptive Interfaces:
- Focus: Building an internal model of the user. Unlike model-free RL which purely learns through trial and error, model-based RL uses simulation to simulate the consequences of an adaptation before applying it.

2. Interactive Reinforcement Learning (IRL) for Feedback:
- Focus: To make the ai agent learn faster by incorporating direct human guidance during the learning process. Instead of waiting for a high-level reward signal, the agent can receive real time advice, corrections, or demonstrations from the user.

*Page 18*
Last is Behavioral Modeling and Multi-Agent Systems applies advanced RL techniques to study and create realistic digital behaviors, from predicting individual choices to managing large-scale interactions between numerous AI agents.

1. Inverse Reinforcement Learning (IRL) for Behavioral Cloning
- Focus: instead of giving a reward function a learning a policy, the agent is given expert human demonstrations and attempts to understand the reward function that motivated this behavior.

2. Multi-Agent Reinforcement Learning (MARL) and Coordination
- Focus: Involving multiple independent ai agents learning to interact within a shaerd environment. This is the foundation for managing complex systems such as traffic control, warehouse robotics, and the financial markets.

  *Page 20*
  And that is the end of chapter 2.....
