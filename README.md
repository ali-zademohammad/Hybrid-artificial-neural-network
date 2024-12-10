# Hybrid Artificial Neural Network Optimization with GA and PSO

This repository demonstrates the implementation of **Genetic Algorithm (GA)** and **Particle Swarm Optimization (PSO)** in optimizing **Artificial Neural Networks (ANN)**. The project is divided into two main sections for each algorithm (GA and PSO), covering:

1. A simple mathematical optimization example using \(x^2\).
2. Building and training an **MLP** (Multi-Layer Perceptron) model with the **California Housing Dataset**.
3. Combining **ANN** with GA and PSO to optimize weights and biases, enhancing performance compared to traditional backpropagation.

---

## Table of Contents

    - [Genetic Algorithm (GA)](#[genetic-algorithm-ga](https://github.com/ali-zademohammad/Hybrid-artificial-neural-network/blob/85222e1ac2d5fc77ca618d03a191db3ee77e9880/Genetic%20Algorithm%20(GA).ipynb))
    - [Particle Swarm Optimization (PSO)](#particle-swarm-optimization-pso)

---

## Introduction

Traditional backpropagation is widely used for training Artificial Neural Networks (ANNs). However, it has limitations, such as susceptibility to local minima and reliance on gradient information. **Genetic Algorithm (GA)** and **Particle Swarm Optimization (PSO)** are powerful metaheuristic optimization techniques inspired by nature, capable of improving ANN training.

This repository explores:
1. Basic implementations of GA and PSO for mathematical optimization.
2. Training a Multi-Layer Perceptron (MLP) on real-world data.
3. Hybrid ANN optimization using GA and PSO to achieve better performance.

---

## Project Overview

### Genetic Algorithm (GA)

- **Stage 1**: A simple example optimizing \(x^2\).
    - Demonstrates how GA works through selection, crossover, and mutation.
- **Stage 2**: Training an MLP on the **California Housing Dataset** using backpropagation.
- **Stage 3**: Replacing backpropagation with GA for optimizing MLP weights and biases.

### Particle Swarm Optimization (PSO)

- **Stage 1**: A simple example optimizing \(x^2\).
    - Demonstrates PSO's particle-based approach.
- **Stage 2**: Training an MLP on the **California Housing Dataset** using backpropagation.
- **Stage 3**: Replacing backpropagation with PSO for optimizing MLP weights and biases.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Hybrid-ANN-GA-PSO.git
   cd Hybrid-ANN-GA-PSO
