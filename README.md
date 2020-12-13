## Taxi-v2 environment - RL solution


I used OpenAI Gym's Taxi-v2 environment to design an algorithm to teach a taxi agent to navigate a small gridworld. The goal is to adapt RL algorithm to solve a new environment!

Description of the environment can be seen in subsection 3.1 of [this paper](https://arxiv.org/pdf/cs/9905014.pdf)

The workspace contains three files:

* **agent.py:** Developing reinforcement learning agent here.
* **monitor.py:** The interact function tests how well your agent learns from interaction with the environment.
* **main.py:** Run this file in the terminal to check the performance of your agent.

When you run **main.py**, the agent specified in **agent.py** interacts with the environment for 20,000 episodes. The details of the interaction are specified in **monitor.py**, which returns two variables: **avg_rewards** and **best_avg_reward**

* **avg_rewards** is a deque where **avg_rewards[i]** is the average (undiscounted) return collected by the agent from episodes i+1 to episode i+100, inclusive. So, for instance, **avg_rewards[0]** is the average return collected by the agent over the first 100 episodes.

* **best_avg_reward** is the largest entry in **avg_rewards**. This is the final score that you should use when determining how well your agent performed in the task.
