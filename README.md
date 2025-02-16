# ConnectX AI Agents 🎮🤖

Welcome to the **ConnectX AI Agents** project! This repository contains AI agents trained to play the ConnectX game using reinforcement learning algorithms. The goal is to create agents that can learn from experience and eventually win against default agents like `random` and `negamax`.

---

## 🌟 Introduction

In this project, we use the **Kaggle ConnectX environment** to train AI agents to play ConnectX. The objective is to create agents that can learn from experience and eventually win against default agents like `random` and `negamax`. The project involves implementing various reinforcement learning algorithms, including Q-Learning, Sarsa(λ), and REINFORCE-with-Baseline.

---

## 📦 Deliverables

1. **Notebook/Python Files**: The project includes a Jupyter notebook or Python files where the agents are created and trained. 
2. **Saved Models**: After training, the learned values are saved for future use.

3. **Report**: A short report (up to 10 pages) explaining the methodology, chosen algorithms, and visualizations of the learning process (e.g., rewards over time, loss functions).

---

## 📊 Evaluation

The project is evaluated based on:
- **Development of Agents (70%)**: Proper implementation and functionality of the agents.
- **Performance (30%)**: How well the agents perform against default agents (`random`, `negamax`) and each other.

---

## 🤖 Agents

### 1. Q-Learning Agent
- **Algorithm**: Q-Learning
- **Description**: This agent uses Q-Learning to learn the optimal policy by updating Q-values based on the Bellman equation.
- **Training**: The agent is trained against a `random` opponent and a `negamax` opponent.
- **Saved Model**: `q_learning_agent1.pkl`, `q_learning_agent2.pkl`

### 2. Sarsa(λ) Agent
- **Algorithm**: Sarsa(λ)
- **Description**: This agent uses the Sarsa(λ) algorithm, which incorporates eligibility traces to improve learning efficiency.
- **Training**: The agent is trained against a `random` opponent and a `negamax` opponent.
- **Saved Model**: `SarsaLambdaAgent.npy`, `SarsaLambdaAgent_negamax.npy`

### 3. REINFORCE-with-Baseline Agent
- **Algorithm**: REINFORCE-with-Baseline (Monte-Carlo Policy Gradient)
- **Description**: This agent uses policy gradient methods to learn the optimal policy by maximizing the expected reward.
- **Training**: The agent is trained using Monte-Carlo methods with a baseline to reduce variance.

---

## 🛠 Installation

To run this project locally, you need to install the Kaggle environments:

```bash
!pip install kaggle-environments --quiet
```

---

## 🚀 Usage

1. **Training the Agents**:
   - Run the training cells in the notebook to train the Q-Learning and Sarsa(λ) agents.
   - The trained models will be saved to the specified paths.

2. **Testing the Agents**:
   - Use the provided wrapper functions (`call_agent_1`, `call_agent_2`) to test the agents against each other or against default agents.
   - Visualize the game using `env.render(mode="ipython")`.

3. **Evaluating Performance**:
   - Run the evaluation cells to compare the performance of the agents over a series of games.

---

## 📈 Results

The performance of the agents is evaluated based on their win percentages against `random` and `negamax` opponents. The results are displayed after training and testing the agents.

---

## 🤝 Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

---


## 🙏 Acknowledgments

- [Kaggle ConnectX Environment](https://github.com/Kaggle/kaggle-environments)
- Reinforcement Learning Algorithms (Q-Learning, Sarsa(λ), REINFORCE)
