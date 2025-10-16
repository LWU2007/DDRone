7 tf questions
7 multiple choice
2 open ended questions



tf questions:

- Is MDP derived from the Markov Chain?
  TRUE
  
- Online reinforcement learning is more useful than offline to train driverless vehicles.
  FALSE

- One of the use cases for reinforcement learning is to train cars to drive on their own
  TRUE
  
- In offline reinforcement learning, the ai can interact with the environment while training.
  FALSE
  
- MDP is defined by a state, action, transition probability, reward function, and discount factor.
  TRUE
  
- We can freely use ai without any consequences.
  FALSE
  
- One of the core fundementals of reinforcement learning is the agent itself.
  TRUE



multiple choice questions:

- Which is not the basic fundementals of reinforcement learning?
+ agent
+ environment
+ state
+ punishment (ANSWER)

- The key elements of reinforcement learning is
+ policy
+ reward signal
+ model
+ agent (ANSWER)

- Where is the Markov Decision Process derived from?
+ Markov's rule
+ Stein's gate rule
+ Stein's decision process
+ Markov chain (ANSWER)

- This is part of the Markov Chain
+ agent
+ punishment
+ reward
+ state (ANSWER)

- What is an agent in reinforcement learning?
+ person who acts on your behalf
+ a person or thing that takes an active role or produces a specified effect
+ a platypus in disguise
+ the one who learns and decides on how to interact with the environment to achieve a certain goal (ANSWER)

- what makes online reinforcement learning different that offline?
+ it continuously adapts
+ data always matches with the current policy
+ it can interact with the environment while training
+ it is cheaper than offline reinforcement learning (ANSWER)



open ended questions

- is online or offline reinforcement learning the better option in training your machine learning project?
  These solely depend on what project you are trying to create, there is no one size fits all solution to this. While offline is best suited for scenarios where online interaction with the environment is costly, dangerous, or unethical. It excels at learning policis from large pre-collected data sets wwithout needing to experiment in real time. While online is best suited for problems that require real-time, sequential decision-making in dynamic environments where an agent learns from direct interaction and can adapt to changing data. This is ideal for applications such as robotics and real-time control systems due to it being able to adapt its policy at real time due to the uncertain and unpredictable feedbacks.

- explain how the Markov Decision Chain is connected to the Markov Chain! (optional: explain why they use the Markov Chain instead of any other probability processes such as the Possion Process)
  The Markov Decision Chain is built upon the Markov Chainby adding the element agent, reward, and action which now influences the transition probability. All of these elements added to the Markov Chain makes it a framework for decision making the agent is able to make its own decision which adds an element of choice to the random probability states of the base Markov Chain.

  (Optional) The markov chain is used instead of any other processes is solely because that the probability of transitioning to another state from the current state is solely dependent on the current state and making it "memoryless". This "memoryless" property makes systems easier to analyse and predict, even help simplify calculations and help reduce the amount of data needed.
