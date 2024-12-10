# Hybrid Artificial Neural Network Optimization (GA & PSO)

This repository demonstrates the use of **Genetic Algorithm (GA)** and **Particle Swarm Optimization (PSO)** in optimizing Artificial Neural Networks (ANN). The implementation is divided into three stages: 

1. **Simple GA Example**: Optimization of a basic mathematical function \(x^2\).
2. **MLP Model Creation**: Training an ANN on the California Housing dataset.
3. **Hybrid ANN Optimization**: Combining ANN with GA and PSO for advanced optimization.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Project Workflow](#project-workflow)
3. [How It Works](#how-it-works)
    - [Stage 1: Simple GA](#stage-1-simple-ga)
    - [Stage 2: MLP Model Creation](#stage-2-mlp-model-creation)
    - [Stage 3: Hybrid Optimization](#stage-3-hybrid-optimization)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Results](#results)
7. [Files and Structure](#files-and-structure)
8. [License](#license)

---

## Introduction

The optimization of neural networks is critical for achieving high performance. Traditional backpropagation has limitations, such as susceptibility to local minima and dependence on gradient information. **GA** and **PSO** are nature-inspired optimization techniques that improve ANN performance by exploring and exploiting the search space more effectively.

This project covers:
1. A basic introduction to **GA** through a mathematical optimization example.
2. Training a **Multi-Layer Perceptron (MLP)** model on a real-world dataset.
3. Combining **GA** and **PSO** with ANN to demonstrate hybrid optimization.

---

## Project Workflow

1. **Stage 1: Simple GA Example**:
   - Optimize the mathematical function \(f(x) = x^2\) using GA.
   - Demonstrates the basic workflow of selection, crossover, and mutation.

2. **Stage 2: MLP Model Creation**:
   - Train a **Multi-Layer Perceptron (MLP)** model using the **California Housing** dataset.
   - Demonstrates traditional training using backpropagation.

3. **Stage 3: Hybrid Optimization**:
   - Replace backpropagation with **GA** and **PSO** to optimize ANN weights and biases.
   - Compare the performance of traditional training vs. hybrid optimization.

---

## How It Works

### Stage 1: Simple GA

- **Objective**: Maximize \(f(x) = x^2\) where \(x \in [0, 31]\).
- **Implementation Steps**:
  - **Population Initialization**: Randomly generate candidate solutions.
  - **Selection**: Use fitness-proportional selection (roulette wheel).
  - **Crossover**: Combine parent solutions to create offspring.
  - **Mutation**: Randomly alter genes to introduce diversity.

### Stage 2: MLP Model Creation

- **Dataset**: Uses the **California Housing** dataset, fetched using `sklearn.datasets.fetch_california_housing`.
- **Model Architecture**:
  - Input Layer: 8 features.
  - Hidden Layers: Configurable.
  - Output Layer: Single neuron (for regression).
- **Training**:
  - Loss Function: Mean Squared Error (MSE).
  - Optimizer: Adam (traditional backpropagation).

### Stage 3: Hybrid Optimization

- **Objective**: Train the MLP using **GA** and **PSO** instead of backpropagation.
- **Workflow**:
  - Initialize weights and biases as candidate solutions.
  - Use **GA** for exploration and **PSO** for fine-tuning.
  - Evaluate fitness as the negative MSE of the network on the dataset.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Hybrid-ANN-GA-PSO.git
   cd Hybrid-ANN-GA-PSO
