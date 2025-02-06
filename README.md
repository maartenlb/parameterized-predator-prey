# Evolutionary Hunter-Prey Simulation in NetLogo

## Overview

This NetLogo model simulates an **evolutionary hunter-prey system**, where **hunters** evolve over generations to improve their ability to track and catch a moving **target**. The simulation uses a **genetic algorithm** with selection, crossover, and mutation to refine the hunters' strategies over time.

![model](https://github.com/maartenlb/parameterized-predator-prey/blob/main/Capture.PNG)

## Features

- **Agent-based Evolution**: Hunters inherit traits and evolve using a **tournament-based genetic algorithm**.
- **Adaptive Behavior**: Hunters adjust their movement based on the target's position.
- **Mutation and Crossover**: Offspring inherit and mutate their genotype to improve performance.
- **Tracking Metrics**: The simulation tracks **average score, maximum score, and evolutionary trends**.

## Time Complexity

- **Movement & Simulation**: **O(n × f)**  
  - `n` = number of hunters  
  - `f` = frames per run  
- **Genetic Algorithm (Selection + Mutation + Crossover)**: **O(n log n)**  
- **Overall Complexity**: **O(n log n + n × f)** (scales with population size and frames per run)

## Usage

1. **Load the NetLogo model**.
2. Run `setup` to initialize hunters and targets.
3. Start the simulation with `go`, where hunters evolve to improve their tracking ability.
4. Adjust parameters such as **population size, mutation rate, and tournament size** using predefined functions like `Populous` or `Mutants`.

## Notes

- The model visualizes **how evolutionary pressure shapes behavior** in a hunter-prey environment.
- Evolutionary progress is tracked using **moving averages** of scores.
- Different setups (`Default`, `Populous`, `Mutants`) provide varying population and mutation dynamics.

---

*For questions or contributions, feel free to open an issue or submit a pull request!*
