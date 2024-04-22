# ECE_7202_Final_Project
## 1. Path planning using value iteration
If both the map and model are know, we use value iteration to find the optimal value functions V* and the optimal path is derived using a greedy policy.

### Model
**Action space S**: up/down/left/right/stay​

**Reward**: **0** for each action; **+10** if enter the goal position (discounting factor = 0.99)​

Task ends when the agent reaches the goal
### Single agent, static enviroment
![alt text](figures_and_results/value_iteration_32x32.gif)
### Single agent, dynamic enviroment
The location of dynamic obstacles is initialized randomly, and move randomly for each step​

Robot is aware of the nearby obstacles, but doesn't know where they will move
![alt text](figures_and_results/path_planning_dynamic_env.PNG)
![alt text](figures_and_results/value_iteration_64x64_100_dynamic_obs.gif)

## 2.Path planning using TD method
If the map is unknow, the robot needs to explore the enviroment and find the optimal path

### Single Agent (SARSA/Q-learning, n-steps SASA/Q-learing)
![alt text](figures_and_results/Q_learning_single_agent.PNG)
### Mulitple Agents (simultaneously Q-learining)
![alt text](figures_and_results/multi-agent.gif)![alt text](figures_and_results/Q_learing_multi_agents.gif)

## 3. Real application
Preprocess the image
![alt text](figures_and_results/Real_map_preprocessing.PNG)
learned path
![alt text](figures_and_results/path_plan_realistic_world.gif)

