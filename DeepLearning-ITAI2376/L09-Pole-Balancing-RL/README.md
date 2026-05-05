# L09 — Reinforcement Learning: Pole Balancing with Q-Learning

## Project Overview

In this lab, I trained a reinforcement learning agent to balance a pole in **CartPole-v1**. I started with a random baseline, then implemented and evaluated a Q-Learning strategy.

## Problem Statement

I investigated how an agent improves over episodes through reward-driven learning and how exploration settings impact training outcomes.

## My Approach

1. Ran a random policy baseline for reference
2. Trained a Q-Learning agent with discretized state bins
3. Tracked episode scores and moving averages
4. Compared epsilon decay variants for exploration/exploitation behavior

## Environment / Dataset

- **Gymnasium CartPole-v1** simulation environment

## Technologies Used

- Python
- gymnasium
- NumPy
- Matplotlib

## Key Results

From notebook outputs:
- Random baseline average score: **15.5**
- Q-Learning final average (last 50 episodes): **80.3**
- Improvement from first 50 episodes (**24.1**) to last 50 (**80.3**)
- Epsilon schedule comparison:
  - Fast decay (0.990): 44.6
  - Slow decay (0.999): 36.2
  - Original (0.995): 80.3

## Visual Results

See `results/`:
- `random_agent_score_baseline.png`
- `q_learning_training_progress.png`
- `epsilon_decay_reward_comparison.png`
- `visualization_inventory.md`

## What I Learned

- RL performance depends heavily on exploration strategy.
- Baselines are critical for proving actual learning.
- Learning curves communicate agent progress better than a single score.
- This lab gave me practical intuition that connects directly to RLHF concepts in modern LLM systems.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Pole_Balancing_Q_Learning.ipynb
```
