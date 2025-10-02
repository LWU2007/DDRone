Now this is the last step to understanding the fundamentals of reinforcement learning ai. All that's left for us to understand is how the agent acquires and utilizes data.

First is through online reinforcement learning; the agent learns through direct and live interaction with the environment. As the agent takes an action, it immediately receives a new state and a reward, which are used to update its policy in real-time or after short batches.
For example, a robot is learning how to walk. When the robot attempts to move its legs (action), it immediately observes the result (state: {fell or moved forward}) and receives a reward ({-} if fell and {+} if it's moving). It then instantly uses this to adjust its new walking policy for the next step.

This has an advantage of: 
- continuously adapting to a changing environment.
- maximizes performance by achieving the optimal policy by exploring and collecting new, highly relevant data.
- the data collected always matches the agent's current policy (on-policy), avoiding data mismatch issues.

But this also has a disadvantage of:
- the agent performing unsafe or highly suboptimal actions during the learning phase (i.e robots crashing).
- requiring continuous, real-time compute resources attached to the environment making it highly expensive and slow to operate.


Second is through offline reinforcement learning; the agent solely focuses learning a policy of static and precollected dataset of experiences. The agent is not allowed to interact with the environment during the training process.
For example, a company training an autonomous vehicle policy. A company collected data of millions of driving hours and is using that to train the agent on this fixed and massive data set (state, action, reward, next state). It then learns the best course of action for each recorded state whilst not being able to test its policy on the real world.

This has an advantage of:
- removing the risk of dangerous exploration and making it ideal for safety-critical domains (healthcare and autonomous driving).
- being able to be trained flexibly and on pre-allocated compute resources without needing real-time environment access.
- leveraging historical data collected over years, which is often infeasable for a single training run.

But it also has the disadvantage of:
- the agent's learnt policy that may choose actions not seen in the dataset(out-of-distribution), leading to an uncertain and highly-unreliable performance.
- the policy's performance that is fundementally limited by the quality and coverage of the static dataset.
- requiring complex and specialized algorithms yo correct for the distributional shift problem.