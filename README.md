# Tic-Tac-Toe Game

Welcome to the Tic-Tac-Toe Game project! This simple web-based game allows two players to take turns and compete to get three of their symbols (X or O) in a row. This README provides essential information about the project, how to play the game, and details about the code structure.

## Table of Contents
- [Game Overview](#game-overview)
- [How to Play](#how-to-play)
- [Code Structure](#tic-tac-toe-game-logic-explanation)
- [Getting Started](#getting-started)
- [Contributing](#contributing)


## Game Overview

Tic-Tac-Toe is a classic two-player game where the objective is to get three of your symbols in a row (horizontally, vertically, or diagonally) on a 3x3 grid. Players take turns marking a square with their symbol (X or O), and the first player to achieve three in a row wins. The game can also end in a tie if no player wins and the grid is full.

![image](https://github.com/user-attachments/assets/6366935d-a69b-4bb3-b6b9-2da3246f9a5c)


## How to Play

1. **Initial Setup**: Open the `index.html` file in your web browser.

2. **Starting a New Game**: Click the "New Game" button to start a new game.

3. **Taking Turns**: Players take turns clicking on the empty squares to place their symbol (X or O). The current player is displayed at the top of the game board.

4. **Winning**: The game will automatically determine if a player has won by getting three of their symbols in a row. If a player wins, their name will be displayed as the winner.

5. **Tie**: If all squares are filled, and no player has won, the game ends in a tie.

6. **Restarting the Game**: After a game ends (either in a win or a tie), you can click the "New Game" button to start a new game.

## Tic-Tac-Toe Game Logic Explanation

This Tic-Tac-Toe game is implemented using HTML, CSS, and JavaScript, designed for two players to take turns placing "X" and "O" marks on a 3x3 grid. The game logic can be broken down as follows:

1. **Initialization**: The game starts with "X" as the starting player. A `game grid` array represents the grid state, and `winningPositions` defines possible winning combinations.

2. **Game Initialization**: `initGame()` resets the game by setting player "X," clearing the grid, enabling cell interactions, and removing the winning class.

3. **Checking for a Winner**: `checkGameOver()` checks for a winner by iterating through `winningPositions`. If a winning combo matches the grid, it displays the winner or a tie.

4. **Swapping Turns**: `swapTurn()` switches the current player between "X" and "O" and updates the game info.

5. **Handling Clicks**: Event listeners on cells call `handleClick(index)`, which updates the grid, disables clicks, swaps turns, and checks for a winner.

6. **New Game Button**: The "New Game" button resets the game with `initGame()`.

The code also features CSS classes to visually highlight the winning cells and disable further interaction with the grid after a win or tie. The game provides a clear interface with informative messages about the current player and the game's outcome.

This project offers a user-friendly and visually appealing implementation of the classic Tic-Tac-Toe game suitable for web applications or standalone use.

## Getting Started

To run this project locally, follow these steps:

1. Clone this repository to your local machine:
```sh
git clone https://github.co
```

2. Navigate to the project directory:
```sh
cd tic-tac-toe
```

3. Open the `index.html` file in your web browser to play the game.

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the project on GitHub.

2. Clone your forked repository to your local machine.

3. Create a new branch for your feature or bug fix:
```sh
git checkout -b feature/your-feature-name
```

4. Make your changes and commit them with descriptive commit messages:
```sh
git commit -m "Add new feature" or "Fix bug"
```

5. Push your changes to your GitHub repository:
```sh
git push origin feature/your-feature-name
```

6. Open a pull request on the original repository, explaining your changes and why they should be merged.
