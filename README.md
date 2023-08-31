# Maze Solver using Local Search

This repository contains a Python implementation of a maze solver using local search techniques. The maze solver aims to find a path from the start (A) to the goal (B) through a maze. The program provides visualization of the maze and the solution.

## Usage

1. Ensure you have Python installed on your system.
2. Open a terminal/command prompt.
3. Run the following command to execute the maze solver:

# Classes
## Node
Represents a node in the search tree.

**Attributes:**

- `state`: The state of the node.
- `parent`: The parent node.
- `action`: The action taken to reach this node.

## StackFrontier
A stack-based implementation of the frontier for Depth-First Search.

**Methods:**

- `add(node)`: Adds a node to the frontier.
- `contains_state(state)`: Checks if a state is in the frontier.
- `empty()`: Checks if the frontier is empty.
- `remove()`: Removes and returns the last node from the frontier.

## QueueFrontier
A queue-based implementation of the frontier for Breadth-First Search.

**Methods:**

- `add(node)`: Adds a node to the frontier.
- `contains_state(state)`: Checks if a state is in the frontier.
- `empty()`: Checks if the frontier is empty.
- `remove()`: Removes and returns the first node from the frontier.

## Maze
Represents a maze and provides methods to solve and visualize it.

**Methods:**

- `__init__(filename)`: Initializes the maze from a file.
- `print()`: Prints the maze with walls, start, and goal.
- `neighbors(state)`: Returns neighboring states of a given state.
- `solve()`: Finds a solution to the maze using local search.
- `output_image(filename, show_solution=True, show_explored=False)`: Outputs the maze as an image.

# Usage Example
To use the maze solver, follow the usage instructions provided above. The program will read the maze from a text file and attempt to find a solution.

# Contributing
Contributions to this project are welcome. Feel free to open issues and pull requests.
