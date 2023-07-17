# Atom Jump - Chain Reaction Board Game

## Introduction

Atom Jump is a web-based chain reaction board game built using HTML, CSS, and JavaScript. Players take turns placing atoms on a 6x6 grid, triggering chain reactions that can capture territory. The objective is to create a connected chain of atoms of your color spanning the entire grid. The game uses the Breadth-First Search (BFS) algorithm to determine when it ends.

## How to Play

1. **Objective**: Create a connected chain of your color's atoms spanning the grid.
2. **Setup**: Players take turns placing atoms on empty cells of the grid.
3. **Chain Reactions**: Cells with maximum atoms trigger chain reactions, jumping to neighboring cells.
4. **Capturing Territory**: Chain reactions capture territory for the initiating player.
5. **Game Over**: The game ends when one player captures enough territory to block the opponent's chain.

## Methodology - BFS Algorithm

1. **Graph Representation and Chain Reaction**: Atom Jump utilizes a graph representation for the game board, with each cell as a node in the graph. Cells are connected based on their neighboring cells. When players place atoms on the board, a chain reaction can occur when a cell's atom count reaches the maximum number of its neighbors. The chain reaction causes atoms to jump to neighboring cells, potentially triggering further reactions. This dynamic gameplay element creates opportunities for strategic territory capturing and chain formation.

2. **BFS Algorithm for Game Over Detection**: To determine when the game is over and identify connected chains of atoms, the game employs the Breadth-First Search (BFS) algorithm. When a player places an atom, the BFS algorithm explores all connected nodes (cells) of the same color starting from the placed cell. It efficiently traverses the graph, utilizing a `Set` data structure to avoid revisiting explored cells. The BFS algorithm helps detect when one player captures enough territory to block the opponent's chain, leading to the end of the game and declaring the winner. By using the BFS algorithm, the game ensures fair and precise game-ending conditions, enhancing the strategic depth and competitiveness of Atom Jump.

## Features

- Interactive 6x6 grid board game.
- Place atoms, trigger chain reactions, and capture territory.
- Auto-detect game over and display the winner.
- "New Game" button to start fresh.

## Getting Started

1. Clone the repository.
2. Open `index.html` in your browser.

## Output


## Contributors
* [Siddhi Patil](https://github.com/Siddhi-Patil06)
* [Mrunmayee Phadke](https://github.com/Mrunmayee-762004)
* [Rahul Sundkar](https://github.com/RahulSundkar)
* [Rajkumar Dongre](https://github.com/rajkumardongre)
* [Atharva Raut](https://www.linkedin.com/in/atharva-raut-4b3296228/)
