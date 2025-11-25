# AI-Driven Self-Healing Critical Infrastructure Networks

## Overview
This project implements a Deep Q-Network (DQN) reinforcement learning system for autonomous reconfiguration of critical infrastructure networks (power grids, communication systems) during large-scale disasters. The AI agent learns to dynamically allocate resources, isolate failures, and restore connectivity without human intervention.

## Key Features
- **Autonomous Failure Response**: AI-driven decision making for network reconfiguration
- **Real-time Visualization**: Grad-CAM interpretability and network state monitoring
- **Synthetic Environment**: Realistic grid topology simulation with failure scenarios
- **Performance Analytics**: Comprehensive evaluation metrics and comparison with traditional methods

## Model Architecture
- **Deep Q-Network**: 3 hidden layers (128-64-32 neurons) with ReLU activation
- **State Representation**: 20-dimensional feature vector capturing topology, component status, and failure indicators
- **Action Space**: Three primary actions - Maintain, Activate Backup Paths, Emergency Reconfigure
- **Training Method**: Experience replay, target network, epsilon-greedy exploration

## Dataset
Synthetic power grid dataset with:
- 15-node network topologies (substations + distribution nodes)
- Multiple failure scenarios (single component to cascading failures)
- Class imbalance handling through strategic sampling and reward engineering

## Installation & Requirements
```bash
pip install torch torchvision numpy matplotlib networkx scikit-learn seaborn pandas
