# Hybrid Artificial Neural Network with GA and PSO

This repository contains the implementation of a **Hybrid Artificial Neural Network (ANN)** model optimized using **Genetic Algorithm (GA)** and **Particle Swarm Optimization (PSO)**. The aim is to demonstrate how hybrid optimization techniques can enhance the performance of ANN models in solving regression or classification problems.

---

## Features

- **Neural Network Optimization**: Optimize ANN weights and biases using GA and PSO.
- **Hybrid Approach**: A combination of GA and PSO for global and local search capabilities.
- **Customizable Design**: Easy to modify the ANN architecture, GA, and PSO parameters.
- **Example Use Case**: Solves a regression problem using hybrid optimization techniques.

---

## Table of Contents

1. [Introduction](#introduction)
2. [How It Works](#how-it-works)
3. [Algorithms](#algorithms)
    - [Genetic Algorithm (GA)](#genetic-algorithm-ga)
    - [Particle Swarm Optimization (PSO)](#particle-swarm-optimization-pso)
    - [Hybrid Optimization](#hybrid-optimization)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Results](#results)
7. [License](#license)

---

## Introduction

Artificial Neural Networks (ANNs) are powerful tools for solving non-linear problems. However, traditional backpropagation-based training methods often get stuck in local minima. **GA** and **PSO** are nature-inspired optimization algorithms that address these limitations by efficiently exploring the search space.

This repository implements a hybrid framework that combines **GA's exploration capabilities** with **PSO's exploitation strengths**, providing a robust solution for optimizing ANN weights and biases.

---

## How It Works

1. **Population Initialization**:
   - The initial population (set of ANN weight and bias vectors) is randomly generated.
   
2. **Hybrid Optimization**:
   - **GA** performs crossover and mutation to explore the global search space.
   - **PSO** refines the solutions locally by adjusting particles' positions based on their velocities and fitness values.

3. **Fitness Evaluation**:
   - Each individual in the population is evaluated based on the ANN's performance (e.g., Mean Squared Error).

4. **Convergence**:
   - The algorithm iterates until a stopping criterion (e.g., maximum generations or desired error) is met.

---

## Algorithms

### Genetic Algorithm (GA)

1. **Selection**: Select parents using fitness-proportional selection (roulette wheel).
2. **Crossover**: Generate offspring by combining parents' genes.
3. **Mutation**: Introduce randomness to maintain diversity in the population.

### Particle Swarm Optimization (PSO)

1. **Particle Dynamics**: Each particle represents a candidate solution (ANN weights and biases).
2. **Velocity Update**: Update particle velocities based on:
   - Its own best-known position.
   - Global best position found by the swarm.

### Hybrid Optimization

1. **GA Phase**: Explore the search space to avoid local optima.
2. **PSO Phase**: Exploit promising regions of the search space for fine-tuning.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Hybrid-Artificial-Neural-Network.git
   cd Hybrid-Artificial-Neural-Network
