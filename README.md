# Solving the Travelling Salesman Problem (TSP) using Genetic Algorithm

## Overview
The **Travelling Salesman Problem (TSP)** is a well-known **NP-hard** optimization problem that aims to determine the shortest possible route that visits a given set of cities exactly once and returns to the starting point. Since solving TSP optimally is computationally expensive, heuristic approaches such as **Genetic Algorithms (GA)** are used to find near-optimal solutions.

This repository implements **TSP optimization using Genetic Algorithms**, simulating natural selection principles such as selection, crossover, and mutation to iteratively improve a set of candidate solutions.

## Problem Statement
The goal is to **find the shortest possible tour** connecting a set of cities, given that:
- Each city must be visited **exactly once**.
- The salesman must return to the starting city.
- The route should be optimized to **minimize the total distance** traveled.

## Genetic Algorithm Approach
A **Genetic Algorithm (GA)** is used to approximate an optimal solution to TSP by:
1. **Creating an initial population**: Randomly generating candidate solutions.
2. **Evaluating fitness**: Assigning scores based on the total distance of each route.
3. **Selection**: Choosing the best-performing routes for reproduction.
4. **Crossover**: Combining parent routes to create new routes.
5. **Mutation**: Introducing small random changes to maintain diversity.
6. **Iterating**: Repeating the process for multiple generations until convergence.

### Key Components:
- **Gene Representation**: Cities are represented as (x, y) coordinates.
- **Fitness Function**: Lower-cost routes have higher fitness scores.
- **Crossover Strategy**: Ordered crossover is used to preserve valid routes.
- **Mutation**: Swapping two randomly selected cities in a route.
- **Elitism**: Best solutions are carried over to the next generation.

## Integer Linear Programming (ILP) for TSP
Beyond genetic algorithms, TSP can also be formulated as an **Integer Linear Programming (ILP)** problem, defining constraints to avoid sub-tours:
- **MTZ Method**: Uses integer variables to track city positions.
- **DFJ Method**: Ensures valid solutions by eliminating subtours iteratively.

## Results & Observations
1. **Genetic Algorithm** effectively finds near-optimal routes within **a reasonable time**.
2. **ILP-based TSP formulations** provide more accurate solutions but are computationally expensive.
3. **Comparative analysis** between **MTZ and DFJ** shows that **DFJ** is more efficient in solving large-scale TSP.

## Folder Structure
```
📂 Solving-TSP-with-Genetic-Algorithm
│── 📂 Paperwork/        # Project Report & Analysis
│── 📂 References/       # Research Papers & Sources
│── 📂 Source Code/      # Implementation of GA for TSP
│── 📜 README.md         # Project Documentation
```

## References
- Applegate, D.L., Bixby, R.E., Chvátal, V., Cook, W.J. *The Traveling Salesman Problem: A Computational Study.* Princeton University Press, 2006.
- Miller, C., Tucker, R., Zemlin, R. *Integer Programming Formulation of Traveling Salesman Problem.*
- Dantzig, Fulkerson, Johnson. *Branch-and-bound method for the TSP.*

## Author
[Rohith Ganesan](https://github.com/rohi52)

---

This README provides a **structured, professional, and detailed** documentation for your **Solving-TSP-with-Genetic-Algorithm** project. 🚀  
Let me know if you need **any modifications or additions**!
