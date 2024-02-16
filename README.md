# Sudoku Solver 🧩

## Overview
This Sudoku Solver is a Python-based tool 🛠️ designed to tackle Sudoku puzzles 🎲 of varying difficulties using different algorithms. It incorporates three primary solving methods: backtracking, forward checking, and a heuristic approach that combines forward checking with additional strategies for selecting variables and values. This solver not only provides a solution to the given Sudoku puzzle but also offers insights into the computational efficiency of each solving method.

## Features
- **Multiple Solving Methods:** Utilizes backtracking, forward checking, and heuristic approaches to find solutions. 🕵️‍♂️
- **Performance Analysis:** Records and displays the number of moves and time taken to solve puzzles, providing an average and standard deviation for multiple runs. 📊
- **Versatility:** Capable of solving puzzles of varying difficulties, from easy to evil. 🔄
- **Randomization:** Introduces randomness in selecting values and empty blocks to potentially optimize the solving process. 🎲

## How to Use
To use the Sudoku Solver, execute the script with specific arguments that define the puzzle's difficulty level, the solving method, and the number of trials for performance analysis.

### Syntax
```sh
python sudoku.py <level> <method> <number of trials>
```
- `<level>`: A number from 1 to 4, indicating the puzzle difficulty (1: Easy 🟢, 2: Medium 🟡, 3: Hard 🔴, 4: Evil 🟣).
- `<method>`: A number from 1 to 3, specifying the solving method (1: Backtracking 🔄, 2: Forward Checking 🔍, 3: Heuristic 🧠).
- `<number of trials>`: The number of times the solver will run to provide average performance metrics. 🔢

### Requirements
- Python 3.x 🐍
- Basic libraries: `random`, `time`, `sys`, `statistics`

## Implementation Details
The solver uses several key functions to navigate and solve the Sudoku puzzles:

- **`print_board(arr)`:** Prints the current state of the Sudoku board. 📋
- **`valid(board, row, col, value)`:** Checks if a given value can be placed in a specific position without violating Sudoku rules. ✅
- **`solve_backtracking(board, empty_blocks, position)`:** Implements the backtracking algorithm. 🔙
- **`solve_forwardchecking(board, empty_blocks, position)`:** Enhances the backtracking approach with forward checking to prune the search space. 🔎
- **`solve_heuristic(board)`:** Applies heuristic methods, including selecting the most constrained variables and the least constraining values, alongside forward checking. 💡

## Performance Metrics
After solving a puzzle, the script outputs the solution along with performance metrics, including the average and standard deviation of moves and time taken across the specified number of trials. This data helps in comparing the efficiency of the different solving methods under various puzzle difficulties. 📈

## Conclusion
This Sudoku Solver is a powerful tool for enthusiasts looking to explore different solving algorithms and their efficiencies. Whether you're a beginner or an advanced player, this script offers valuable insights into the complexities of Sudoku puzzles and the effectiveness of algorithmic strategies in conquering them. 🏆
