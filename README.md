# snakegameQ
An automated agent based on the concept of Q-Learning for playing the popular snake game.

# Features

Q-Learning with Deep Neural Networks: policy & target networks for stability.

State Representation: 11 engineered features capturing food direction, obstacles, and snake body position.

Neural Network Architecture: MLP (11 → 1024 → 3) with ReLU activations.

Exploration Strategy: exponential epsilon decay, optimized for convergence.

Reward Shaping: penalizes loop traps & moving away from food, encourages efficient paths.

Results: average score ~30; highest scores reaching 80–90+.

# Results & Visuals

| Metric                  | Value               |
| ----------------------- | ------------------- |
| Avg score (over N runs) | \~30                |
| Best score              | 80–90+              |
| Network                 | 11-1024-3 MLP       |
| Exploration             | Exponential epsilon |


# Experiments

Compared linear vs exponential epsilon decay.

Analyzed reward shaping impact on agent’s survival.

Tested stability improvements with target vs policy networks.
