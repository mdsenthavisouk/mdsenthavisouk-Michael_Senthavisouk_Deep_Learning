# Visualization Inventory — L09 Pole Balancing RL

## Graphs

### 1. `random_agent_score_baseline.png`
- **Description:** Bar chart showing scores from 10 episodes of a completely random agent on CartPole-v1.
- **Key Metric:** Average score = 17.3 (out of a maximum 500).
- **Purpose:** Establishes the baseline — what performance looks like with zero learning.

### 2. `q_learning_training_progress.png`
- **Description:** Two-panel chart showing Q-Learning training over 500 episodes.
  - **Top panel:** Raw episode scores (blue) with 50-episode rolling average (orange). Includes reference lines for perfect score (500) and random agent average (17.3).
  - **Bottom panel:** Epsilon (exploration rate) decay curve from 1.0 to ~0.08 over training.
- **Key Metrics:**
  - First 50 episodes average: 22.7
  - Last 50 episodes average: 65.1
  - Final epsilon: 0.0816
- **Purpose:** Shows the agent learning over time — scores rise as epsilon falls.

### 3. `epsilon_decay_reward_comparison.png`
- **Description:** Rolling average comparison of three agents trained with different epsilon decay rates.
  - Agent A (fast decay, 0.990): last-50 avg = 36.4
  - Original (medium decay, 0.995): last-50 avg = 65.1
  - Agent B (slow decay, 0.999): last-50 avg = 42.4
- **Purpose:** Demonstrates the exploration/exploitation tradeoff — medium decay balances learning best.
