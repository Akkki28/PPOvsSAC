# PPOvsSAC
Research suggests that the top two most used reinforcement learning algorithms in robotics applications are Proximal Policy Optimization (PPO) and Soft Actor-Critic (SAC), due to their effectiveness in continuous control tasks. It seems likely that PPO is more widely used in simulation, while SAC is preferred for real-world robotics due to its sample efficiency and off-policy nature. This work tries to compare the performance of these two popular algorithms across different robotics based reinforcement learning environments

## Performance Comparison Across Environments  

| Environment            | Metric             | PPO           | SAC           |
|------------------------|--------------------|---------------|---------------|
| Env 1 (e.g., HalfCheetah) | Average Reward      | X ± Y         | A ± B         |
|                        | Convergence Steps   | X Steps       | A Steps       |
|                        | Stability (Variance)| X             | A             |
| Env 2 (e.g., Ant)      | Average Reward      | X ± Y         | A ± B         |
|                        | Convergence Steps   | X Steps       | A Steps       |
|                        | Stability (Variance)| X             | A             |
| Env 3 (e.g., Humanoid) | Average Reward      | X ± Y         | A ± B         |
|                        | Convergence Steps   | X Steps       | A Steps       |
|                        | Stability (Variance)| X             | A             |

**Notes:**  
- Average Reward: Mean ± Standard Deviation over multiple runs.  
- Convergence Steps: Number of steps required to reach a stable reward.  
- Stability: Variance in reward during the training process.  
