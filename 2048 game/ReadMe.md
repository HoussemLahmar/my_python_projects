# 2048 Game in Python

This is a simple Python implementation of the popular 2048 game. Below you'll find the logic and code for the game. 

## How to Play

1. **Initialization**: The game starts with a 4x4 grid where two random cells are filled with the number 2.

2. **Movement**: Use the following commands to move the tiles in the grid:
    - 'W' or 'w': Move Up
    - 'S' or 's': Move Down
    - 'A' or 'a': Move Left
    - 'D' or 'd': Move Right

3. **Game Progression**:
    - When you press a key, the elements in the grid move in that direction.
    - If two identical numbers are adjacent in a row (for left/right movement) or column (for up/down movement), they combine into one with double the value. The extreme cell in that direction is filled with the resulting number, and the rest become empty.
    - After each move, a random empty cell gets filled with the number 2.
    - Continue making moves to try and reach the number 2048 in any cell.
  
4. **Winning**: If you successfully get the number 2048 in any cell, you win the game.

5. **Losing**: If there are no empty cells left to be filled with a new 2, the game is over.

## Example Gameplay

Commands are as follows:
'W' or 'w': Move Up
'S' or 's': Move Down
'A' or 'a': Move Left
'D' or 'd': Move Right

Initial State:
[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 2, 0]

Press the command: a
GAME NOT OVER
[0, 0, 0, 2]
[0, 0, 0, 0]
[0, 0, 0, 0]
[2, 0, 0, 0]

Press the command: s
GAME NOT OVER
[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 2, 0]
[2, 0, 0, 2]

Press the command: d
GAME NOT OVER
[0, 0, 0, 0]
[0, 0, 0, 0]
[2, 0, 0, 2]
[0, 0, 0, 4]

Press the command: a
GAME NOT OVER
[0, 2, 0, 0]
[0, 0, 0, 0]
[4, 0, 0, 0]
[4, 0, 0, 0]

Press the command: s
GAME NOT OVER
[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 0, 0]
[8, 2, 0, 2]


Continue playing until you win or lose.
