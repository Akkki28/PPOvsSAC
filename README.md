# PPOvsSAC
Research suggests that the top two most used reinforcement learning algorithms in robotics applications are Proximal Policy Optimization (PPO) and Soft Actor-Critic (SAC), due to their effectiveness in continuous control tasks. It seems likely that PPO is more widely used in simulation, while SAC is preferred for real-world robotics due to its sample efficiency and off-policy nature. This work tries to compare the performance of these two popular algorithms across different robotics based reinforcement learning environments

## Performance Comparison

| Environment             | Metric         | PPO           | SAC           |
|--------------------------|----------------|---------------|---------------|
| AdroitHandDoor           | Best Average Reward | -86.74        | -80.13         |
|                         | Time Taken     | 2 mins 47s        | 11 mins 52s        |
| FetchReach               | Best Average Reward | -15.55         | -7.85         |
|                         | Time Taken     | 2 mins 36s        | 6mins 21s         |
| PickAndPlace             | Best Average Reward | -26.18         | -27.44         |
|                         | Time Taken     | 3 mins 11s        | 6mins 22s         |
| Push                     | Best Average Reward | -22.62        | -22.22        |
|                         | Time Taken     | 2mins 22s         | 12 mins 33s        |
| Slide                    | Best Average Reward | -31.60         | -31.39         |
|                         | Time Taken     | 2 mins 52s        | 12 mins 12 s        |

# Conclusion
The comparison between PPO and SAC across different Robotic environments shows that SAC consistently achieves higher average rewards, whereas PPO converges faster. I suspect that SAC's superior performance is due to its entropy maximization, which enhances exploration, which is considered particularly valuable in such settings. However, SAC's off-policy learning and use of twin Q-networks increase computational complexity, leading to longer training times. In contrast, PPO's on-policy updates are more sample-efficient, resulting in faster convergence. Therefore, SAC is preferable for maximizing performance, while PPO is more suitable when training speed is a priority.
