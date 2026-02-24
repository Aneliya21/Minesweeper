# 🎮 Minesweeper Project Overview

### Intoduction to Programming Practicum Course - Final project

#### This is a console-based implementation of the classic Minesweeper game. At the start of the game, the user configures the board size and the difficulty level by specifying the number of hidden mines.
___

#### Configuration

Upon launching, the game prompts the user for two inputs:
>Grid Dimension ($N$): The size of the square board ($3 \le N \le 10$).

>Mines Count: The number of hidden mines, which must be within the range $[1 : 3N]$.

⚠️ If the user enters invalid values, the program will display an error message and prompt the user to re-enter the data until valid inputs are provided.
___
#### How to play?

The game is controlled via console commands using the following syntax:
```
[command] [x_coordinate] [y_coordinate]
```
___
#### SupportedCommands

| Command | Action | Description |
| :--- | :--- | :--- |
| **open** | Open Cell | Reveals the content of the cell. If it contains a mine—**Game Over!** |
| **mark** | Flag Mine | Marks a cell as a suspected mine. |
| **unmark** | Remove Flag | Removes a mark from a cell. If the cell wasn't marked, an error message is shown. |

#### Winning Conditions

The player wins the game when:
> All mines have been correctly marked.

> All remaining safe cells have been opened.
