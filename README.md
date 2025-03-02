# Tic-Tac-Toe (Tkinter Edition)

A simple **Tic-Tac-Toe** game built using **Python** and **Tkinter** for the graphical user interface (GUI).

## Features
- **Classic Tic-Tac-Toe Gameplay**: Two players (X and O) take turns marking the 3×3 grid.
- **Basic UI with Tkinter**: Simple and clean graphical user interface using Tkinter.
- **Win/Tie Detection**: Automatically checks for a winner or a tie after each move.
- **Message Box Alerts**: Displays a pop-up message when a player wins or when the game ends in a tie.
- **Automatic Board Reset**: Resets the board after a win or tie.

## Installation and Setup
### 1. Download the Game from GitHub
To get the game, clone the repository using the following command:
```sh
 git clone https://github.com/Sanjay1712KSK/Tic-Tac-Toe.git
```
Alternatively, you can download the ZIP file from GitHub and extract it manually.

### 2. Navigate to the Project Directory
Once downloaded, open a terminal or command prompt and move into the project folder:
```sh
 cd Tic-Tac-Toe
```

### 3. Run the Game
Ensure you have **Python 3** installed on your system. Since Tkinter is included by default in Python, no additional installation is needed. Simply execute:
```sh
 python tic_tac_toe.py
```

## Output Screenshots
```md
 ![Winning Game Screenshot](https://github.com/Sanjay1712KSK/Tic-Tac-Toe/blob/main/image.png)
```

## Strategies Used
1. **Turn-Based Player Switching**: The game starts with Player **X**, and after each valid move, it switches to **O**.
2. **Win Detection Mechanism**:
   - Checks all **rows**, **columns**, and **diagonals** to determine a winner.
3. **Tie Detection Mechanism**:
   - If all grid positions are filled without a winner, the game ends in a tie.
4. **Game Reset Feature**:
   - After a win or tie, the board resets automatically.

## Code Explanation
### Main Components:
- **Grid Creation (`create_buttons`)**: Creates a 3×3 button grid using Tkinter’s `Button` widget.
- **Handling Button Clicks (`on_button_click`)**:
  - Updates the button text with the current player's mark (`X` or `O`).
  - Calls `check_winner()` to determine if there’s a winner.
  - Calls `check_tie()` to check if the grid is full.
  - Switches turns if no winner is found.
- **Checking Game State (`check_winner` and `check_tie`)**:
  - Evaluates whether a player has won by checking row, column, and diagonal matches.
  - Determines if the grid is full without a winner (tie condition).
- **Resetting the Game (`reset_board`)**:
  - Clears the board and sets the next turn to **Player X**.

## Possible Improvements
- **AI Opponent**: Implement a basic AI using the **Minimax algorithm** for single-player mode.
- **Score Tracking**: Keep track of player wins.
- **Enhanced UI**: Add color themes and animations for better user experience.

## License
This project is open-source and available under the **GNU GENERAL PUBLIC LICENSE**.

---

Enjoy the game! 🎮

