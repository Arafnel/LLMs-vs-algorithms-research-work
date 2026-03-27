# LLMs-vs-algorithms-research-work

This repository contains research on the efficiency and optimality of LLM-based planning agents compared to classical search algorithms (BFS, DFS, A*) in maze environments. This work was prepared for **IRC ACADEMIXHUB96**.

## Project Overview

The core objective of this research is to evaluate how modern Large Language Models (LLMs) perform as pathfinding agents when given a textual representation of a maze, versus traditional algorithmic approaches.

### Algorithms Compared
- **BFS (Breadth-First Search)**: Guaranteed to find the shortest path.
- **DFS (Depth-First Search)**: Explores as far as possible along each branch.
- **A* (A-Star)**: Uses heuristics to find the shortest path efficiently.

### LLMs Evaluated
- **Llama 3.1 70B**
- **Llama 3.1 8B**
- **GPT-OSS 20B** (via Groq API)

## Methodology

1.  **Maze Generation**: Mazes are procedurally generated with a fixed seed to ensure fair comparison. Random cycles are added to increase complexity.
2.  **Prompting Strategy**: LLMs are provided with a 2D grid representation and specific rules (start, goal, walls, open cells). A multi-turn conversation or specific instruction formatting is used to improve model reasoning.
3.  **Metrics**:
    - **Path Length**: Compared against the optimal BFS path.
    - **Success Rate**: Ability to reach the goal without hitting walls or going out of bounds.
    - **Execution Time**: Comparative analysis of algorithmic vs. LLM inference time.

## Repository Structure

- `creation_and_visualization.ipynb`: Tools for maze generation and visualization of algorithmic paths.
- `maze_creation_and_llama-70b.ipynb`: Experimentation with Llama-3.1-70b.
- `maze_creation_and_llama-3.1-8b.ipynb`: Experimentation with Llama-3.1-8b.
- `maze_creation_and_gpt-oss_20b.ipynb`: Experimentation with GPT-OSS-20b.
- `results_*.csv`: Detailed statistics from the experiments.
- **`Research work by @arafnel.pdf`**: The complete research paper detailing the findings, analysis, and conclusions.

## Research Paper

The formal documentation of this study can be found in the file `Research work by @arafnel.pdf` included in this repository. It covers the theoretical background, experimental setup, and in-depth results.

---
*Research work by @arafnel*
