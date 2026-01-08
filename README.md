# Hidden Markov Model Agent for Multi-Sensor State Estimation

Probabilistic AI · Sensor Fusion · State Estimation · Decision-Making

This project implements an **autonomous agent** that estimates the hidden state of a dynamic environment using a **Hidden Markov Model (HMM)** and makes decisions under uncertainty.

The agent fuses **multiple noisy sensors** and applies probabilistic filtering to support time-critical actions.

---

## Problem Statement
The true state of the environment (target location) is not directly observable.
Available sensors:
- GPS (coarse, noisy)
- Microphone signals (context-dependent noise)

The agent must:
- Maintain a belief distribution over states
- Update beliefs over time
- Decide **when and where to act** based on predicted future states

---

## Approach

### State Estimation
- Modeled environment dynamics using an HMM
- Maintained belief distributions over hidden states
- Implemented:
  - Prediction (transition model)
  - Update (sensor emission models)
  - Normalization

### Sensor Fusion
- Combined GPS and microphone observations probabilistically
- Augmented state to preserve first-order Markov assumptions

### Decision Logic
- Used **one-step-ahead belief prediction**
- Designed confidence-based decision heuristics
- Balanced risk vs. information gain

---

## Key Skills Demonstrated
- Hidden Markov Models
- Sensor fusion
- Probabilistic filtering
- Decision-making under uncertainty
- Applied AI for autonomous systems

---

## Use Cases
- Robotics and autonomous agents
- Tracking and localization
- Multi-sensor systems
- Real-time decision-support AI
