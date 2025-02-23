# Local Search Algorithms for Graph Optimization

This repository contains implementations of three algorithms—**Brute Force**, **Hill Climbing**, and **Simulated Annealing**—to solve a graph optimization problem. The goal is to select a subset of nodes from a graph such that the induced subgraph has the maximum sum of edge weights.

## Problem Definition

Given a graph with 20 nodes and edges between each pair of nodes, the task is to select 5 nodes such that the sum of the edge weights in the induced subgraph is maximized. The project implements three algorithms to solve this problem:

1. **Brute Force**: A naive approach that explores all possible combinations of 5 nodes to find the optimal solution.
2. **Hill Climbing**: A local search algorithm that starts with a random solution and iteratively improves it by exploring neighboring states.
3. **Simulated Annealing**: A probabilistic optimization algorithm that allows for occasional worse solutions to escape local optima and potentially find a better global solution.


## Algorithms

### 1. Brute Force
The brute force algorithm exhaustively checks all possible combinations of 5 nodes and calculates the sum of edge weights for each combination. It returns the combination with the highest sum.

### 2. Hill Climbing
The hill climbing algorithm starts with a random selection of 5 nodes and iteratively improves the solution by exploring neighboring states. A neighbor state is defined as a state where one node is swapped with another node not in the current selection. The algorithm stops when no better neighbor is found.

### 3. Simulated Annealing
Simulated annealing is a probabilistic optimization algorithm that starts with a random solution and explores neighboring states. It allows for occasional worse solutions to escape local optima. The probability of accepting worse solutions decreases over time as the "temperature" cools down.

## Results

The notebook compares the results of the three algorithms across different random seeds. The brute force algorithm provides the optimal solution, while hill climbing and simulated annealing provide approximate solutions. The results show how close the approximate algorithms are to the optimal solution.

