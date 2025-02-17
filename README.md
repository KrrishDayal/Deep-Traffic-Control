# SmartTraffic-DQN  
A Deep Q-Network (DQN)-based traffic signal optimization system to reduce congestion and improve traffic flow.

## Features  
- **Custom Gym Environment**: Simulates a traffic signal with dynamic traffic conditions.  
- **Deep Q-Network (DQN)**: Implements reinforcement learning for optimal signal control.  
- **Experience Replay**: Improves training stability and efficiency.  
- **Epsilon-Greedy Exploration**: Balances exploration and exploitation.  
- **Performance Visualization**: Plots reward progression, action distributions, and traffic density trends.  

## Results
The training process is logged, and key metrics like rewards, epsilon decay, and traffic densities are visualized using Matplotlib.

## Technologies Used
- Python
- OpenAI Gym
- PyTorch
- NumPy
- Matplotlib

## To-Do
- Improve reward function for better traffic flow.
- Integrate with real-world traffic data.
- Extend to multi-intersection control.

## License
This project is licensed under the MIT License.


## 🔍 Overview  
Traffic congestion is a major issue in urban areas, leading to delays, fuel wastage, and increased pollution. Traditional traffic signals operate on **fixed timers**, which are often inefficient. This project explores a **reinforcement learning approach** where an **AI agent** controls traffic signals by learning optimal phase-switching strategies through interaction with a simulated environment.  

The agent is trained using a **Deep Q-Network (DQN)** and learns to **reduce overall congestion** by minimizing the sum of traffic densities in all directions. 

## How It Works  
1. The environment simulates traffic conditions with **randomized vehicle densities**.  
2. The agent receives an observation of the **current traffic density** in four directions.  
3. The agent selects an **action**:  
   - **0**: Keep the current traffic light phase.  
   - **1**: Switch to the alternate phase.  
4. The **environment updates traffic densities** based on the selected action.  
5. The agent receives a **reward** (negative sum of traffic densities) and updates its strategy.  
6. The training continues for multiple episodes until the agent learns an optimal policy.  

## Installation  
### Prerequisites  
Ensure you have **Python 3.7+** installed.  


