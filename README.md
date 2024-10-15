
# Maze Solver Project

This project is a simple **maze solver** using the **Breadth-First Search (BFS)** algorithm to find the shortest path between a start point and an end point in a maze. The maze is represented as a grid, and the algorithm explores each cell of the maze to find the optimal solution.

## Table of Contents

- [Description](#description)
- [Requirements](#requirements)
- [How It Works](#how-it-works)
- [Features](#features)
- [Usage](#usage)
- [Customization](#customization)
- [License](#license)

## Description

The **Maze Solver** project demonstrates how to implement the BFS algorithm to find the shortest path through a maze. The maze is represented as a 2D grid where:
- `#` represents walls (non-passable).
- `O` represents the starting point.
- `X` represents the ending point.
- `" "` represents open spaces (passable).

The goal is to find the shortest path from `O` (start) to `X` (end), while avoiding walls. The algorithm explores the maze step-by-step, showing the progress in real-time.

## Requirements

To run this project, you'll need:
- Python 3.x (preferably 3.10+)
- `time` module (standard in Python)
- `queue` module (standard in Python)

> Note: No additional external libraries are required.

## How It Works

The algorithm used is **Breadth-First Search (BFS)**, which works by exploring all the neighboring cells at the current depth before moving on to the cells at the next depth level. This ensures that the shortest path is found in an unweighted grid like the maze.

- The start point `O` is found and added to a queue.
- Each neighboring cell (up, down, left, right) is explored one by one.
- If the end point `X` is reached, the algorithm stops and prints the path.
- The maze is printed in each step to show the current exploration status.

## Features

- **Maze Representation**: The maze is stored in a list of lists and can be customized.
- **Breadth-First Search**: Ensures that the shortest path is found.
- **Real-time Visualization**: The maze is displayed in the terminal as the path is being explored.
- **Pathfinding**: Finds the shortest path between two points in the maze.

## Usage

1. Clone the repository or download the code.
2. Open a terminal and navigate to the project directory.
3. Run the script using Python:
   ```bash
   python maze_solver.py
   ```
4. The script will print the maze and display the pathfinding progress step-by-step. The path to the goal will be marked with `X` symbols.

### Example Maze:

```
# O # # # # # # #
#               #
#   # #   # #   #
#   #     #     #
#   # #   #   # #
#   # #   #     #
#   # #   # # # #
#               #
# # # # # # # X #
```

### Example Output:

The algorithm will explore the maze step-by-step and print the maze at each stage, showing the progress toward the goal.

## Customization

You can modify the maze by changing the `maze` list in the script. For example, add more walls, change the start (`O`) and end (`X`) positions, or modify the size of the maze.

### Customizing the Maze

To change the maze, edit the `maze` variable in the script:
```python
maze = [
    ["#", "O", "#", "#", "#", "#", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", " ", "#", "#", " ", "#", "#", " ", "#"],
    ["#", " ", "#", " ", " ", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", "#", "#", "#", "#", "#", "#", "X", "#"]
]
```

You can adjust the size, layout, and positions of walls, open spaces, start, and end points.

