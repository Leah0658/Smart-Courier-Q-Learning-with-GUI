
# Smart Courier: A Q-Learning Agent in Grid World

This project implements a reinforcement learning agent using Q-learning to learn optimal policies in a custom-built Grid World environment. The agent learns to pick up an item and deliver it to a target location within a 2D grid while being visualized in real-time using a graphical user interface (GUI) built with Tkinter.

## Overview

The environment is a 5x5 grid where an agent must:
1. Locate and collect a randomly placed item.
2. Navigate to a fixed target cell while carrying the item.
3. Receive feedback via a reward mechanism to optimize its behavior.

The learning algorithm uses tabular Q-learning with an ε-greedy strategy and updates Q-values for each state-action pair based on experience.

## Objectives

- Train a Q-learning agent to learn efficient delivery strategies.
- Visualize the learning process using a dynamic GUI.
- Track and compare actual vs optimal steps taken by the agent during training.

## Features

- Custom Grid World environment with agent, item, and target objects.
- Tkinter-based GUI for step-by-step visualization.
- Q-learning agent with customizable parameters:
  - Learning rate (α)
  - Discount factor (γ)
  - Exploration rate (ε)
- Reward system:
  - −1 per step
  - +10 for picking up item
  - +100 for successful delivery
- Real-time performance statistics:
  - Number of episodes
  - Steps taken
  - Time elapsed
  - Optimal steps vs actual steps

## Screenshots

> Note: You may need to close the GUI window manually after training to continue execution.

![Agent Screenshot](icon/agent.png)
![Item Screenshot](icon/item.png)
![Target Screenshot](icon/target.png)

## Results

After training, a plot is generated comparing the agent’s actual steps vs the theoretical optimal steps for each episode, helping to measure the agent's learning performance over time.

## How to Run

> **Warning:** Full training may take up to 10 minutes depending on machine performance.

1. Make sure you have Python 3 and required libraries installed:
   ```bash
   pip install numpy matplotlib pillow


2. Place the required image files in an `icon/` folder:

   * `agent.png`
   * `item.png`
   * `target.png`

3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook 5226\ ass1.ipynb
   ```

4. Follow in-notebook instructions. Training will launch a GUI and begin automatically.

## 📁 Project Structure

```
├── smart-courier-qlearning-gridworld.ipynb        # Main training and visualization notebook
├── icon/
│   ├── agent.png          # Agent icon
│   ├── item.png           # Item icon
│   └── target.png         # Target icon
```

## Dependencies

* Python 3.x
* numpy
* matplotlib
* tkinter (built-in with Python)
* pillow (PIL)

## Learning Concepts

* Reinforcement Learning
* Q-learning
* ε-Greedy Policy
* Markov Decision Process
* Grid-based Environment Modeling
* GUI-based Simulation

## Author

YA LIU

Master of Artificial Intelligence, Monash University

July 2025

---

Feel free to fork, extend, or adapt this project for your own research or experimentation in reinforcement learning.

```