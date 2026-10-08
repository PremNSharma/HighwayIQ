# HighwayIQ

A reinforcement learning project that trains an autonomous driving agent to perform safer overtaking decisions in a simulated highway environment.

## Overview

HighwayIQ explores decision-making for autonomous vehicles using a **Deep Q-Network (DQN)**. The agent learns from simulated highway states and a custom reward design that encourages safe, efficient, and smooth driving behavior.

## Key Features

- Deep Q-Network based decision making
- Highway simulation with `highway-env`
- Custom reward design for safety and driving efficiency
- Training and demonstration workflows
- Real-time simulation visualization
- Automatic loading of trained model files
- Optional CUDA/GPU acceleration

## Technical Stack

- Python
- PyTorch
- Stable-Baselines3
- highway-env
- Gymnasium
- NumPy
- Matplotlib
- CUDA (optional)

## Project Structure

```text
HighwayIQ/
├── main.py                    # DQN training workflow
├── demo_final_autoload.py     # Trained-agent demonstration
├── rl_overtake_safe_realistic_v2.zip
├── output.jpg
└── README.md
```

## Run

Install the required dependencies for the project, then train the agent:

```bash
python main.py
```

Run the trained-agent demonstration:

```bash
python demo_final_autoload.py
```

The existing trained model can be used to skip training when available.

## Reward Design

The environment rewards desirable driving behavior while penalizing unsafe decisions. The current setup considers factors such as safety, speed, lane-change efficiency, and collisions.

## Project Goal

Use reinforcement learning and simulation to study how an autonomous agent can learn safer highway decision-making under dynamic traffic conditions.

## Author

**Prem Sharma**

GitHub: https://github.com/PremNSharma
