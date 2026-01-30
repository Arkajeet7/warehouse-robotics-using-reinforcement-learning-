# Reinforcement Learning–Based Warehouse Robot 🤖📦

## Overview
This project focuses on developing an **intelligent warehouse robot** capable of **optimal path planning** in a dynamic warehouse environment using **Deep Reinforcement Learning (DQN)**.  
The work combines **simulation-based learning** with an ongoing **physical robot prototype** equipped with a **vacuum gripper** for pick-and-place operations.

---

## Project Objectives
- Model a grid-based warehouse environment with obstacles and goals
- Train a Reinforcement Learning agent to learn optimal navigation paths
- Minimize travel distance and collision with racks/obstacles
- Extend the trained policy to a real-world robotic system

---

## Key Features
- Custom **OpenAI Gym–style Warehouse Environment**
- **Deep Q-Network (DQN)** for decision-making
- Discrete action space: LEFT, RIGHT, UP, DOWN
- Reward shaping for efficient navigation
- Scalable design for real-robot deployment

---

## Environment Description
The warehouse is represented as a 2D grid:

| Symbol | Meaning |
|------|--------|
| 0 | Free path |
| 1 | Rack / Obstacle |
| S | Start position |
| I | Intermediate waypoint |
| G | Goal location |
| A | Agent |

---

## Reinforcement Learning Details
- **Algorithm**: Deep Q-Network (DQN)
- **State Space**: Grid position of the agent
- **Action Space**: 4 discrete movements
- **Reward Strategy**:
  - Positive reward for reaching goal
  - Penalty for collisions
  - Small negative reward per step to encourage shortest paths

---

## Tech Stack
- **Python**
- **NumPy**
- **OpenAI Gym**
- **PyTorch**
- **Matplotlib (visualization)**

---

## Repository Structure
├── environment/
│ └── warehouse_env.py
├── agent/
│ └── dqn_agent.py
├── training/
│ └── train.py
├── utils/
│ └── replay_buffer.py
├── results/
│ └── plots/
└── README.md

---

## Current Progress
- ✅ Warehouse environment implemented
- ✅ DQN agent trained in simulation
- ✅ Policy convergence observed
- 🔄 Hardware prototype under development

---

## Hardware (Ongoing Work)
- Differential-drive mobile robot
- Vacuum gripper for pick-and-place
- DC motors with motor driver IC
- Microcontroller-based control system
- Planned integration with trained RL policy

---

## Future Work
- Domain transfer from simulation to real robot
- Sensor noise and dynamic obstacle handling
- Multi-agent coordination
- Performance benchmarking against classical algorithms

---

## Applications
- Smart warehouses
- Autonomous logistics
- Industrial automation
- Research in robotics and reinforcement learning

---

## Author
**Arkajeet**  
Undergraduate Mechanical Engineering Student  
Focus: Robotics, Reinforcement Learning, Intelligent Systems

---

## License
This project is open for academic and educational use.
