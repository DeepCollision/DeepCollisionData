# Public Data for Peer Review of DeepCollision 

```
To facilitate reviewing our proposed approach, reviewers please refer to the corresponding data in this repository: 
Piloty Study, all data and figures for the pilot study; 
Formal Experiment, all data for the formal experiment; 
Restful APIs, all implemented REST APIs for environment parameters.
```

## 1. Overview of DeepCollision

**DeepCollision** learns environment configurations to maximize collisions of an Autonomous Vehicle Under Test (AVUT). As shown in the following figure, DeepCollision employs a *Simulator* (e.g., LGSVL) to simulate the *Testing Environment* comprising the AVUT and its operating environment. DeepCollision also integrates with an *Autopilot Algorithm Platform* (e.g., the Baidu Apollo ) deployed on the AVUT to enable its autonomous driving.

<div align=center><img width="500" height="500" src="https://github.com/DeepCollision/DeepCollisionData/blob/main/figures/Overview.png"/ "Magic Gardens"></div>

**DeepCollision** employs a DQN component to generate a set of actions to configure the environment of the AVUT, e.g., weather condition, time of day. At each time step $t$, the DQN component observes a state $S_t$ describing the current states of the AVUT and its environment. With the state, DeepCollision decides an action $A_t$ based on the Q-network with the policy $\pi$. With our developed *Environment Configuration REST API*, such an action $A_t$ can be considered as an HTTP request for accessing the simulator to introduce new environment configurations. After the AVUT driving into a new environment within a fixed time period, both the AVUT and its environment will enter a new state $S_{t+1}$. Based on the observed states of the AVUT and its environment, *Reward calculator* calculates a reward $R_{t}$ for $A_t$ and $S_{t}$ at $t+1$. Then DQN stores them (as $<S_t$, $A_t$, $R_t$, $S_{t+1}>$) into the replay memory buffer.

Once the replay memory is full, Q-network will be updated based on the loss function by a mini-batch randomly selected from the updated replay memory. In addition, with $S_{t+1}$, the (updated) Q-network with policy $\pi$ decides the next action: $A_{t+1}$. In DeepCollision, an episode is finished once the AVUT arrives at its destination or the AVUT cannot move for a specific duration. At each time step $t$, the information about the AVUT (e.g., its driving and collision status) and its environment (e.g., its status and driving scenarios) are stored as *Environment Configuration Logs* for further analyses and collision replaying. 
More details of Hyper-parameters of DQN used in DeepCollision can be accessed here \cite{DeepCollisonRepository}.

Once the replay memory is full, Q-network will be updated based on the loss function by a mini-batch randomly selected from the updated replay memory. In DeepCollision, an episode is finished once the AVUT arrives at its destination or the AVUT cannot move for a specific duration. At each time step, the information about the AVUT (e.g., its driving and collision status) and its environment (e.g., its status and driving scenarios) are stored as *Environment Configuration Logs* for further analyses and collision replaying.
